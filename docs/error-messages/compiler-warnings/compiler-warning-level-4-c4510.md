---
title: Предупреждение компилятора (уровень 4) C4510 | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-diagnostics
ms.topic: error-reference
f1_keywords:
- C4510
dev_langs:
- C++
helpviewer_keywords:
- C4510
ms.assetid: fd28d1d4-ad27-4dad-94c0-9dba46c93180
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: f2aaf7286c2e900629a18d7df5824ef4b7af1f5f
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46048972"
---
# <a name="compiler-warning-level-4-c4510"></a>Предупреждение компилятора (уровень 4) C4510

«класс»: не удалось создать конструктор по умолчанию

Компилятор не может создать конструктор по умолчанию для заданного класса и был создан без определенного пользователем конструктора. Вы не сможете создавать объекты этого типа.

Существует несколько ситуаций, в которых компилятор по умолчанию конструктор, включая:

- Константный член данных.

- Элемент данных, который является ссылкой.

Вам нужно создать конструктор по умолчанию, определяемые пользователем для класса, который инициализирует эти члены.

Следующий пример приводит к возникновению ошибки C4510:

```
// C4510.cpp
// compile with: /W4
struct A {
   const int i;
   int &j;
   A& operator=( const A& ); // C4510 expected
   // uncomment the following line to resolve this C4510
   // A(int ii, int &jj) : i(ii), j(jj) {}
};   // C4510

int main() {
}
```