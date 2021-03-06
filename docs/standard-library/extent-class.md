---
title: Класс extent | Документы Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-standard-libraries
ms.topic: reference
f1_keywords:
- type_traits/std::extent
dev_langs:
- C++
helpviewer_keywords:
- extent class
- extent
ms.assetid: 6d16263d-90b2-4330-9ec7-b59ed898792d
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 156ae11bcc63e5d19b816580bfce7bb24cfbc3d4
ms.sourcegitcommit: 761c5f7c506915f5a62ef3847714f43e9b815352
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2018
ms.locfileid: "44106682"
---
# <a name="extent-class"></a>Класс extent

Получает измерение массива.

## <a name="syntax"></a>Синтаксис

```cpp
template <class Ty, unsigned I = 0>
struct extent;
```

### <a name="parameters"></a>Параметры

*Ty*<br/>
Запрашиваемый тип.

*I*<br/>
Массив, привязанный к запросу.

## <a name="remarks"></a>Примечания

Если *Ty* является типом массива, который имеет по крайней мере *я* измерений, запрос типа содержит число элементов в измерении, заданное *я*. Если *Ty* не является типом массива или его ранг меньше, чем *я*, или если *я* равно нулю и *Ty* имеет тип «массив с неизвестной граница `U` «, запрос типа содержит значение 0.

## <a name="example"></a>Пример

```cpp
// std__type_traits__extent.cpp
// compile with: /EHsc
#include <type_traits>
#include <iostream>

int main()
    {
    std::cout << "extent 0 == "
        << std::extent<int[5][10]>::value << std::endl;
    std::cout << "extent 1 == "
        << std::extent<int[5][10], 1>::value << std::endl;

    return (0);
    }

```

```Output
extent 0 == 5
extent 1 == 10
```

## <a name="requirements"></a>Требования

**Заголовок:** \<type_traits>

**Пространство имен:** std

## <a name="see-also"></a>См. также

[<type_traits>](../standard-library/type-traits.md)<br/>
[Класс remove_all_extents](../standard-library/remove-all-extents-class.md)<br/>
[Класс remove_extent](../standard-library/remove-extent-class.md)<br/>
