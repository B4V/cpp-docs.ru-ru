---
title: Комментарии в файле Makefile | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-tools
ms.topic: conceptual
dev_langs:
- C++
helpviewer_keywords:
- makefiles, comments
ms.assetid: 76fd9e3d-5966-47f4-a091-c9e80b232b49
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 0bff732a0e9becc9b6c829c70a1bc6701e6031bf
ms.sourcegitcommit: 92f2fff4ce77387b57a4546de1bd4bd464fb51b6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/17/2018
ms.locfileid: "45723961"
---
# <a name="comments-in-a-makefile"></a>Комментарии в файлах makefile

Перед комментарий со знака номера (#). NMAKE игнорирует текст из решетки на следующий символ новой строки. Примеры

```
# Comment on line by itself
OPTIONS = /MAP  # Comment on macro definition line

all.exe : one.obj two.obj  # Comment on dependency line
    link one.obj two.obj
# Comment in commands block
#   copy *.obj \objects  # Command turned into comment
    copy one.exe \release

.obj.exe:  # Comment on inference rule line
    link $<

my.exe : my.obj ; link my.obj  # Err: cannot comment this
# Error: # must be the first character
.obj.exe: ; link $<  # Error: cannot comment this
```

Чтобы указать литерал решетки, укажите перед ним знак крышки (**^**), как показано ниже:

```
DEF = ^#define  #Macro for a C preprocessing directive
```

## <a name="see-also"></a>См. также

[Содержимое файла Makefile](../build/contents-of-a-makefile.md)