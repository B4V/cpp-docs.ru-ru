---
title: Предупреждение (уровень 4) C4481 компилятора | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-diagnostics
ms.topic: error-reference
f1_keywords:
- C4481
dev_langs:
- C++
helpviewer_keywords:
- C4481
ms.assetid: 7bfd4e0c-b452-4e6c-b7c4-ac5cc93fe4ea
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 48ed2ba08423f7540f4e0a855aacbcab993d41aa
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46063766"
---
# <a name="compiler-warning-level-4-c4481"></a>Предупреждение компилятора (уровень 1) C4481

использовано нестандартное расширение: спецификатор переопределения «ключевое слово»

Ключевое слово использовался, не находится в стандарт языка C++, например, один из спецификаторов переопределения, которые также могут использоваться в/CLR.  Дополнительные сведения см. в следующих разделах:

- [/clr (компиляция среды выполнения)](../../build/reference/clr-common-language-runtime-compilation.md)

- [Спецификаторы переопределения](../../windows/override-specifiers-cpp-component-extensions.md)

## <a name="example"></a>Пример

Следующий пример приводит к возникновению ошибки C4481.

```
// C4481.cpp
// compile with: /W4 /c
class B {
   virtual void f(unsigned);
};

class C : B {
   void f(unsigned) override;   // C4481
   void f2(unsigned);
};
```