---
title: Поддержка библиотек для смешанных сборок | Документация Майкрософт
ms.custom: ''
ms.date: 09/18/2018
ms.technology:
- cpp-cli
ms.topic: conceptual
dev_langs:
- C++
helpviewer_keywords:
- msvcm90[d].dll
- mixed assemblies [C++], library support
- msvcmrt[d].lib
- libraries [C++], mixed assemblies
ms.assetid: 1229595c-9e9d-414d-b018-b4e4c727576d
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
- dotnet
ms.openlocfilehash: 8c3fec26f3e41c3edd2346ac2e1b9b1f6b98ba33
ms.sourcegitcommit: a9dcbcc85b4c28eed280d8e451c494a00d8c4c25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2018
ms.locfileid: "50069624"
---
# <a name="library-support-for-mixed-assemblies"></a>Поддержка библиотек для смешанных сборок

Visual C++ поддерживает использование стандартной библиотеки C++, библиотеку времени выполнения C (CRT), ATL и MFC в приложениях, скомпилированных с [/CLR (компиляция CLR)](../build/reference/clr-common-language-runtime-compilation.md). Благодаря этому существующие приложения, использующие эти библиотеки для использования возможностей .NET Framework также.

> [!IMPORTANT]
> **/CLR: pure** и **/CLR: safe** параметры компилятора признаны устаревшими в Visual Studio 2015 и не поддерживается в Visual Studio 2017.

Эта поддержка включает следующие библиотеки DLL и импорта:

- .Lib msvcmrt [d] при компиляции с параметром **/CLR**. Смешанные сборки ссылку на эту библиотеку импорта.

Эта поддержка обеспечивает некоторые дополнительные преимущества:

- CRT и стандартной библиотеки C++ доступны для смешанного кода. CRT и стандартной библиотеки C++ предоставляются не подлежат проверке; в конечном счете вызовы по-прежнему направляются на один и тот же CRT и стандартной библиотеки C++, что вы используете из машинного кода.

- Правильная унифицированная обработка исключений в смешанных образов.

- Статическая инициализация переменных C++ в смешанном образов.

- Поддержка переменных на уровне домена приложения и каждого процесса в управляемом коде.

- Устраняет проблемы блокировки загрузчика, которые применены к смешанные библиотеки DLL, скомпилированные в Visual Studio 2003 и более ранних версий.

Кроме того эта поддержка действуют следующие ограничения:

- Поддерживается только модель CRT DLL, для кода, компилируемого с **/CLR**. Нет статических библиотек CRT, которые поддерживают **/CLR** сборки.

## <a name="see-also"></a>См. также

- [Смешанные (собственные и управляемые) сборки](../dotnet/mixed-native-and-managed-assemblies.md)
