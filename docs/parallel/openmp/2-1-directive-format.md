---
title: 2.1 формат директивы | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-parallel
ms.topic: conceptual
dev_langs:
- C++
ms.assetid: 918b6445-d35e-4176-9565-b045be941b4d
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 1b2f2d2f5742dbc4faa1d8386e935c9d4ccc8049
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46424655"
---
# <a name="21-directive-format"></a>2.1 Формат директивы

Синтаксис в директиве OpenMP определяется формально грамматики в [приложении C](../../parallel/openmp/c-openmp-c-and-cpp-grammar.md)и неформально следующим образом:

```
#pragma omp directive-name  [clause[ [,] clause]...] new-line
```

Каждая директива начинается с **#pragma omp**, чтобы уменьшить вероятность возникновения конфликтов с помощью директивы pragma других (отличных от OpenMP или поставщика расширения с OpenMP) с теми же именами. Остальная часть директивы соглашениям стандартов C и C++ для директивы компилятора. В частности, можно использовать пробелы до и после **#**, и иногда необходимо использовать пробелы для разделения слов в директиве. Следующие токены предварительной обработки **#pragma omp** подвержены замены макроса.

Директивы учитывается регистр. Порядок, в котором предложения отображаются в директивы не имеет значения. Предложения для директивы может повторяться, при необходимости, распространяются ограничения, перечисленных в описании каждого предложения. Если *списка переменной* отображается в предложении, его необходимо указать только переменные. Только один *имя директивы* может быть указан для каждой директивы.  Например следующая директива не допускается:

```
/* ERROR - multiple directive names not allowed */
#pragma omp parallel barrier
```

В директиве OpenMP применяется более одной последующие инструкции, который должен быть структурированный блок.