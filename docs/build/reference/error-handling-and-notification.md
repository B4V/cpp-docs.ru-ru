---
title: Обработка ошибок и предупреждений | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-tools
ms.topic: reference
dev_langs:
- C++
helpviewer_keywords:
- error handling, and notification
ms.assetid: b621cf60-d869-451a-b05e-dc86d78addaa
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 17df0dfd57bf24c7cd442c296409530e521b28de
ms.sourcegitcommit: 92f2fff4ce77387b57a4546de1bd4bd464fb51b6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/17/2018
ms.locfileid: "45723207"
---
# <a name="error-handling-and-notification"></a>Обработка ошибок и предупреждений

Дополнительные сведения о обработка ошибок и предупреждений, см. в разделе [понятие вспомогательной функции](understanding-the-helper-function.md).

Дополнительные сведения о функции-ловушки, см. в разделе [определение структуры и константы](../../build/reference/structure-and-constant-definitions.md).

Если программа использует библиотеки DLL, загружаемых с задержкой, она должна обрабатывать ошибки надежно так, как сбои, возникающие во время работы программы приведет к необработанных исключений. Обработка сбоев состоит из двух частей:

Восстановление ловушки.
Если ваш код должен восстановить или предоставлять альтернативные библиотеки и/или подпрограмму для сбоя, можно указать обработчик для вспомогательной функции, можно предоставить или исправить ситуацию. Процедура обработки требует возврата подходящего значения, таким образом, чтобы обработку можно продолжить (HINSTANCE или FARPROC) или 0, чтобы указать, что должно вызываться исключение. Он также может породить собственное исключение или **longjmp** за пределы ловушки. Существуют обработчики уведомления и обработчики сбоев.

Отчет или исключение.
Если все необходимое для обработки ошибки прекращение процедуры, никаких обработчиков не требуется, поскольку пользовательский код может обработать исключение.

Обработка ошибок и предупреждений, рассматривается в следующих разделах:

- [Обработчики уведомлений](../../build/reference/notification-hooks.md)

- [Обработчики сбоев](../../build/reference/failure-hooks.md)

- [Исключения](../../build/reference/exceptions-c-cpp.md)

## <a name="see-also"></a>См. также

[Поддержка компоновщика для библиотек DLL с отложенной загрузкой](../../build/reference/linker-support-for-delay-loaded-dlls.md)