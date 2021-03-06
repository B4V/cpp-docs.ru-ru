---
title: Константы fseek, _lseek | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-standard-libraries
ms.topic: conceptual
f1_keywords:
- SEEK_END
- SEEK_SET
- SEEK_CUR
dev_langs:
- C++
helpviewer_keywords:
- SEEK_SET constant
- SEEK_END constant
- SEEK_CUR constant
ms.assetid: 9deeb13e-5aa3-4c33-80d8-721c80a4de9d
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 3d48ead4532638461962a3bf88d2321cee775ab3
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46087664"
---
# <a name="fseek-lseek-constants"></a>fseek, _lseek Constants

## <a name="syntax"></a>Синтаксис

```

#include <stdio.h>

```

## <a name="remarks"></a>Примечания

Аргумент *origin* определяет исходную позицию и может быть одной из следующих констант манифеста.

|Константа|Значение|
|--------------|-------------|
|`SEEK_END`|Конец файла|
|`SEEK_CUR`|Текущая позиция файлового указателя|
|`SEEK_SET`|Начало файла|

## <a name="see-also"></a>См. также

[fseek, _fseeki64](../c-runtime-library/reference/fseek-fseeki64.md)<br/>
[_lseek, _lseeki64](../c-runtime-library/reference/lseek-lseeki64.md)<br/>
[Глобальные константы](../c-runtime-library/global-constants.md)