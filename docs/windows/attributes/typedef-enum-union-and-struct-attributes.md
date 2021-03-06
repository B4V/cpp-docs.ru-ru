---
title: TypeDef, Enum, Union и Struct атрибуты (C++ COM) | Документация Майкрософт
ms.custom: ''
ms.date: 10/02/2018
ms.technology:
- cpp-windows
ms.topic: reference
dev_langs:
- C++
helpviewer_keywords:
- union attributes
- attributes [C++/CLI], reference topics
ms.assetid: f8a4fe94-dc02-4aed-bc31-3e500d42f4c7
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
- uwp
ms.openlocfilehash: 89e1511df2aeabe7cbd63549a1dca6e53944fbe2
ms.sourcegitcommit: 955ef0f9d966e7c9c65e040f1e28fa83abe102a5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/04/2018
ms.locfileid: "48792221"
---
# <a name="typedef-enum-union-and-struct-attributes"></a>Атрибуты Typedef, Enum, Union и Struct

Следующие атрибуты применяются к [typedef](../../cpp/aliases-and-typedefs-cpp.md), [структуры](../../cpp/struct-cpp.md), и [перечисления](../../cpp/enumerations-cpp.md) ключевые слова C++.

### <a name="typedef"></a>typedef

|Атрибут|Описание|
|---------------|-----------------|
|[case](case-cpp.md)|Используется с [switch_type](switch-type.md) атрибут в **объединение**.|
|[Custom](custom-cpp.md)|Позволяет определять собственный атрибут.|
|[export](export.md)|В результате структуру данных, должно быть помещено в IDL-файла.|
|[first_is](first-is.md)|Указывает индекс первого элемента массива для передачи.|
|[helpcontext](helpcontext.md)|Указывает идентификатор контекста, который позволяет пользователю просматривать сведения об этом элементе в файле справки.|
|[helpfile](helpfile.md)|Задает имя файла справки для библиотеки типов.|
|[helpstring](helpstring.md)|Определяет строку символов, используемую для описания элемента, к которому оно применяется.|
|[library_block](library-block.md)|Помещает конструкцию внутри блока библиотеки в IDL-файл.|
|[ptr](ptr.md)|Определяет указатель как полный указатель.|
|[public](public-cpp-attributes.md)|Гарантирует, что typedef перейдет в библиотеке типов, даже если нет ссылок из в IDL-файла.|
|[ref](ref-cpp.md)|Определяет указатель ссылки.|
|[switch_is](switch-is.md)|Указывает выражение или идентификатор, действующий как объединения дискриминантный, который выбирает член объединения.|
|[switch_type](switch-type.md)|Определяет тип переменной, которая используется в качестве объединения дискриминантный.|
|[unique](unique-cpp.md)|Указывает уникальный указатель.|
|[wire_marshal](wire-marshal.md)|Указывает тип данных, который будет использоваться для передачи данных вместо типа данных приложения.|

### <a name="enum"></a>перечисление

|Атрибут|Описание|
|---------------|-----------------|
|[Custom](custom-cpp.md)|Позволяет определять собственный атрибут.|
|[export](export.md)|В результате структуру данных, должно быть помещено в IDL-файла.|
|[uuid](uuid-cpp-attributes.md)|Указывает уникальный идентификатор для класса или интерфейса.|
|[v1_enum](v1-enum.md)|Указывает, что заданного перечислимого типа, передаваться в объект 32-разрядной, а не по умолчанию 16-разрядное.|

### <a name="union"></a>union

|Атрибут|Описание|
|---------------|-----------------|
|[Custom](custom-cpp.md)|Позволяет определять собственный атрибут.|
|[export](export.md)|В результате структуру данных, должно быть помещено в IDL-файла.|
|[first_is](first-is.md)|Указывает индекс первого элемента массива для передачи.|
|[last_is](last-is.md)|Указывает индекс последнего элемента массива для передачи.|
|[length_is](length-is.md)|Указывает количество элементов массива для передачи.|
|[max_is](max-is.md)|Определяет максимальное значение для индекса допустимым массивом.|
|[size_is](size-is.md)|Указывает объем памяти, выделенной для размера указатели, размер указателей на указатели по размеру и одно - или многомерные массивы.|
|[unique](unique-cpp.md)|Указывает уникальный указатель.|
|[uuid](uuid-cpp-attributes.md)|Указывает уникальный идентификатор для класса или интерфейса.|

