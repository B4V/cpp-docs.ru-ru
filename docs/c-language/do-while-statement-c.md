---
title: Оператор do-while в С | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-language
ms.topic: language-reference
f1_keywords:
- do
- while
dev_langs:
- C++
helpviewer_keywords:
- do-while keyword [C]
ms.assetid: f2ac20a6-10c7-4a08-b5e3-c3b3639dbeaf
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 4b86fa6444889f77b306e4ae543e7d2db41d721b
ms.sourcegitcommit: 997e6b7d336cddb388bb6e9e56527725fcaa0624
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/08/2018
ms.locfileid: "48860684"
---
# <a name="do-while-statement-c"></a>Оператор do-while (C)

Оператор *do-while* позволяет повторять простой или составной оператор, пока указанное выражение не примет значение false.

## <a name="syntax"></a>Синтаксис

*iteration-statement*: &nbsp;&nbsp;&nbsp;&nbsp;**do** *statement*  **while (**  *expression* **) ;**

Выражение *expression* в операторе *do-while* вычисляется после выполнения тела цикла. Поэтому тело цикла всегда выполняется по крайней мере один раз.

Выражение *expression* должно иметь арифметический тип или тип указателя. Выполнение происходит следующим образом:

1. Выполняется тело оператора.

1. Затем вычисляется значение *expression*. Если выражение *expression* имеет значение false, выполнение оператора *do-while* завершается и управление передается следующему оператору программы. Если *expression* имеет значение true (то есть не равно нулю), процесс повторяется с шага 1.

Выполнение оператора *do-while* также может прерваться, если в теле оператора выполняется оператор **break**, **goto** или **return**.

Это пример оператора *do-while*:

```C
do
{
    y = f( x );
    x--;
} while ( x > 0 );
```

В этом операторе *do-while* два оператора `y = f( x );` и `x--;` выполняются независимо от начального значения переменной `x`. Затем вычисляется выражение `x > 0`. Если `x` больше 0, тело оператора выполняется еще раз и снова вычисляется выражение `x > 0`. Тело оператора многократно выполняется, пока значение переменной `x` остается больше 0. Выполнение оператора *do-while* завершается, когда значение переменной `x` становится равным 0 или отрицательным. Тело цикла выполняется по крайней мере один раз.

## <a name="see-also"></a>См. также

[Оператор do-while (C)](../cpp/do-while-statement-cpp.md)
