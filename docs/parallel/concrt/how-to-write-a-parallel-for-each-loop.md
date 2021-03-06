---
title: 'Практическое: написание цикла parallel_for_each | Документация Майкрософт'
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-concrt
ms.topic: conceptual
dev_langs:
- C++
helpviewer_keywords:
- writing a parallel_for_each loop [Concurrency Runtime]
- parallel_for_each function, example
ms.assetid: fa9c0ba6-ace0-4f88-8681-c7c1f52aff20
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 4c68afa77c46e4d57ef01984b44ecb6f4951494a
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46427086"
---
# <a name="how-to-write-a-parallelforeach-loop"></a>Практическое руководство. Написание цикла parallel_for_each

В этом примере показано, как использовать [concurrency::parallel_for_each](reference/concurrency-namespace-functions.md#parallel_for_each) алгоритм для вычисления количества простых чисел в [std::array](../../standard-library/array-class-stl.md) объекта в параллельном режиме.

## <a name="example"></a>Пример

В следующем примере вычисляется количество простых чисел в массиве два раза. В примере сначала используется [std::for_each](../../standard-library/algorithm-functions.md#for_each) алгоритм, для которого вычисляется количество последовательно. Затем в примере используется `parallel_for_each` алгоритм для выполнения той же задачи в параллельном режиме. В этом примере в консоль также выводится время, необходимое на выполнение обоих вычислений.

[!code-cpp[concrt-parallel-count-primes#1](../../parallel/concrt/codesnippet/cpp/how-to-write-a-parallel-for-each-loop_1.cpp)]

В следующем примере показаны выходные данные, полученные на четырехпроцессорном компьютере.

```Output
serial version:
found 17984 prime numbers
took 6115 ms

parallel version:
found 17984 prime numbers
took 1653 ms
```

## <a name="compiling-the-code"></a>Компиляция кода

Чтобы скомпилировать код, скопируйте его и затем вставьте его в проект Visual Studio или вставьте его в файл с именем `parallel-count-primes.cpp` и выполните следующую команду в окне командной строки Visual Studio.

**/ EHsc CL.exe parallel-count-primes.cpp**

## <a name="robust-programming"></a>Отказоустойчивость

Лямбда-выражения, в примере передается `parallel_for_each` алгоритм использует `InterlockedIncrement` функция для включения параллельных итераций цикла увеличивается счетчик одновременно. При использовании функции, такие как `InterlockedIncrement` для синхронизации доступа к общим ресурсам, можно представить узкие места производительности в коде. Можно использовать механизм синхронизации без блокировки, например, [concurrency::combinable](../../parallel/concrt/reference/combinable-class.md) класса, чтобы исключить одновременный доступ к общим ресурсам. Пример, использующий `combinable` класса таким образом, см. в разделе [как: использование класса combinable для повышения производительности](../../parallel/concrt/how-to-use-combinable-to-improve-performance.md).

## <a name="see-also"></a>См. также

[Параллельные алгоритмы](../../parallel/concrt/parallel-algorithms.md)<br/>
[Функция parallel_for_each](reference/concurrency-namespace-functions.md#parallel_for_each)

