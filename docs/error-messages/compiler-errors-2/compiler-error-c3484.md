---
title: Ошибка компилятора C3484 | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-diagnostics
ms.topic: error-reference
f1_keywords:
- C3484
dev_langs:
- C++
helpviewer_keywords:
- C3484
ms.assetid: 2fe847fa-f6ee-4978-bc1d-b6dc6ae906ac
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 19a79574f85d05c6b1ac32416509ba1f8c05e26b
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46019190"
---
# <a name="compiler-error-c3484"></a>Ошибка компилятора C3484

требуется "->" перед типом возврата

Необходимо указать `->` перед типом возврата лямбда-выражения.

### <a name="to-correct-this-error"></a>Исправление ошибки

- Укажите `->` перед типом возврата.

## <a name="example"></a>Пример

В следующем примере возникает ошибка C3484:

```
// C3484a.cpp

int main()
{
   return []() . int { return 42; }(); // C3484
}
```

## <a name="example"></a>Пример

В следующем примере устраняется ошибка C3484 путем предоставления `->` перед типом возврата лямбда-выражения:

```
// C3484b.cpp

int main()
{
   return []() -> int { return 42; }();
}
```

## <a name="see-also"></a>См. также

[Лямбда-выражения](../../cpp/lambda-expressions-in-cpp.md)