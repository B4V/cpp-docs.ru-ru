---
title: Предупреждение (уровень 1) C4945 компилятора | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-diagnostics
ms.topic: error-reference
f1_keywords:
- C4945
dev_langs:
- C++
helpviewer_keywords:
- C4945
ms.assetid: 6d2079ea-dc59-4611-bc68-9a22c06f7587
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 48797667c880bcd441065da3651adabdb955b52b
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46027523"
---
# <a name="compiler-warning-level-1-c4945"></a>Предупреждение компилятора (уровень level 1) C4945

«символ»: не удается импортировать символ из «сборка2»: «символ» уже был импортирован из другой сборки «сборка1»

Символ был импортирован в указанной сборке, но этот символ уже был импортирован из другой сборки, на которую указывает ссылка. Не ссылаться на одной из сборок, или имя символа, изменения в одной из сборок.

Приведенные ниже примеры создают C4945.

```
// C4945a.cs
// compile with: /target:library
// C# source code to create a dll
public class ClassA {
   public int i;
}
```

И потом

```
// C4945b.cs
// compile with: /target:library
// C# source code to create a dll
public class ClassA {
   public int i;
}
```

И потом

```
// C4945c.cpp
// compile with: /clr /LD /W1
#using "C4945a.dll"
#using "C4945b.dll"   // C4945
```