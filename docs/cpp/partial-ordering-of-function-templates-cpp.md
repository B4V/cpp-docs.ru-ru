---
title: Частичное Упорядочение шаблонов функций (C++) | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-language
ms.topic: language-reference
dev_langs:
- C++
helpviewer_keywords:
- partial ordering of function templates
ms.assetid: 0c17347d-0e80-47ad-b5ac-046462d9dc73
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 048589ecab367a3762764b627de11d72160c4602
ms.sourcegitcommit: 997e6b7d336cddb388bb6e9e56527725fcaa0624
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/08/2018
ms.locfileid: "48861308"
---
# <a name="partial-ordering-of-function-templates-c"></a>Частичное упорядочение шаблонов функций (C++)

Может быть доступно несколько шаблонов функций, соответствующих списку аргументов в вызове функции. В C++ определено частичное упорядочение шаблонов функции, что позволяет указать, какую функцию необходимо вызвать. Упорядочение выполняется частично, поскольку может быть несколько шаблонов, которые считаются в равной мере специализированными.

Компилятор выбирает функцию наиболее специализированного шаблона среди всех возможных совпадений. Например, если шаблон функции принимает тип __T__и создания другого шаблона функции __T\*__  доступен, __T\*__  говорят, что версии более специализированным, поэтому предпочтительнее, чем универсальный __T__ версии каждый раз, когда аргумент имеет тип указателя, несмотря на то, что оба будет представлять собой допустимый совпадения.

Чтобы определить, является ли один кандидатов — шаблонов функций — более специализированным, используйте следующую процедуру:

1. Рассмотрим два шаблона функции, T1 и T2.

1. Замените параметры в шаблоне T1 на гипотетический уникальный тип X.

1. Пользуясь списком параметров из шаблона T1, проверьте, является ли T2 допустимым шаблоном для этого списка параметров. Любые неявные преобразования пропускайте.

1. Повторите ту же самую процедуру, поменяв шаблоны T1 и T2 местами.

1. Если список аргументов из одного шаблона будет допустимым для другого, но не наоборот, то первый шаблон считается менее специализированным, чем второй. Если оба шаблона с помощью предыдущего шага формы допустимые аргументы друг для друга, то они считаются в равной мере специализированными, и результаты неоднозначного вызова при попытке их использования.

1. При проведении процедуры руководствуйтесь следующими правилами:

   1. Шаблон для определенного типа является более специализированным, чем шаблон, принимающий аргумент универсального типа.

   1. Шаблон, используя только __T\*__  является более специализированным, чем один только принимая __T__, так как гипотетический тип __X\*__  является допустимым аргументом для __T__ аргумент шаблона, но __X__ не является допустимым аргументом для __T\*__  аргумент шаблона.

   1. __const T__ является более специализированным, чем __T__, так как __const X__ является допустимым аргументом для __T__ аргумент шаблона, но __X__ — не является допустимым аргументом для __const T__ аргумент шаблона.

   1. __const T\*__  является более специализированным, чем __T\*__, так как __const X\*__  является допустимым аргументом для __T\*__  аргумент шаблона, но __X\*__  не является допустимым аргументом для __const T\*__  аргумент шаблона.

## <a name="example"></a>Пример

Следующий пример работает в том, как указано в стандарте:

```cpp
// partial_ordering_of_function_templates.cpp
// compile with: /EHsc
#include <iostream>

extern "C" int printf(const char*,...);
template <class T> void f(T) {
   printf_s("Less specialized function called\n");
}

template <class T> void f(T*) {
   printf_s("More specialized function called\n");
}

template <class T> void f(const T*) {
   printf_s("Even more specialized function for const T*\n");
}

int main() {
   int i =0;
   const int j = 0;
   int *pi = &i;
   const int *cpi = &j;

   f(i);   // Calls less specialized function.
   f(pi);  // Calls more specialized function.
   f(cpi); // Calls even more specialized function.
   // Without partial ordering, these calls would be ambiguous.
}
```

### <a name="output"></a>Вывод

```Output
Less specialized function called
More specialized function called
Even more specialized function for const T*
```

## <a name="see-also"></a>См. также

[Шаблоны функций](../cpp/function-templates.md)
