---
title: Ошибка компилятора C3008 | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-diagnostics
ms.topic: error-reference
f1_keywords:
- C3008
dev_langs:
- C++
helpviewer_keywords:
- C3008
ms.assetid: 04d93201-28e5-4be0-945c-aad616376f4b
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: af4a7c5cf4cf80595be0b21f3313dab1cf20acb2
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46027249"
---
# <a name="compiler-error-c3008"></a>Ошибка компилятора C3008

"аргумент": в аргументе директивы OpenMP "директива" отсутствует закрывающая скобка ")"

Директива OpenMP, которая принимает аргумент, не содержит закрывающую скобку.

При компиляции следующего примера возникнет ошибка C3008:

```
// C3008.c
// compile with: /openmp
int main()
{
   int x, y, z;
   #pragma omp parallel shared(x   // C3008
   // Try the following line instead:
   #pragma omp parallel shared(x)
   {
   }
}
```