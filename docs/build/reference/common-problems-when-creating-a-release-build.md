---
title: Распространенные проблемы при создании сборки выпуска | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-tools
ms.topic: reference
dev_langs:
- C++
helpviewer_keywords:
- unexpected code generation
- debugging [MFC], release builds
- release builds, troubleshooting
- stray pointers
- debug builds, difference from release builds
- MFC [C++], release builds
- heap layout problems
- pointers, stray
- release builds, building applications
- debug memory allocator
- optimization [C++], compiler
- projects [C++], debug configuration
- troubleshooting Visual C++
- troubleshooting release builds
- memory [C++], overwrites
ms.assetid: 73cbc1f9-3e33-472d-9880-39a8e9977b95
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: b423f173bfa2d7fdc3fd8e97fe9eb42cf8e76f3d
ms.sourcegitcommit: 92f2fff4ce77387b57a4546de1bd4bd464fb51b6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/17/2018
ms.locfileid: "45702459"
---
# <a name="common-problems-when-creating-a-release-build"></a>Распространенные проблемы, возникающие при создании построений выпуска

Во время разработки обычно построение и тестирование с помощью отладочной сборки проекта. При построении приложения для сборки выпуска может появиться сообщение о нарушении прав доступа.

Ниже перечислены основные различия между отладочной и сборки выпуска (отладки). Существуют другие различия, но ниже приведены основные различия, которые могут привести к сбою приложения в сборке выпуска, когда оно работает в отладочной сборке.

- [Размещение в куче](#_core_heap_layout)

- [Компиляция](#_core_compilation)

- [Поддержка указателей](#_core_pointer_support)

- [Оптимизация](#_core_optimizations)

См. в разделе [/GZ (перехват ошибок построения выпуска в отладочное построение)](../../build/reference/gz-enable-stack-frame-run-time-error-checking.md) Дополнительные сведения о том, как перехватить выпуска ошибки сборки в отладочных сборках.

##  <a name="_core_heap_layout"></a> Размещение в куче

Макет кучи будет причиной около 90% компаний проблем приложения, работающего в отладки, но не выпуск.

При построении проекта для отладки используется механизм распределения отладочной памяти. Это означает, что всех операций выделения памяти байты guard. Эти защитных байтов для обнаружения перезаписи памяти. Поскольку макет кучи отличается между отладочной и окончательной версиях перезаписи памяти не может создать проблемы в сборке отладки, но может иметь последствия катастрофической в окончательной сборке.

Дополнительные сведения см. в разделе [проверки перезаписи памяти](../../build/reference/checking-for-memory-overwrites.md) и [использования отладка сборки для проверки перезаписи памяти](../../build/reference/using-the-debug-build-to-check-for-memory-overwrite.md).

##  <a name="_core_compilation"></a> Компиляция

Многие из макросов MFC и изменении реализации MFC при создании для выпуска. В частности макрос ASSERT имеет значение nothing в сборке выпуска, поэтому код, содержащийся в будет выполняться. Дополнительные сведения см. в разделе [изучить инструкции ASSERT](../../build/reference/using-verify-instead-of-assert.md).

Некоторые функции являются встроенными в целях повышения производительности в окончательной сборке. Оптимизация обычно включаются в сборку выпуска. Также используется другой механизм распределения памяти.

##  <a name="_core_pointer_support"></a> Поддержка указателей

Отсутствие отладочной информации, удаляет заполнение из приложения. В сборке выпуска свободные указатели имеют больше шансов на неинициализированной памяти, а не к отладочной информации.

##  <a name="_core_optimizations"></a> Оптимизация

В зависимости от характера определенные сегменты кода оптимизирующий компилятор может создавать непредвиденный код. Это наименее вероятная причина проблем построения выпуска, но возникают в некоторых случаях. Для решения, см. в разделе [оптимизация кода](../../build/reference/optimizing-your-code.md).

## <a name="see-also"></a>См. также

[Сборки выпуска](../../build/reference/release-builds.md)<br/>
[Устранение проблем сборки выпуска](../../build/reference/fixing-release-build-problems.md)