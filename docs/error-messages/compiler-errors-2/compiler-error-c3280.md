---
title: Ошибка компилятора C3280 | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-diagnostics
ms.topic: error-reference
f1_keywords:
- C3280
dev_langs:
- C++
helpviewer_keywords:
- C3280
ms.assetid: 86dc5bbc-8818-4786-a728-9334268d308b
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: ed102abc0f46b896b70cb4681db4b0924b6c5822
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46085123"
---
# <a name="compiler-error-c3280"></a>Ошибка компилятора C3280

"класс": функцию-член управляемого типа нельзя скомпилировать как неуправляемую функцию

Функции-члены управляемого типа нельзя компилировать как неуправляемые функции.

Следующий пример приводит к возникновению ошибки C3280:

```
// C3280_2.cpp
// compile with: /clr
ref struct A {
   void func();
};

#pragma managed(push,off)

void A::func()   // C3280
{
}

#pragma managed(pop)
```
