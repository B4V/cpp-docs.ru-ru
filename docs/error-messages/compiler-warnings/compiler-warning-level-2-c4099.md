---
title: Предупреждение компилятора (уровень 2) C4099 | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-diagnostics
ms.topic: error-reference
f1_keywords:
- C4099
dev_langs:
- C++
helpviewer_keywords:
- C4099
ms.assetid: 00bb803d-cae7-4ab8-8969-b46f54139ac8
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 2d7ffee02e8e5414a0e06cc4ba0da77a50c75f53
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46110176"
---
# <a name="compiler-warning-level-2-c4099"></a>Предупреждение компилятора (уровень 2) C4099

«Идентификатор»: имя типа, ранее отображенное с помощью objecttype1 теперь увидеть при помощи «objecttype2»

Объект, объявленный как структура определяется как класс или объект объявлен как класс, определенный как структура. Компилятор использует тип, заданный в определении.

## <a name="example"></a>Пример

Следующий пример приводит к возникновению ошибки C4099.

```
// C4099.cpp
// compile with: /W2 /c
struct A;
class A {};   // C4099, use different identifer or use same object type
```