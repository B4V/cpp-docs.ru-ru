---
title: Ошибка компилятора C3005 | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-diagnostics
ms.topic: error-reference
f1_keywords:
- C3005
dev_langs:
- C++
helpviewer_keywords:
- C3005
ms.assetid: 30bad565-e79f-4c3f-82cb-a74bd0baab8f
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: d94d32def0a2fc5ddc3b992d4098a75f925499e7
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46089339"
---
# <a name="compiler-error-c3005"></a>Ошибка компилятора C3005

"текст_ошибки": непредвиденная лексема в директиве OpenMP "директива"

Директива OpenMP сформирована неправильно.

В следующем примере возникает ошибка C3005:

```
// C3005.c
// compile with: /openmp
int main()
{
   #pragma omp parallel + for   // C3005
}
```

Ошибка C3005 также может возникать, если поместить открывающую фигурную скобку в одной строке с директивой pragma.

```
// C3005b.c
// compile with: /openmp
int main() {
   #pragma omp parallel {   // C3005 put open brace on next line
   lbl2:;
   }
   goto lbl2;
}
```