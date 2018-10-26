---
title: Класс tuple_size | Документы Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-standard-libraries
ms.topic: reference
f1_keywords:
- tuple_size
- std::tuple_size
- utility/std::tuple_size
dev_langs:
- C++
helpviewer_keywords:
- std::tuple_size
ms.assetid: 73852fc5-eb68-41f1-8379-465cedc2314a
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 4169532a6aff64d24bdff59debcb675a35d72f06
ms.sourcegitcommit: 1d9bd38cacbc783fccd3884b7b92062161c91c84
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/03/2018
ms.locfileid: "48233610"
---
# <a name="tuplesize-class"></a>Класс tuple_size

Передает число элементов, содержащихся в кортеже `tuple` .

## <a name="syntax"></a>Синтаксис

```cpp
// TEMPLATE STRUCT tuple_size
template <class Tuple>
   struct tuple_size;

// number of elements in array
template <class Elem, size_t Size>
   struct tuple_size<array<Elem, Size>>
      : integral_constant<size_t, Size>;

// size of pair
template <class T1, class T2>
   struct tuple_size<pair<T1, T2>>
      : integral_constant<size_t, 2>

// size of tuple
template <class... Types>
   struct tuple_size<tuple<Types...>>
      : integral_constant<size_t, sizeof...(Types)>;

// size of const tuple
template <class Tuple>
   struct tuple_size<const Tuple>;

// size of volatile tuple
template <class Tuple>
   struct tuple_size<volatile Tuple>;

// size of const volatile tuple
template <class Tuple>
   struct tuple_size<const volatile Tuple>;
```

### <a name="parameters"></a>Параметры

*Tuple*<br/>
Тип кортежа.

*Elem*<br/>
Тип элементов массива.

*Size*<br/>
Размер массива.

*T1*<br/>
Тип первого элемента пары.

*T2*<br/>
Тип второго элемента пары.

*Типы*<br/>
Типы элементов кортежа.

## <a name="remarks"></a>Примечания

Класс шаблонов имеет член `value` , представляет собой интегральное константное выражение, значение которого равно степени тип кортежа *кортежа*.

В специализации шаблона для массивов есть член `value` , представляет собой интегральное константное выражение, значение которого равно *размер*, равным размеру массива.

В специализации шаблона для пар есть член `value`, который представляет собой интегральное константное выражение со значением 2.

## <a name="example"></a>Пример

```cpp
#include <tuple>
#include <iostream>

using namespace std;

typedef tuple<int, double, int, double> MyTuple;
int main()
{
    MyTuple c0(0, 1.5, 2, 3.7);

    // display contents "0 1 2 3"
    cout << get<0>(c0);
    cout << " " << get<1>(c0);
    cout << " " << get<2>(c0);
    cout << " " << get<3>(c0) << endl;

    // display size "4"
    cout << " " << tuple_size<MyTuple>::value << endl;
}
```

```Output
0 1.5 2 3.7
4
```

## <a name="requirements"></a>Требования

**Заголовок:** \<tuple>

**Заголовок:** \<array> (для специализации массива)

**Заголовок:** \<utility> (для специализации пары)

**Пространство имен:** std

## <a name="see-also"></a>См. также

[\<tuple>](../standard-library/tuple.md)<br/>
[tuple](../standard-library/tuple-class.md)<br/>
[Класс tuple_element](../standard-library/tuple-element-class-tuple.md)<br/>
