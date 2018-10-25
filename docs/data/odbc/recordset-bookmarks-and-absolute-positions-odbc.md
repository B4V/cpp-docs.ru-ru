---
title: 'Набор записей: Закладки и абсолютное позиционирование (ODBC) | Документация Майкрософт'
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-data
ms.topic: conceptual
f1_keywords:
- SetAbsolutePosition
dev_langs:
- C++
helpviewer_keywords:
- CDBVariant class, bookmarks
- absolute positions, ODBC recordsets
- bookmarks, CDBVariant
- bookmarks, ODBC recordsets
- ODBC recordsets, absolute positions
- ODBC recordsets, bookmarks
- cursors [ODBC], absolute position in recordsets
- recordsets, bookmarks
- bookmarks
- SetAbsolutePosition method
- recordsets, absolute positions
- positioning records
- SetBookmark method
- record positioning
- GetBookmark method
- SetAbsolutePosition method, bookmarks
ms.assetid: 189788d6-33c1-41c5-9265-97db2a5d43cc
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
- data-storage
ms.openlocfilehash: 4e751ab86548f42e5ab9350f95cb2b49d813ec8c
ms.sourcegitcommit: a9dcbcc85b4c28eed280d8e451c494a00d8c4c25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2018
ms.locfileid: "50064079"
---
# <a name="recordset-bookmarks-and-absolute-positions-odbc"></a>Набор записей. Закладки и абсолютное позиционирование (ODBC)

Этот раздел относится к классам ODBC библиотеки MFC.

При перемещении по набору записей, часто требуется иметь возможность вернуться к конкретной записи. Закладки и абсолютное позиционирование записи предоставляют два таких метода.

Содержание раздела:

- [Использование закладок](#_core_bookmarks_in_mfc_odbc).

- [Как задать текущую запись, с помощью абсолютных положений](#_core_absolute_positions_in_mfc_odbc).

##  <a name="_core_bookmarks_in_mfc_odbc"></a> Закладки в MFC ODBC

Закладка однозначно определяет запись. При переходе по набору записей нельзя всегда полагаться на абсолютное положение записи, так как записи могут быть удалены из набора записей. Использование закладок является надежным способом для отслеживания позиции записи. Класс `CRecordset` предоставляет функции-члены для:

- Установка закладки для текущей записи, его можно сохранить в переменной ([GetBookmark](../../mfc/reference/crecordset-class.md#getbookmark)).

- Быстрое перемещение к определенной записи, указав ее закладки, ранее сохраненной в переменной ([SetBookmark](../../mfc/reference/crecordset-class.md#setbookmark)).

Приведенный ниже показано, как использовать эти функции-члены для пометки текущей записи и позже вернуться к нему.

```cpp
// rs is a CRecordset or
// CRecordset-derived object

CDBVariant varRecordToReturnTo;
rs.GetBookmark( varRecordToReturnTo );

// More code in which you
// move to other records

rs.SetBookmark( varRecordToReturnTo );
```

Необходимо извлечь базовый тип данных из [класс CDBVariant](../../mfc/reference/cdbvariant-class.md) объекта. Назначьте с `GetBookmark` и вернуться к закладке с `SetBookmark`.

> [!NOTE]
>  В зависимости от драйвера ODBC и тип набора записей закладки могут не поддерживаться. Можно легко определить, поддерживаются ли закладки, вызвав [CRecordset::CanBookmark](../../mfc/reference/crecordset-class.md#canbookmark). Кроме того, поддерживаются ли закладки, необходимо явно выбрать их реализации, указав `CRecordset::useBookmarks` в диалоговом окне [CRecordset::Open](../../mfc/reference/crecordset-class.md#open) функция-член. Следует также проверить наличие закладок после определенных операций набор записей. Например если вы `Requery` recordset, закладки больше не может быть допустимым. Вызовите [CDatabase::GetBookmarkPersistence](../../mfc/reference/cdatabase-class.md#getbookmarkpersistence) для проверки, можно ли безопасно вызов `SetBookmark`.

##  <a name="_core_absolute_positions_in_mfc_odbc"></a> Абсолютное позиционирование в MFC ODBC

Помимо закладок класс `CRecordset` можно задать, указав порядковый номер текущей записи. Это называется абсолютное позиционирование.

> [!NOTE]
>  Абсолютное позиционирование недоступна на последовательным. Дополнительные сведения о последовательным доступом, см. в разделе [записей (ODBC)](../../data/odbc/recordset-odbc.md).

Чтобы переместить указатель текущей записи, с помощью абсолютное положение, вызовите [CRecordset::SetAbsolutePosition](../../mfc/reference/crecordset-class.md#setabsoluteposition). При передаче значение `SetAbsolutePosition`, запись, соответствующая, порядковый номер становится текущей записи.

> [!NOTE]
>  Абсолютное положение записи потенциально ненадежным. Если пользователь удаляет записи из набора записей, изменяет порядковый номер всех последующих записей. Закладки-это рекомендуемый метод для перемещения текущей записи. Дополнительные сведения см. в разделе [закладки в MFC ODBC](#_core_bookmarks_in_mfc_odbc).

Дополнительные сведения о перемещении по набору записей, см. в разделе [набор записей: прокрутка (ODBC)](../../data/odbc/recordset-scrolling-odbc.md).

## <a name="see-also"></a>См. также

[Набор записей (ODBC)](../../data/odbc/recordset-odbc.md)