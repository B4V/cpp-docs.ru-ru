---
title: Ошибка компилятора C3655 | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-diagnostics
ms.topic: error-reference
f1_keywords:
- C3655
dev_langs:
- C++
helpviewer_keywords:
- C3655
ms.assetid: 724919ab-2915-4b61-8794-44648e162d62
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 2322e2f6393b87e8a26dc0b61f19f8a68065b638
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46118184"
---
# <a name="compiler-error-c3655"></a>Ошибка компилятора C3655

«функция»: функция уже явно переопределена

Функции можно явно переопределяться один раз. Дополнительные сведения см. в разделе [явное переопределение](../../windows/explicit-overrides-cpp-component-extensions.md).

Следующий пример приводит к возникновению ошибки C3655:

```
// C3655.cpp
// compile with: /clr /c
public ref struct B {
   virtual void f();
   virtual void g();
};

public ref struct D : B {
   virtual void f() new sealed = B::f;
   virtual void g() new sealed = B::f;   // C3655
   // try the following line instead
   // virtual void g() new sealed = B::g;
};
```