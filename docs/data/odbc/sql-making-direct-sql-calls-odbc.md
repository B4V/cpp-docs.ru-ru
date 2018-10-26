---
title: 'SQL: Выполнение прямых вызовов SQL (ODBC) | Документация Майкрософт'
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-data
ms.topic: conceptual
dev_langs:
- C++
helpviewer_keywords:
- SQL, direct calls from ODBC
- SQL, calling directly from ODBC
- ODBC, SQL calls
- SQL calls
- direct SQL calls from ODBC
ms.assetid: 091988d2-f5a5-4c2d-aa09-8779a9fb9607
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
- data-storage
ms.openlocfilehash: 2201a8936c1f28221bfcb628139a979e042715b9
ms.sourcegitcommit: a9dcbcc85b4c28eed280d8e451c494a00d8c4c25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2018
ms.locfileid: "50079224"
---
# <a name="sql-making-direct-sql-calls-odbc"></a>SQL. Выполнение прямых вызовов SQL (ODBC)

Содержание раздела:

- Когда следует использовать прямые SQL вызывает.

- [Порядок выполнения прямого SQL вызывает к источнику данных](#_core_making_direct_sql_function_calls).

> [!NOTE]
>  Эти сведения относятся к классам ODBC библиотеки MFC. Если вы работаете с классами MFC DAO, см. в разделе «Сравнения Microsoft Jet базы данных ядра SQL и ANSI SQL» в справке DAO.

##  <a name="_core_when_to_call_sql_directly"></a> Когда для непосредственного вызова SQL

Для создания новых таблиц, удаление (delete) таблиц, изменить существующие таблицы, создание индексов и выполнять другие функции SQL, которые изменяют [источника данных (ODBC)](../../data/odbc/data-source-odbc.md) схемы, необходимо выполнить инструкцию SQL непосредственно для источника данных, с помощью базы данных Определение языка DDL. При использовании мастера для создания набора записей для таблицы (во время разработки), можно выбрать, какие столбцы таблицы для представления в наборе записей. Это свойство не допускает для столбцов, которые вы или другой пользователь источника данных, добавить в таблицу позже, после компиляции программы. Классы баз данных не поддерживают DDL напрямую, но по-прежнему можно написать код для привязки нового столбца к набору записей динамически, во время выполнения. Сведения о том, как сделать этой привязки, см. в разделе [набор записей: динамическая привязка столбцов данных (ODBC)](../../data/odbc/recordset-dynamically-binding-data-columns-odbc.md).

Саму СУБД можно использовать для изменения схемы или другое средство, которое позволяет выполнять функции DDL. Вызовы функций ODBC также можно использовать для отправки инструкций SQL, например вызов предопределенного запроса (хранимой процедуры), которая не возвращает записей.

##  <a name="_core_making_direct_sql_function_calls"></a> Выполнение прямых вызовов SQL-функция

Чтобы выполнить прямой вызов SQL с помощью [класс CDatabase](../../mfc/reference/cdatabase-class.md) объекта. Настроить строку инструкции SQL (обычно в `CString`) и передать его в [помощью функции CDatabase::ExecuteSQL](../../mfc/reference/cdatabase-class.md#executesql) функцию-член вашей `CDatabase` объекта. Если вы используете вызовы функций ODBC для отправки инструкцию SQL, которая обычно возвращает записи, записи учитываются.

## <a name="see-also"></a>См. также

[SQL](../../data/odbc/sql.md)