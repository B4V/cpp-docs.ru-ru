---
title: Предупреждение компилятора (уровень 1) C4182 | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-diagnostics
ms.topic: error-reference
f1_keywords:
- C4182
dev_langs:
- C++
helpviewer_keywords:
- C4182
ms.assetid: 8970f3c6-e2dd-407e-b2ec-964360eb8b43
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 80c0cdac45238a4734b02d34f4c540c62a2f0c09
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46056577"
---
# <a name="compiler-warning-level-1-c4182"></a>Предупреждение компилятора (уровень 1) C4182

\#включать уровень вложенности составляет «число»; возможна бесконечная рекурсия

Компилятору недостаточно места в куче из-за количества вложенных файлов include. Файл include является вложенным, когда он включается из другого файла include.

Это сообщение является информационным и предшествует ошибке [C1076](../../error-messages/compiler-errors-1/fatal-error-c1076.md).