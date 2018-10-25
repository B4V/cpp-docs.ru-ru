---
title: Доступ к ODBC и SQL | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-data
ms.topic: conceptual
dev_langs:
- C++
helpviewer_keywords:
- API calls [C++], calling DAO or ODBC directly
- Windows API [C++], calling from MFC
- ODBC API functions [C++]
- ODBC API functions [C++], calling from MFC
- SQL [C++], calling ODBC API functions
- ODBC [C++], API functions
ms.assetid: 5613d7dc-00b7-4646-99ae-1116c05c52b4
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
- data-storage
ms.openlocfilehash: 4635d482a08c486c1cf3259ae642fd82eb4bae82
ms.sourcegitcommit: a9dcbcc85b4c28eed280d8e451c494a00d8c4c25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2018
ms.locfileid: "50055948"
---
# <a name="access-to-odbc-and-sql"></a>Доступ к ODBC и SQL

Библиотеки Microsoft Foundation Class инкапсулирует большого числа вызовов Windows API и по-прежнему позволяет напрямую вызывать любой функции Windows API. Классы баз данных дают такую же гибкость, что и ODBC API. Хотя классы баз данных обходить сложности ODBC, можно вызывать функции ODBC API непосредственно из любого места в программе.

Аналогично, классы баз данных позволит предотвратить работы с [SQL](../../data/odbc/sql.md), но вы можете использовать SQL напрямую, если требуется. Объекты набора записей можно настроить путем передачи пользовательские инструкции SQL (или часть параметров инструкцию по умолчанию) при открытии набора записей. Вы также можете напрямую с помощью вызовов SQL [ExecuteSQL](../../mfc/reference/cdatabase-class.md#executesql) функция-член класса [CDatabase](../../mfc/reference/cdatabase-class.md).

Дополнительные сведения см. в разделе [ODBC: вызов ODBC API функции непосредственно](../../data/odbc/odbc-calling-odbc-api-functions-directly.md) и [SQL: Создание-прямых вызовов SQL (ODBC)](../../data/odbc/sql-making-direct-sql-calls-odbc.md).

## <a name="see-also"></a>См. также

[ODBC и MFC](../../data/odbc/odbc-and-mfc.md)