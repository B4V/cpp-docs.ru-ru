---
title: Создание документа фрейма Windows | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-mfc
ms.topic: conceptual
dev_langs:
- C++
helpviewer_keywords:
- frame windows [MFC], creating
- document templates [MFC], and document frame windows
- windows [MFC], creating
- runtime, class information
- run-time class [MFC], and document frame window creation
- document frame windows [MFC], creating
- MFC, frame windows
ms.assetid: 8671e239-b76f-4dea-afa8-7024e6e58ff5
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 172076113a6bd7e223d99c238d0e05987cdcaae6
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46433703"
---
# <a name="creating-document-frame-windows"></a>Создание окон фрейма документа

[Создание документов и представлений](../mfc/document-view-creation.md) показано, как [CDocTemplate](../mfc/reference/cdoctemplate-class.md) объект организует Создание фрейм окна, документ и представление, а затем подключить их все вместе. Три [CRuntimeClass](../mfc/reference/cruntimeclass-structure.md) аргументы `CDocTemplate` конструктор укажите фрейм окна, документ и классы представлений, которые динамически создает шаблон документа в ответ на команды пользователя, например новой команды для файла меню или команды создания окна в меню окна интерфейса MDI. Шаблон документа сохраняет эти сведения для дальнейшего использования, когда он создает окно фрейма для представления и документа.

Для [RUNTIME_CLASS](../mfc/reference/run-time-object-model-services.md#runtime_class) механизм работал правильно, в производный классы окна фрейма, должна быть объявлена с [DECLARE_DYNCREATE](../mfc/reference/run-time-object-model-services.md#declare_dyncreate) макрос. Это обусловлено тем, необходимо создать документ с помощью механизма динамического создания класса окон фрейма платформ `CObject`.

Когда пользователь выбирает команду, которая создает документ, платформа вызывает шаблон документа, чтобы создать объект документа, его представлением и окном фрейма, который будет отображать представление. При создании окна фрейма документа, шаблон документа создает объект соответствующего класса — класс, производный от [CFrameWnd](../mfc/reference/cframewnd-class.md) для приложения SDI или из [CMDIChildWnd](../mfc/reference/cmdichildwnd-class.md) для MDI приложение. Затем вызывается метод объекта окна фрейма [LoadFrame](../mfc/reference/cframewnd-class.md#loadframe) функция-член для получения сведения о создании ресурсов и для создания окна Windows. Платформа прикрепляет дескриптор окна к объекту окна фрейма. Затем он создает представление как дочернего окна фрейма окна документа.

Соблюдайте осторожность при выборе [время инициализации](../mfc/when-to-initialize-cwnd-objects.md) вашей `CWnd`-объект, производный от.

## <a name="what-do-you-want-to-know-more-about"></a>Выберите для получения дополнительных сведений

- [Наследование класса от CObject (динамическое создание механизма)](../mfc/deriving-a-class-from-cobject.md)

- [Создание документов и представлений (шаблоны и Создание окон фрейма)](../mfc/document-view-creation.md)

- [Уничтожение окон фрейма](../mfc/destroying-frame-windows.md)

## <a name="see-also"></a>См. также

[Использование окон фрейма](../mfc/using-frame-windows.md)