### <a name="nonencapsulated-union"></a>Nonencapsulated union

|Атрибут|Описание|
|---------------|-----------------|
|[ms_union](ms-union.md)|Управляет выравниванием представление данных сети nonencapsulated объединений.|
|[no_injected_text](no-injected-text.md)|Запрещает компилятору вставку кода в результате использования атрибута.|

### <a name="struct"></a>структура

|Атрибут|Описание|
|---------------|-----------------|
|[aggregatable](aggregatable.md)|Указывает, что класс поддерживает агрегирование.|
|[aggregates](aggregates.md)|Указывает, что элемент управления использует статистическую функцию целевого класса.|
|[appobject](appobject.md)|Идентифицирует сокласс как объект приложения, который связан с приложением полный .exe и указывает, что функциях и свойствах компонентного класса доступны глобально в этой библиотеки типов.|
|[coclass](coclass.md)|Создает элемент управления ActiveX.|
|[COM_INTERFACE_ENTRY](com-interface-entry-cpp.md)|Добавляет запись интерфейс COM карты.|
|[control](control.md)|Указывает, что определяемый пользователем тип элемента управления.|
|[Custom](custom-cpp.md)|Позволяет определять собственный атрибут.|
|[db_column](db-column.md)|Связывает указанный столбец набора строк.|
|[db_command](db-command.md)|Создает команду OLE DB.|
|[db_param](db-param.md)|Связывает указанный член переменной с входным или выходным параметром и разделяет переменной.|
|[db_source](db-source.md)|Создает подключение к источнику данных.|
|[db_table](db-table.md)|Открывает таблицу OLE DB.|
|[default](default-cpp.md)|Указывает, что настраиваемый или disp-интерфейс, определенный в коклассе, представляет интерфейс программирования по умолчанию.|
|[defaultvtable](defaultvtable.md)|Определяет интерфейс как интерфейс vtable по умолчанию для элемента управления.|
|[event_receiver](event-receiver.md)|Создает приемник событий.|
|[event_source](event-source.md)|Создает источник событий.|
|[export](export.md)|В результате структуру данных, должно быть помещено в IDL-файла.|
|[first_is](first-is.md)|Указывает индекс первого элемента массива для передачи.|
|[hidden](hidden.md)|Указывает, что элемент существует, но не должен отображаться в пользовательском браузере.|
|[implements_category](implements-category.md)|Указывает категории реализованного компонента для класса.|
|[last_is](last-is.md)|Указывает индекс последнего элемента массива для передачи.|
|[length_is](length-is.md)|Указывает количество элементов массива для передачи.|
|[max_is](max-is.md)|Определяет максимальное значение для индекса допустимым массивом.|
|[requires_category](requires-category.md)|Указывает необходимый компонент категории целевого класса.|
|[size_is](size-is.md)|Указывает объем памяти, выделенной для размера указатели, размер указателей на указатели по размеру и одно - или многомерные массивы.|
|[source](source-cpp.md)|В классе, задает интерфейсы COM-объекта источника для точек подключения. На свойства или метода указывает, что член возвращает объект или переменная типа VARIANT, являющейся источником событий.|
|[Работа с потоками](threading-cpp.md)|Указывает потоковую модель для COM-объекта.|
|[unique](unique-cpp.md)|Указывает уникальный указатель.|
|[uuid](uuid-cpp-attributes.md)|Указывает уникальный идентификатор для класса или интерфейса.|
|[version](version-cpp.md)|Идентифицирует конкретную версию несколькими версиями класса.|
|[vi_progid](vi-progid.md)|Указывает форму независящим от версии идентификатор ProgID.|

## <a name="see-also"></a>См. также

[Список атрибутов по использованию](attributes-by-usage.md)