---
title: Ошибка компилятора C3100 | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-diagnostics
ms.topic: error-reference
f1_keywords:
- C3100
dev_langs:
- C++
helpviewer_keywords:
- C3100
ms.assetid: 7a9c9eaf-08ef-442d-94a0-e457beee8549
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: f37d21015724bbb66aaa2abf52f0ee2fab7b50a8
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46045358"
---
# <a name="compiler-error-c3100"></a>Ошибка компилятора C3100

«целевой объект»: неизвестный квалификатор атрибута

Указан недопустимый целевой атрибут.

Дополнительные сведения см. в разделе [User-Defined Attributes](../../windows/user-defined-attributes-cpp-component-extensions.md).

## <a name="example"></a>Пример

Следующий пример приводит к возникновению ошибки C3100.

```
// C3100.cpp
// compile with: /clr /c
using namespace System;
[AttributeUsage(AttributeTargets::All)]
public ref class Attr : public Attribute {
public:
   Attr(int t) : m_t(t) {}
   int m_t;
};

[invalid_target:Attr(10)];   // C3100
[assembly:Attr(10)];   // OK
```