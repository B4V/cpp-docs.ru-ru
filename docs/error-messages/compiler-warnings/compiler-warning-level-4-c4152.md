---
title: Предупреждение компилятора (уровень 4) C4152 | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-diagnostics
ms.topic: error-reference
f1_keywords:
- C4152
dev_langs:
- C++
helpviewer_keywords:
- C4152
ms.assetid: 6025ab70-d7cf-4730-913a-3ca0b1186a3a
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: cab4d812c91239f277dbacede6db43f669908b0a
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46099633"
---
# <a name="compiler-warning-level-4-c4152"></a>Предупреждение компилятора (уровень 4) C4152

нестандартное расширение, преобразование указателя функции/указателя данных в выражении

Указатель функции преобразуется в указатель данных или наоборот. Подобное преобразование допустимо при использовании расширений Майкрософт (/Ze), но не в ANSI C.