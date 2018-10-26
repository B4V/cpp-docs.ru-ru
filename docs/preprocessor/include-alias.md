---
title: include_alias | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-tools
ms.topic: reference
f1_keywords:
- vc-pragma.include_alias
- include_alias_CPP
dev_langs:
- C++
helpviewer_keywords:
- pragmas, include_alias
- include_alias pragma
ms.assetid: 3256d589-12b3-4af0-a586-199e96eabacc
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: c9844c610a1b5bffab8f5fba67daff90a52412e4
ms.sourcegitcommit: a9dcbcc85b4c28eed280d8e451c494a00d8c4c25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2018
ms.locfileid: "50065178"
---
# <a name="includealias"></a>include_alias

Указывает, что *кратким_именем_файла* будет использоваться в качестве псевдонима для *длинное_имя_файла*.

## <a name="syntax"></a>Синтаксис

> #<a name="pragma-includealiaslongfilename-shortfilename"></a>Директива #pragma include_alias («*длинное_имя_файла*","*кратким_именем_файла*")
> #<a name="pragma-includealiaslongfilename-shortfilename"></a>Директива #pragma include_alias (*длинное_имя_файла*, *кратким_именем_файла*)

## <a name="remarks"></a>Примечания

Некоторые файловые системы поддерживают более длинные имена файлов заголовков, чем допускается ограничением файловой системы FAT (8 символов в имени файла и 3 символа в расширении). Компилятор не может просто усечь более длинные имена до этого стандарта, поскольку первые восемь символов в длинных именах файлов заголовков могут быть неуникальными. Каждый раз, когда компилятор обнаруживает *длинное_имя_файла* строку, он подставляет *кратким_именем_файла*и выполняет поиск файла заголовка *кратким_именем_файла* вместо этого. Эта директива pragma должна располагаться до соответствующей директивы `#include`. Пример:

```cpp
// First eight characters of these two files not unique.
#pragma include_alias( "AppleSystemHeaderQuickdraw.h", "quickdra.h" )
#pragma include_alias( "AppleSystemHeaderFruit.h", "fruit.h" )

#pragma include_alias( "GraphicsMenu.h", "gramenu.h" )

#include "AppleSystemHeaderQuickdraw.h"
#include "AppleSystemHeaderFruit.h"
#include "GraphicsMenu.h"
```

Псевдоним должен точно соответствовать заданному имени как по написанию, так и по регистру. а также по использованию двойных кавычек и угловых скобок. **Include_alias** pragma выполняет сопоставляет строки в имена файлов; проверка имени файла не выполняется. Рассмотрим директивы в следующем примере:

```cpp
#pragma include_alias("mymath.h", "math.h")
#include "./mymath.h"
#include "sys/mymath.h"
```

В этом примере псевдоним не назначается (подстановка не выполняется), поскольку строки файлов заголовков совпадают не полностью. Кроме того, именах файлов заголовков, используемых как аргументы для `/Yu` и `/Yc` параметры компилятора, или `hdrstop` pragma, подстановка не выполняется. Например, представим, что исходный файл содержит следующую директиву:

```cpp
#include <AppleSystemHeaderStop.h>
```

В этом случае должен использоваться следующий параметр компилятора:

> /YcAppleSystemHeaderStop.h

Можно использовать **include_alias** pragma для сопоставления имен файлов заголовка в другой. Пример:

```cpp
#pragma include_alias( "api.h", "c:\version1.0\api.h" )
#pragma include_alias( <stdio.h>, <newstdio.h> )
#include "api.h"
#include <stdio.h>
```

Не смешивайте имена файлов в двойных кавычках с именами файлов, заключенными в угловые скобки. Например, в двух приведенных выше `#pragma include_alias` директивы, компилятор не будет выполнять подстановку для следующих `#include` директивы:

```cpp
#include <api.h>
#include "stdio.h"
```

Кроме того, следующая директива вызовет ошибку:

```cpp
#pragma include_alias(<header.h>, "header.h")  // Error
```

Обратите внимание, что имя файла не сообщали о в сообщениях об ошибках, или в качестве значения из предварительно определенных `__FILE__` макрос, является имя файла, после выполнения подстановки. Например см. в разделе выходных данных после следующие директивы:

```cpp
#pragma include_alias( "VeryLongFileName.H", "myfile.h" )
#include "VeryLongFileName.H"
```

Ошибка в VERYLONGFILENAME. H выдает следующее сообщение об ошибке:

```Output
myfile.h(15) : error C2059 : syntax error
```

Также обратите внимание, что транзитивность не поддерживается. Рассмотрим следующий пример:

```cpp
#pragma include_alias( "one.h", "two.h" )
#pragma include_alias( "two.h", "three.h" )
#include "one.h"
```

В этом случае компилятор будет искать файл TWO.H, а не THREE.H.

## <a name="see-also"></a>См. также

[Директивы Pragma и ключевое слово __Pragma](../preprocessor/pragma-directives-and-the-pragma-keyword.md)