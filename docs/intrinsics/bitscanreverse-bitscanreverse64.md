---
title: _BitScanReverse _BitScanReverse64 | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-tools
ms.topic: reference
f1_keywords:
- _BitScanReverse64
- _BitScanReverse_cpp
- _BitScanReverse
- _BitScanReverse64_cpp
dev_langs:
- C++
helpviewer_keywords:
- bsr instruction
- _BitScanReverse intrinsic
- BitScanReverse intrinsic
ms.assetid: 2520a207-af8b-4aad-9ae7-831abeadf376
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 0867241e983794177cdb53b4bbacd1aadd9b8eba
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46436329"
---
# <a name="bitscanreverse-bitscanreverse64"></a>_BitScanReverse, _BitScanReverse64

**Блок, относящийся только к системам Microsoft**

Найти данные маски от наибольшего значащего разряда (MSB) к наименьшему значащему разряду (LSB) для значащего разряда (1).

## <a name="syntax"></a>Синтаксис

```
unsigned char _BitScanReverse(
   unsigned long * Index,
   unsigned long Mask
);
unsigned char _BitScanReverse64(
   unsigned long * Index,
   unsigned __int64 Mask
);
```

#### <a name="parameters"></a>Параметры

*Index*<br/>
[out] Загрузить с позиции разряда Первый значащий разряд (1) найден.

*Маска*<br/>
[in] 32-разрядная или 64-разрядное значение для поиска.

## <a name="return-value"></a>Возвращаемое значение

Не нуль, если `Index` был установлен, или 0, если значащие разряды не найдены.

## <a name="requirements"></a>Требования

|Встроенная функция|Архитектура|Header|
|---------------|------------------|------------|
|`_BitScanReverse`|x86, ARM, x64|\<Intrin.h >|
|`_BitScanReverse64`|ARM, x64||

## <a name="example"></a>Пример

```
// BitScanReverse.cpp
// compile with: /EHsc
#include <iostream>
#include <intrin.h>
using namespace std;

#pragma intrinsic(_BitScanReverse)

int main()
{
   unsigned long mask = 0x1000;
   unsigned long index;
   unsigned char isNonzero;

   cout << "Enter a positive integer as the mask: " << flush;
   cin >> mask;
   isNonzero = _BitScanReverse(&index, mask);
   if (isNonzero)
   {
      cout << "Mask: " << mask << " Index: " << index << endl;
   }
   else
   {
      cout << "No set bits found.  Mask is zero." << endl;
   }
}
```

## <a name="input"></a>Входные данные

```
12
```

## <a name="sample-output"></a>Пример результатов выполнения

```
Enter a positive integer as the mask:
Mask: 12 Index: 3
```

**Завершение блока, относящегося только к системам Майкрософт**

## <a name="see-also"></a>См. также

[Встроенные инструкции компилятора](../intrinsics/compiler-intrinsics.md)