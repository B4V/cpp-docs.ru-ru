---
title: Ошибка компилятора C3044 | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-diagnostics
ms.topic: error-reference
f1_keywords:
- C3044
dev_langs:
- C++
helpviewer_keywords:
- C3044
ms.assetid: 9f3e25b2-4676-49ab-97bf-6c88cd0fa377
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 888a899bcc44867b0b586f50f66971d6821d44ec
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46086386"
---
# <a name="compiler-error-c3044"></a>Ошибка компилятора C3044

section: допускается только непосредственное вложение в директиву OpenMP "sections"

Компилятор обнаружил неправильное использование директивы `section` . Дополнительные сведения см. в разделе [sections](../../parallel/openmp/reference/sections-openmp.md).

Следующий пример приводит к возникновению ошибки C3044:

```
// C3044.cpp
// compile with: /openmp /c
#include "omp.h"
int main() {
   int n2 = 2, n3 = 3;

   #pragma omp parallel
   {
      ++n2;

      #pragma omp sections
      {
         ++n2;
      }

      #pragma omp section   // C3044
      {
         ++n3;
      }
   }

   #pragma omp parallel
   {
      ++n2;

      #pragma omp sections
      {
         #pragma omp section   // OK
         {
            ++n3;
         }
      }
   }
}
```