---
title: Неустранимая ошибка C1209 | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-diagnostics
ms.topic: error-reference
f1_keywords:
- C1209
dev_langs:
- C++
helpviewer_keywords:
- C1209
ms.assetid: aa9ee10f-abe3-4683-9792-adca4cbbabb5
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: e518cacdeb8db133ff6378e6569ee868312b8333
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46081498"
---
# <a name="fatal-error-c1209"></a>Неустранимая ошибка C1209

Дружественные сборки не поддерживаются установленной версией среды выполнения

Ошибка C1208 возникает, когда компилятор из текущего выпуска используется со средой CLR из предыдущего выпуска.

Некоторые функциональные возможности компилятора могут не работать в предыдущей версии среды выполнения.

Чтобы устранить ошибку C1209, установите среду CLR, поставляемую вместе с используемым компилятором.

Дополнительные сведения см. в разделе [дружественные сборки (C++)](../../dotnet/friend-assemblies-cpp.md).