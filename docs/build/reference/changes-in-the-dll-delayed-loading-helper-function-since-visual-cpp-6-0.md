---
title: Изменения в библиотеке DLL вспомогательной функции отложенной загрузки с Visual C++ 6.0 | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-tools
ms.topic: reference
dev_langs:
- C++
helpviewer_keywords:
- delayed loading of DLLs, what's changed
- PFromRva method
- __delayLoadHelper2 function
- helper functions, what's changed
ms.assetid: 99f0be69-105d-49ba-8dd5-3be7939c0c72
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 0caf74f02b005ef65e8ac30750fdf244ddeeed0d
ms.sourcegitcommit: 92f2fff4ce77387b57a4546de1bd4bd464fb51b6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/17/2018
ms.locfileid: "45712274"
---
# <a name="changes-in-the-dll-delayed-loading-helper-function-since-visual-c-60"></a>Изменения вспомогательной функции отложенной загрузки библиотек DLL по сравнению с Visual C++ версии 6.0

Если у вас есть несколько версий Visual C++ на компьютере, или если вы определили собственной вспомогательной функции, вам могут влиять изменения, внесенные в библиотеки DLL вспомогательной функции отложенной загрузки. Пример:

- **__delayLoadHelper** теперь **__delayLoadHelper2**

- **__pfnDliNotifyHook** теперь **__pfnDliNotifyHook2**

- **__pfnDliFailureHook** теперь **__pfnDliFailureHook2**

- **__FUnloadDelayLoadedDLL** теперь **__FUnloadDelayLoadedDLL2**

> [!NOTE]
>  Если вы используете вспомогательную функцию по умолчанию, эти изменения не отразятся на вас. Нет изменений по каким образом вызывать компоновщик.

## <a name="multiple-versions-of-visual-c"></a>Несколько версий Visual C++

Если у вас есть несколько версий Visual C++ на компьютере, убедитесь, что компоновщик совпадает с библиотекой delayimp.lib. Если существует несоответствие, отобразится ошибка компоновщика отчетов либо `___delayLoadHelper2@8` или `___delayLoadHelper@8` как неразрешенном внешнем символе. Первое означает новый компоновщика со старой библиотекой delayimp.lib, а второе означает, что старый компоновщик с новой библиотекой delayimp.lib.

Если возникнет Неустранимая ошибка компоновщика, запустите [dumpbin/LINKERMEMBER](../../build/reference/linkermember.md): 1 на библиотекой delayimp.lib, которая должна содержать вспомогательную функцию, чтобы узнать, какие вспомогательную функцию вместо определен. Вспомогательная функция также можно определить в объектный файл; Запустите [dumpbin/Symbols](../../build/reference/symbols.md) и найдите `delayLoadHelper(2)`.

Если вы знаете, что у вас есть компоновщик Visual C++ 6.0, затем:

- (Программа DUMPBIN) под управлением файла LIB или OBJ вспомогательных нагрузки задержки, чтобы определить, является ли он определяет **__delayLoadHelper2**. В противном случае такая компоновка завершается ошибкой.

- Определение **__delayLoadHelper** возможную задержку, которая загрузки файла LIB или OBJ вспомогательного приложения.

## <a name="user-defined-helper-function"></a>Определяемые пользователем вспомогательной функции

Если определен собственной вспомогательной функции и при использовании текущей версии Visual C++, сделайте следующее:

- Переименовать вспомогательную функцию для **__delayLoadHelper2**.

- Так как на относительные адреса (RVA), работают в обеих программ 32 - и 64-разрядные указатели дескриптора задержки (ImgDelayDescr в delayimp.h) из абсолютных адресов (VAs) были изменены, необходимо преобразовать их обратно в указатели. Представлена новая функция: PFromRva, найден в delayhlp.cpp. Можно использовать эту функцию на каждом из полей дескриптора для преобразования их либо 32 - или 64-разрядные указатели. Вспомогательную функцию отложенной загрузки по умолчанию по-прежнему можно использовать в качестве примера.

## <a name="load-all-imports-for-a-delay-loaded-dll"></a>Загрузка всех импортов для библиотеки DLL с отложенной загрузкой

Компоновщик может загружать все импорты из библиотеки DLL, созданную с отложенной загрузкой. См. в разделе [загрузка всех импортов для библиотеки DLL Delay-Loaded](../../build/reference/loading-all-imports-for-a-delay-loaded-dll.md) Дополнительные сведения.

## <a name="see-also"></a>См. также

[Понятие вспомогательной функции](understanding-the-helper-function.md)