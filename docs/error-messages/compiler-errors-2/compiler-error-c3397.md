---
title: Ошибка компилятора C3397 | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-diagnostics
ms.topic: error-reference
f1_keywords:
- C3397
dev_langs:
- C++
helpviewer_keywords:
- C3397
ms.assetid: a8536e87-79c4-4ed7-bd96-42704d06391f
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 80db76886b4de529b75fd402a70af7c9fa2a892c
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46064078"
---
# <a name="compiler-error-c3397"></a>Ошибка компилятора C3397

Агрегатная инициализация не допускается в аргументах по умолчанию

Массив был объявлен неправильно.  См. в разделе [массивы](../../windows/arrays-cpp-component-extensions.md) Дополнительные сведения.

## <a name="example"></a>Пример

Следующий пример приводит к возникновению ошибки C3397:

```
// C3397.cpp
// compile with: /clr
// /clr /c
void Func(array<int> ^p = gcnew array<int> { 1, 2, 3 });   // C3397
void Func2(array<int> ^p = gcnew array<int> (3));   // OK

int main() {
   array<int> ^p = gcnew array<int> { 1, 2, 3};   // OK
}
```