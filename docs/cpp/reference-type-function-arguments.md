---
title: Аргументы функции ссылочного типа | Документация Майкрософт
ms.custom: ''
ms.date: 08/27/2018
ms.technology:
- cpp-language
ms.topic: language-reference
dev_langs:
- C++
helpviewer_keywords:
- arguments [C++], function
- functions [C++], paramters
- function parameters [C++], reference-type
- function arguments [C++], reference-type
- passing parameters [C++], reference-type arguments
ms.assetid: 0a70e831-9e76-46c0-821d-aeba13d73cc0
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 042f609988a87beb8a990405e0426405bc874128
ms.sourcegitcommit: 9a0905c03a73c904014ec9fd3d6e59e4fa7813cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/29/2018
ms.locfileid: "43209755"
---
# <a name="reference-type-function-arguments"></a>Аргументы функции ссылочного типа

Вместо крупных объектов эффективнее бывает передавать функциям ссылки. Это позволяет компилятору передавать адрес объекта, сохраняя при этом синтаксис, который использовался бы для обращения к этому объекту. Рассмотрим следующий пример, в котором используется структура `Date`:

```cpp
// reference_type_function_arguments.cpp
#include <iostream>

struct Date
{
    short Month;
    short Day;
    short Year;
};

// Create a date of the form DDDYYYY (day of year, year)
// from a Date.
long DateOfYear( Date& date )
{
    static int cDaysInMonth[] = {
        31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31
    };
    long dateOfYear = 0;

    // Add in days for months already elapsed.
    for ( int i = 0; i < date.Month - 1; ++i )
        dateOfYear += cDaysInMonth[i];

    // Add in days for this month.
    dateOfYear += date.Day;

    // Check for leap year.
    if ( date.Month > 2 &&
        (( date.Year % 100 != 0 || date.Year % 400 == 0 ) &&
        date.Year % 4 == 0 ))
        dateOfYear++;

    // Add in year.
    dateOfYear *= 10000;
    dateOfYear += date.Year;

    return dateOfYear;
}

int main()
{
    Date date{ 8, 27, 2018 };
    long dateOfYear = DateOfYear(date);
    std::cout << dateOfYear << std::endl;
}
```

Предыдущий код показывает, что членам структуры, передаваемой по ссылке осуществляется с помощью оператора выбора члена (**.**) вместо указатель оператора выбора члена (**->**).

Несмотря на то, что аргументы, передаваемые как ссылочные типы Просмотрите синтаксис типов, не являющихся указателями, они сохраняют одну важную характеристику типов указателя: они являются изменяемыми, если иное не объявлено как **const**. Поскольку задача приведенного выше кода заключается не в том, чтобы изменить объект `date`, более подходящим будет следующий прототип функции:

```cpp
long DateOfYear( const Date& date );
```

Этот прототип гарантирует, что функция `DateOfYear` не изменит его аргумент.

Любая функция, прототипирован как ссылочный тип может принимать объект одного типа на его месте, так как имеется стандартное преобразование из *typename* для *typename* <strong>&</strong>.

## <a name="see-also"></a>См. также

[Ссылки](../cpp/references-cpp.md)<br/>
