---
title: Математическая ошибка M6205 | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-diagnostics
ms.topic: error-reference
f1_keywords:
- M6205
dev_langs:
- C++
helpviewer_keywords:
- M6205
ms.assetid: fd28e7c9-a463-4a9c-a863-cc9e75315550
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 55549300a5ea603e4462d5b81679f935319838ca
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46099759"
---
# <a name="math-error-m6205"></a>Математическая ошибка M6205

«функция»: ошибка _TLOSS

Произошла полная потеря значимости (точность).

Эта ошибка может возникать, предоставляя очень много как операнд sin, cos или tan, поскольку операнд должен быть сокращен до число от 0 до 2 * pi.