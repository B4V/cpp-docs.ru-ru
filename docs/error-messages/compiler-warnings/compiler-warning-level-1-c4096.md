---
title: Предупреждение (уровень 1) C4096 компилятора | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-diagnostics
ms.topic: error-reference
f1_keywords:
- C4096
dev_langs:
- C++
helpviewer_keywords:
- C4096
ms.assetid: abf3cca2-2f21-45d8-b025-6b513b00681e
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 86387103d4d8257a109928a665579621468a3cf3
ms.sourcegitcommit: 955ef0f9d966e7c9c65e040f1e28fa83abe102a5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/04/2018
ms.locfileid: "48788704"
---
# <a name="compiler-warning-level-1-c4096"></a>Компилятор предупреждение (уровень 1) C4096

«»: интерфейс не является COM-интерфейс; он не будет передан в IDL

Определение интерфейса, предназначенное для использования в качестве COM-интерфейс не был определен как COM-интерфейс и поэтому он не будет передан в IDL-файл.

См. в разделе [атрибуты интерфейса](../../windows/attributes/interface-attributes.md) список атрибутов, определяющих интерфейс COM-интерфейса.

Следующий пример приводит к возникновению ошибки C4096:

```
// C4096.cpp
// compile with: /W1 /LD
#include "windows.h"
[module(name="xx")];

// [object, uuid("00000000-0000-0000-0000-000000000001")]
__interface a
{
};

[coclass, uuid("00000000-0000-0000-0000-000000000002")]
struct b : a
{
};   // C4096, remove coclass or uncomment object
```