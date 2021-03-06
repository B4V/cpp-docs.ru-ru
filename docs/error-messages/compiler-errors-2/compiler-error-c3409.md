---
title: Ошибка компилятора C3409 | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-diagnostics
ms.topic: error-reference
f1_keywords:
- C3409
dev_langs:
- C++
helpviewer_keywords:
- C3409
ms.assetid: e372d9fa-230c-4b28-b6d3-6ad81ccf9dbb
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 338a98adb45ee9fc8eb392853a5693d10a171940
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46058839"
---
# <a name="compiler-error-c3409"></a>Ошибка компилятора C3409

пустой блок атрибута не допускается

Квадратные скобки интерпретировал компилятора как [атрибут](../../windows/cpp-attributes-reference.md) блок, но атрибуты не найдены.

Компилятор может создать эту ошибку, при использовании квадратных скобок как часть определения лямбда-выражения. Эта ошибка возникает, когда компилятор не может определить, являются ли квадратные скобки частью определения лямбда-выражения или блока атрибута. Дополнительные сведения о лямбда-выражениях см. в разделе [Лямбда-выражения](../../cpp/lambda-expressions-in-cpp.md).

### <a name="to-correct-this-error"></a>Исправление ошибки

1. Если квадратные скобки являются частью блок атрибутов:

   1. Укажите один или несколько атрибутов в блоке атрибутов.

   1. Удалите блок атрибутов.

1. Если квадратные скобки являются частью лямбда-выражения:

   1. Убедитесь, что лямбда-выражение имеет правила синтаксиса.

         Дополнительные сведения о синтаксисе лямбда-выражений, см. в разделе [синтаксис лямбда-выражений](../../cpp/lambda-expression-syntax.md).

    2.

## <a name="example"></a>Пример

Следующий пример приводит к возникновению ошибки C3409.

```
// C3409.cpp
// compile with: /c
#include <windows.h>
[]   // C3409
class a {};

// OK
[object, uuid("00000000-0000-0000-0000-000000000000")]
__interface x {};

[coclass, uuid("00000000-0000-0000-0000-000000000001")]
class b : public x {};
```

## <a name="example"></a>Пример

В следующем примере возникает C3409, так как лямбда-выражение использует `mutable` спецификации, но не предоставляет список параметров. Компилятор не может определить, являются ли квадратные скобки частью определения лямбда-выражение или блок атрибутов.

```
// C3409b.cpp

int main()
{
   [] mutable {}();
}
```

## <a name="see-also"></a>См. также

[attribute](../../windows/cpp-attributes-reference.md)<br/>
[Лямбда-выражения](../../cpp/lambda-expressions-in-cpp.md)<br/>
[Синтаксис лямбда-выражений](../../cpp/lambda-expression-syntax.md)