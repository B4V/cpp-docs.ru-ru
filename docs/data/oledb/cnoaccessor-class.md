---
title: Класс CNoAccessor | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-data
ms.topic: reference
f1_keywords:
- ATL::CNoAccessor
- CNoAccessor
- ATL.CNoAccessor
dev_langs:
- C++
helpviewer_keywords:
- CNoAccessor class
ms.assetid: eb669ae5-0a56-49a3-9646-c4ae6239da31
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
- data-storage
ms.openlocfilehash: 97cfefc679391cb54ff40f38285f22f40d068553
ms.sourcegitcommit: a9dcbcc85b4c28eed280d8e451c494a00d8c4c25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2018
ms.locfileid: "50063839"
---
# <a name="cnoaccessor-class"></a>Класс CNoAccessor

Можно использовать в качестве аргумента шаблона (`TAccessor`) для классов шаблонов, таких как `CCommand` и `CTable`, которых требуется аргумент метода доступа класса.

## <a name="syntax"></a>Синтаксис

```cpp
class CNoAccessor
```

## <a name="remarks"></a>Примечания

Используйте `CNoAccessor` как аргумент шаблона, если класс поддерживает параметры или выходные столбцы не нужно.

`CNoAccessor` реализует следующие методы-заглушки, каждый из которых соответствуют другим методам класса метода доступа:

- `BindColumns` -Привязывает столбцы к методы доступа.

- `BindParameters` — Связывает созданный параметры к столбцам.

- `Bind` — Создает привязки.

- `Close` -Закрывает метода доступа.

- `ReleaseAccessors` -Освобождает методы доступа, созданный классом.

- `FreeRecordMemory` -Освобождает все столбцы в текущей записи, которые следует освободиться.

- `GetColumnInfo` — Возвращает сведения о столбцах из открытого набора строк.

- `GetNumAccessors` — Извлекает число методов доступа, созданный классом.

- `IsAutoAccessor` — Возвращает значение true, если данные извлекаются автоматически для метода доступа во время операции перемещения.

- `GetHAccessor` — Извлекает дескриптор метода доступа указанного метода доступа.

- `GetBuffer` — Извлекает указатель на буфер закладки.

- `NoBindOnNullRowset` — Предотвращение привязки данных на пустой набор строк.

## <a name="requirements"></a>Требования

**Заголовок:** atldbcli.h

## <a name="see-also"></a>См. также

[Шаблоны потребителей OLE DB](../../data/oledb/ole-db-consumer-templates-cpp.md)<br/>
[Ссылка на шаблоны объекта-получателя OLE DB](../../data/oledb/ole-db-consumer-templates-reference.md)