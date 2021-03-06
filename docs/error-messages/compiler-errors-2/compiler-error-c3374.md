---
title: Ошибка компилятора C3374 | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-diagnostics
ms.topic: error-reference
f1_keywords:
- C3374
dev_langs:
- C++
helpviewer_keywords:
- C3374
ms.assetid: 41431299-bd20-47d4-a0c8-1334dd79018b
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 1c4fce4e39dac7342e8d564c0adc7537a856c05d
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46104898"
---
# <a name="compiler-error-c3374"></a>Ошибка компилятора C3374

невозможно взять адрес 'функции' без создания экземпляра делегата

Адрес функции был взят в контексте, отличном от создания экземпляра делегата.

Следующий пример приводит к возникновению ошибки C3374:

```
// C3374.cpp
// compile with: /clr
public delegate void MyDel(int i);

ref class A {
public:
   void func1(int i) {
      System::Console::WriteLine("in func1 {0}", i);
   }
};

int main() {
   &A::func1;   // C3374

   // OK
   A ^ a = gcnew A;
   MyDel ^ StaticDelInst = gcnew MyDel(a, &A::func1);
}
```

## <a name="see-also"></a>См. также

[Практическое руководство. Определение и использование делегатов (C++/CLI)](../../dotnet/how-to-define-and-use-delegates-cpp-cli.md)