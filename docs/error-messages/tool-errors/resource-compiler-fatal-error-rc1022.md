---
title: Неустранимая ошибка компилятора ресурсов RC1022 | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-diagnostics
ms.topic: error-reference
f1_keywords:
- RC1022
dev_langs:
- C++
helpviewer_keywords:
- RC1022
ms.assetid: 30a0f3c7-08a8-4c40-b0de-46ee5feb789d
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 4186b531fce1b608122df676139b9c676ce2df27
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46070452"
---
# <a name="resource-compiler-fatal-error-rc1022"></a>Неустранимая ошибка компилятора ресурсов RC1022

Непредвиденный «#endif»

`#if`, **#Ifdef**, или **#ifndef** директива не заканчивается `#endif` директива.

Убедитесь, что имеется `#if`, **#ifdef**, или **#ifndef** фактически перед этой инструкцией.