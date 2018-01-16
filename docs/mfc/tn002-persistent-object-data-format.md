---
title: "TN002: Формат данных постоянного объекта | Документы Microsoft"
ms.custom: 
ms.date: 11/04/2016
ms.reviewer: 
ms.suite: 
ms.technology: cpp-windows
ms.tgt_pltfrm: 
ms.topic: article
f1_keywords: vc.data
dev_langs: C++
helpviewer_keywords:
- VERSIONABLE_SCHEMA macro [MFC]
- persistent object data
- CArchive class [MFC], support for persistent data
- persistent C++ objects [MFC]
- TN002
ms.assetid: 553fe01d-c587-4c8d-a181-3244a15c2be9
caps.latest.revision: "22"
author: mikeblome
ms.author: mblome
manager: ghogen
ms.workload: cplusplus
ms.openlocfilehash: ca6a78f19b43ded59efb56b87f9fe3f44887a31a
ms.sourcegitcommit: 8fa8fdf0fbb4f57950f1e8f4f9b81b4d39ec7d7a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/21/2017
---
# <a name="tn002-persistent-object-data-format"></a>TN002. Формат данных постоянного объекта
Эта заметка описывает MFC подпрограммы, которые поддерживают постоянные объекты C++ и формат данных объекта, когда он хранится в файле. Это относится только к классам с [DECLARE_SERIAL](../mfc/reference/run-time-object-model-services.md#declare_serial) и [IMPLEMENT_SERIAL](../mfc/reference/run-time-object-model-services.md#implement_serial) макросы.  
  
## <a name="the-problem"></a>Проблема  
 Реализация MFC для постоянных данных хранит данные для нескольких объектов в смежных часть файла. Объект `Serialize` метод преобразует объект данных в компактный двоичный формат.  
  
 Реализация гарантирует, что все данные сохраняются в том же формате с помощью [CArchive-класс](../mfc/reference/carchive-class.md). Она использует `CArchive` объект функции преобразователя. Этот объект будет повторяться с момента его создания до вызова [CArchive::Close](../mfc/reference/carchive-class.md#close). Этот метод может вызываться явным образом программистом или неявно деструктором при выходе программы к области, содержащей `CArchive`.  
  
 Эта заметка описывается реализация `CArchive` элементы [CArchive::ReadObject](../mfc/reference/carchive-class.md#readobject) и [CArchive::WriteObject](../mfc/reference/carchive-class.md#writeobject). Вы найдете код для этих функций в Arcobj.cpp и реализации основных `CArchive` в Arccore.cpp. Пользовательский код не вызывает `ReadObject` и `WriteObject` напрямую. Вместо этого эти объекты используются данного класса строго типизированным операторов вставки и извлечения, созданные автоматически `DECLARE_SERIAL` и `IMPLEMENT_SERIAL` макросы. В следующем коде показано, как `WriteObject` и `ReadObject` являются неявно вызывается:  
  
```  
class CMyObject : public CObject  
{  
    DECLARE_SERIAL(CMyObject) 
};  
 
IMPLEMENT_SERIAL(CMyObj, CObject, 1)  
 
// example usage (ar is a CArchive&)  
CMyObject* pObj;  
CArchive& ar;  
ar <<pObj;        // calls ar.WriteObject(pObj)  
ar>> pObj;        // calls ar.ReadObject(RUNTIME_CLASS(CObj))  
```  
  
## <a name="saving-objects-to-the-store-carchivewriteobject"></a>Сохранение объектов в хранилище (CArchive::WriteObject)  
 Метод `CArchive::WriteObject` записывает данные заголовка, который используется для воссоздания объекта. Эти данные состоит из двух частей: тип объекта и состояние объекта. Этот метод также отвечает за поддержание удостоверение объекта, которая записывается, так, что сохраняется только по одной копии, независимо от количества указателей на этот объект (включая циклические указатели).  
  
 Сохранение (Вставка) и восстановление объектов (извлечение) зависит от нескольких «констант манифеста.» Это значения, которые хранятся в двоичном формате и содержат важную информацию в архив (Обратите внимание, что префикс «w» указывает количества 16-разрядное):  
  
|Тег|Описание:|  
|---------|-----------------|  
|wNullTag|Используется для указателей на объекты NULL (0).|  
|wNewClassTag|Указывает, что класс описание, которое следует за является новой возможностью в этом контексте архива (-1).|  
|wOldClassTag|Указывает, что класс объекта, считываемое встречалась в этом контексте (0x8000).|  
  
 Во время сохранения объектов, архив сохраняет [CMapPtrToPtr](../mfc/reference/cmapptrtoptr-class.md) ( `m_pStoreMap`) это сопоставление из сохраненного объекта в 32-разрядных постоянный идентификатор (PID). PID назначается каждый уникальный объект и каждый уникальное имя класса, сохраненный в контексте архива. Эти PID предоставленному последовательно, начиная с 1. Эти PID не имеет значения за пределами области архив и находятся в частности, не следует путать с номера записей и прочих идентификаторов.  
  
 В `CArchive` класс, PID являются 32-разрядными, но они записываются как 16-разрядное пока не будут больше, чем 0x7FFE. Большие PID записываются в виде 0x7FFF следуют PID 32-разрядной. Это обеспечивает совместимость с проектами, которые были созданы в более ранних версиях.  
  
 При выполнении запроса для сохранения объекта в архив (обычно с помощью оператора глобальной вставки), выполняется проверка на значение NULL, [CObject](../mfc/reference/cobject-class.md) указателя. Если указатель имеет значение NULL, `wNullTag` вставляется в архивный поток.  
  
 Если указатель не имеет значение NULL и может быть сериализован (класс `DECLARE_SERIAL` класса), этот код проверяет `m_pStoreMap` чтобы увидеть, является ли объект уже сохранен. Если Да, этот код вставляет 32-разрядных PID, связанные с этим объектом в архивный поток.  
  
 Если объект не сохранялся, есть две возможности, которые следует учитывать: объект и точный тип объекта (то есть класс) являются новыми для данного содержимого архива или объект имеет точный тип уже видели. Чтобы определить, является ли тип было выявлено, кода запросы `m_pStoreMap` для [CRuntimeClass](../mfc/reference/cruntimeclass-structure.md) объект, который соответствует `CRuntimeClass` объект, связанный с объектом, который сохраняется. Если соответствие, `WriteObject` вставляет тег, который является побитовое `OR` из `wOldClassTag` и этот индекс. Если `CRuntimeClass` является новой возможностью в данном контексте архив `WriteObject` назначает новый номер продукта для этого класса и вставляет его в архив, предшествует `wNewClassTag` значение.  
  
 Дескриптор для данного класса затем вставляется в архив с помощью `CRuntimeClass::Store` метод. `CRuntimeClass::Store`Вставляет номер схемы классов (см. ниже) и имя класса текста ASCII. Обратите внимание, что использование имени текста ASCII не гарантирует уникальность архива в приложениях. Таким образом следует пометить файлы данных, чтобы избежать повреждения. После вставки информация о классе, архив помещает объект в `m_pStoreMap` , а затем вызывает `Serialize` для вставки данных определенного класса. Перевести объект в `m_pStoreMap` перед вызовом `Serialize` предотвращает сохранение в хранилище несколько копий объекта.  
  
 При возврате изначальной вызывающей стороны (обычно корневой сетевых объектов), необходимо вызвать [CArchive::Close](../mfc/reference/carchive-class.md#close). Если планируется для выполнения других [CFile](../mfc/reference/cfile-class.md)операций, необходимо вызвать `CArchive` метод [Flush](../mfc/reference/carchive-class.md#flush) во избежание повреждения архива.  
  
> [!NOTE]
>  Эта реализация налагает жесткий предел 0x3FFFFFFE индексов каждого контекста архива. Это число представляет максимальное число уникальных объектов и классы, которые могут быть сохранены в один архив, но один дисковый файл может иметь неограниченное число контекстов архива.  
  
## <a name="loading-objects-from-the-store-carchivereadobject"></a>Загрузка объектов из хранилища (CArchive::ReadObject)  
 Загрузка (извлечение) объектов использует `CArchive::ReadObject` метод и обратный `WriteObject`. Как и в `WriteObject`, `ReadObject` не вызывается непосредственно в пользовательском коде; пользовательский код должен вызывать оператор извлечения строго типизированным, который вызывает `ReadObject` с ожидаемым `CRuntimeClass`. Это гарантирует целостность тип операции извлечения.  
  
 Так как `WriteObject` реализацию назначенный возрастающей PID, начиная с 1 (как объект NULL предварительно 0), `ReadObject` реализация может использовать массив для сохранения состояния контекста архива. При считывании PID из хранилища, если код продукта больше текущей верхней границы `m_pLoadArray`, `ReadObject` знает, что следует нового объекта (или описание класса).  
  
## <a name="schema-numbers"></a>Номера схемы  
 Номер схемы, которой присваивается класс при `IMPLEMENT_SERIAL` метод класса встречается, является «версия» реализацию класса. Схема относится реализации класса, не на число попыток данного объекта была предпринята постоянные (обычно называют версии объекта).  
  
 Если вы собираетесь постоянно поддерживать несколько различных реализаций того же класса, увеличивая схемы в исправленном объекта `Serialize` реализации метода позволит написать код, который можно загрузить объекты, сохраненные с помощью более ранних версий Реализация.  
  
 `CArchive::ReadObject` Метод вызывает исключение [CArchiveException](../mfc/reference/carchiveexception-class.md) при обнаружении несколько схем в постоянное хранилище, которое отличается от схемы числа описания класса в памяти. Это не просто восстановить из этого исключения.  
  
 Можно использовать `VERSIONABLE_SCHEMA` в сочетании с (побитовое `OR`) на версию схемы, чтобы сохранить это исключение вызывается. С помощью `VERSIONABLE_SCHEMA`, код может выполнять необходимые действия его `Serialize` функция, установив значение, возвращаемое [CArchive::GetObjectSchema](../mfc/reference/carchive-class.md#getobjectschema).  
  
## <a name="calling-serialize-directly"></a>Вызов непосредственно сериализации  
 Во многих случаях издержки схема архива общие объекта `WriteObject` и `ReadObject` не требуется. Это стандартный вариант сериализации данных в [CDocument](../mfc/reference/cdocument-class.md). В этом случае `Serialize` метод `CDocument` вызывается напрямую, не с помощью операторов извлечения или insert. Содержимое документа в свою очередь могут использовать схему архив более общих объекта.  
  
 Вызов `Serialize` непосредственно имеет следующие преимущества и недостатки:  
  
-   Дополнительные байты не добавляются в архиве до или после сериализации объекта. Это не только упрощает сохраненных данных меньшего размера, но позволяет реализовать `Serialize` подпрограммы, которые можно обрабатывать все форматы файлов.  
  
-   MFC настраивается таким образом `WriteObject` и `ReadObject` реализации и соответствующих коллекций не будет связан в приложение бесполезно, если схему более общих объектов архива для некоторых других целей.  
  
-   Код не имеет для восстановления из старого номера схемы. Это делает код сериализации документа ответственность за кодирования схемы номеров файл формата версии, и любое определение порядковые номера использовать в начале файлы данных.  
  
-   Любой объект, который сериализуется с использованием прямого вызова `Serialize` не должны использовать `CArchive::GetObjectSchema` или необходимо дескриптор возвращаемое значение (UINT) -1, указывающую на версию Неизвестный.  
  
 Поскольку `Serialize` вызывается непосредственно в документе, это обычно невозможно для вложенных объектов документа, чтобы архивировать ссылки на их родительский документ. Эти объекты необходимо предоставить указатель в документе-контейнере явным образом или необходимо использовать [CArchive::MapObject](../mfc/reference/carchive-class.md#mapobject) функция, сопоставляющая `CDocument` указатель PID, прежде чем эти обратные указатели архивируются.  
  
 Как отмечалось ранее, необходимо закодировать версии и информация о классе самостоятельно при вызове `Serialize` напрямую, что позволяет позднее изменить формат, поддерживая обратную совместимость с более старыми версиями файлов. `CArchive::SerializeClass` Функция может вызываться явным образом до сериализации объекта непосредственно или перед вызовом базового класса.  
  
## <a name="see-also"></a>См. также  
 [Технические примечания по номеру](../mfc/technical-notes-by-number.md)   
 [Технические примечания по категории](../mfc/technical-notes-by-category.md)
