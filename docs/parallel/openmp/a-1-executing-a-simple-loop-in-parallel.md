---
title: A.1 параллельное выполнение простого цикла | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-parallel
ms.topic: conceptual
dev_langs:
- C++
ms.assetid: b8aaacae-b20d-4b16-a540-54ccbf09582b
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: b5446f72cc5ee0577385527be24bc912297aec0d
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46418949"
---
# <a name="a1---executing-a-simple-loop-in-parallel"></a>A.1   Параллельное выполнение простого цикла

В следующем примере показано, как для параллельного выполнения простого цикла с помощью `parallel for` директива ([разделе 2.5.1](../../parallel/openmp/2-5-1-parallel-for-construct.md) на странице 16). Переменная итерации цикла является закрытым по умолчанию, поэтому нет необходимости явно указывать в предложения private.

```
#pragma omp parallel for
    for (i=1; i<n; i++)
        b[i] = (a[i] + a[i-1]) / 2.0;
```