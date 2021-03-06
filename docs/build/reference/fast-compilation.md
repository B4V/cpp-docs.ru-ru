---
title: Быстрая компиляция | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-tools
ms.topic: reference
dev_langs:
- C++
helpviewer_keywords:
- performance, cle.exe compiler
- compilation, performance
- cl.exe compiler, performance
- fast compiling
ms.assetid: 5fead136-ba69-40c8-8e25-236f89d5990a
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 926c63d3d556d1aa9b85a7ce97e93b60e7c2ea23
ms.sourcegitcommit: 92f2fff4ce77387b57a4546de1bd4bd464fb51b6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/17/2018
ms.locfileid: "45722272"
---
# <a name="fast-compilation"></a>Быстрая компиляция

Для увеличения скорости компиляции:

- Используйте [минимальное перестроение](../../build/reference/gm-enable-minimal-rebuild.md), в которой компилятор C++ повторно компилирует исходный файл только в том случае, если он зависит от изменения класса в файле заголовка.

- [Создание файлов предкомпилированных заголовков](../../build/reference/creating-precompiled-header-files.md) и использовать [предкомпилированный заголовок параметры](../../build/reference/yc-create-precompiled-header-file.md).

## <a name="see-also"></a>См. также

[Параметры компилятора](../../build/reference/compiler-options.md)<br/>
[Настройка параметров компилятора](../../build/reference/setting-compiler-options.md)