---
title: Класс shuffle_order_engine | Документы Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-standard-libraries
ms.topic: reference
f1_keywords:
- random/std::shuffle_order_engine
- random/std::shuffle_order_engine::base
- random/std::shuffle_order_engine::discard
- random/std::shuffle_order_engine::operator()
- random/std::shuffle_order_engine::base_type
- random/std::shuffle_order_engine::seed
dev_langs:
- C++
helpviewer_keywords:
- std::shuffle_order_engine [C++]
- std::shuffle_order_engine [C++], base
- std::shuffle_order_engine [C++], discard
- std::shuffle_order_engine [C++], base_type
- std::shuffle_order_engine [C++], seed
ms.assetid: 0bcd1fb0-44d7-4e59-bb1b-4a9b673a960d
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 7893f992fa19cdef8713ec4c9fd755c7cd1b465e
ms.sourcegitcommit: 761c5f7c506915f5a62ef3847714f43e9b815352
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2018
ms.locfileid: "44100317"
---
# <a name="shuffleorderengine-class"></a>Класс shuffle_order_engine

Создает случайную последовательность, изменяя порядок значений, возвращенных базовым механизмом.

## <a name="syntax"></a>Синтаксис

```cpp
template <class Engine, size_t K>
class shuffle_order_engine;
```

### <a name="parameters"></a>Параметры

*ядра*<br/>
Тип базового механизма.

*K*<br/>
**Размер таблицы**. Количество элементов в буфере (таблице). **Предварительные условия**: `0 < K`

## <a name="members"></a>Участники

||||
|-|-|-|
|`shuffle_order_engine::shuffle_order_engine`|`shuffle_order_engine::base`|`shuffle_order_engine::discard`|
|`shuffle_order_engine::operator()`|`shuffle_order_engine::base_type`|`shuffle_order_engine::seed`|

Дополнительные сведения о членах механизма см. в разделе [\<random>](../standard-library/random.md).

## <a name="remarks"></a>Примечания

Этот класс шаблона описывает *адаптер механизма*, формирующий значения путем изменения порядка значений, возвращаемых базовым механизмом. Каждый конструктор заполняет внутреннюю таблицу с *K* возвращаются значения базового механизма, а случайный элемент выбирается из таблицы, при запросе значения.

## <a name="requirements"></a>Требования

**Заголовок:** \<random>

**Пространство имен:** std

## <a name="see-also"></a>См. также

[\<random>](../standard-library/random.md)<br/>
