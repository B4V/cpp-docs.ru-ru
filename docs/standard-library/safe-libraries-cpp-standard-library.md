---
title: 'Безопасные библиотеки: стандартная библиотека C++ | Документы Майкрософт'
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-standard-libraries
ms.topic: reference
f1_keywords:
- _SCL_SECURE_NO_DEPRECATE
dev_langs:
- C++
helpviewer_keywords:
- Safe Libraries
- Safe Libraries, C++ Standard Library
- Safe C++ Standard Library
ms.assetid: 3993340f-1f29-4d81-b3f5-52a52bc8e148
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 0a139be1598dfdeaaece5c4b2cf8d253beb754ff
ms.sourcegitcommit: d55ac596ba8f908f5d91d228dc070dad31cb8360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/08/2018
ms.locfileid: "33859050"
---
# <a name="safe-libraries-c-standard-library"></a>Безопасные библиотеки: стандартная библиотека C++

В библиотеки, входящие в состав Visual C++ (включая стандартную библиотеку C++), были внесены различные улучшения, чтобы сделать их более безопасными.

В стандартной библиотеке C++ несколько методов оказались потенциально небезопасными, так как могли привести к переполнению буфера или другим дефектам кода. Использовать эти методы не рекомендуется; вместо них созданы новые, более безопасные методы. Эти новые методы оканчиваются на `_s`.

Также были внесены некоторые улучшения для повышения безопасности итераторов и алгоритмов. Дополнительные сведения см. в разделах [Проверяемые итераторы](../standard-library/checked-iterators.md), [Поддержка в отладке итераторов](../standard-library/debug-iterator-support.md) и [_ITERATOR_DEBUG_LEVEL](../standard-library/iterator-debug-level.md).

## <a name="remarks"></a>Примечания

В следующей таблице перечислены потенциально небезопасные методы стандартной библиотеки C++, а также их более безопасные эквиваленты:

|Потенциально небезопасный метод|Более безопасный эквивалент|
|-------------------------------|----------------------|
|[copy](../standard-library/basic-string-class.md#copy)|[basic_string::_Copy_s](../standard-library/basic-string-class.md#copy_s)|
|[copy](../standard-library/char-traits-struct.md#copy)|[char_traits::_Copy_s](../standard-library/char-traits-struct.md#copy_s)|

При вызове любого из перечисленных выше потенциально небезопасных методов или при неправильном использовании итераторов компилятор создает [Предупреждение компилятора (уровень 3) С4996](../error-messages/compiler-warnings/compiler-warning-level-3-c4996.md). Сведения о том, как отключить эти предупреждения, см. в разделе [_SCL_SECURE_NO_WARNINGS](../standard-library/scl-secure-no-warnings.md).

## <a name="in-this-section"></a>В этом разделе

[_ITERATOR_DEBUG_LEVEL](../standard-library/iterator-debug-level.md)

[_SCL_SECURE_NO_WARNINGS](../standard-library/scl-secure-no-warnings.md)

[Checked Iterators](../standard-library/checked-iterators.md)

[Debug Iterator Support](../standard-library/debug-iterator-support.md)

## <a name="see-also"></a>См. также

[Общие сведения о стандартной библиотеке C++](../standard-library/cpp-standard-library-overview.md)<br/>
