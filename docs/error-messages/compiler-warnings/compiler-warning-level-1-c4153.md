---
title: Предупреждение компилятора (уровень 1) C4153 | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-diagnostics
ms.topic: error-reference
f1_keywords:
- C4153
dev_langs:
- C++
helpviewer_keywords:
- C4153
ms.assetid: 37a15754-9dba-470b-adda-c4b888064b3e
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 99aa207c550004eee1db906acf5dc567e9859f7c
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46074088"
---
# <a name="compiler-warning-level-1-c4153"></a>Предупреждение компилятора (уровень 1) C4153

преобразование указателя на функцию в указатель на данные (или наоборот) в выражении

Указатель на функцию преобразуется в указатель на данные или наоборот. Подобное преобразование допустимо при использовании расширений Майкрософт (/Ze), но не в ANSI C.