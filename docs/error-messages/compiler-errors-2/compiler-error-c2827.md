---
title: Ошибка компилятора C2827 | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-diagnostics
ms.topic: error-reference
f1_keywords:
- C2827
dev_langs:
- C++
helpviewer_keywords:
- C2827
ms.assetid: cb3e5814-0c92-40e4-b620-98578ae3003a
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 139a012f9ed4dd3b6d81d92be3c441df4f899aac
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46052222"
---
# <a name="compiler-error-c2827"></a>Ошибка компилятора C2827

«оператор» не может быть глобально переопределен унарной формой

Оператор не может иметь унарной формой за пределами объекта.

### <a name="to-fix-by-using-the-following-possible-solutions"></a>Возможные способы устранения этой ошибки

1. Внесите перегруженный оператор локального объекта.

1. Выберите подходящий унарный оператор для перегрузки.