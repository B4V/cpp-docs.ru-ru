---
title: _ITERATOR_DEBUG_LEVEL | Документы Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-standard-libraries
ms.topic: reference
f1_keywords:
- _ITERATOR_DEBUG_LEVEL
dev_langs:
- C++
helpviewer_keywords:
- _ITERATOR_DEBUG_LEVEL
ms.assetid: 718549cd-a9a9-4ab3-867b-aac00b321e67
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 4163542d0ba741e6f0a123cbdcdc44dbbec470d1
ms.sourcegitcommit: 3614b52b28c24f70d90b20d781d548ef74ef7082
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2018
ms.locfileid: "38957795"
---
# <a name="iteratordebuglevel"></a>_ITERATOR_DEBUG_LEVEL

Элементы управления макрос _ITERATOR_DEBUG_LEVEL ли [проверенные итераторы](../standard-library/checked-iterators.md) и [поддержки отладки итераторов](../standard-library/debug-iterator-support.md) включены. Этот макрос заменяет и объединяет функциональные возможности более старых _SECURE_SCL и _HAS_ITERATOR_DEBUGGING макросы.

## <a name="macro-values"></a>Значение макроса

В следующей таблице перечислены возможные значения для макрос _ITERATOR_DEBUG_LEVEL.

|Режим компиляции|Значение макроса|Описание:|
|----------------------|----------------|-----------------|
|**Отладка**|||
||0|Отключает проверенные итераторы и отключает отладку итераторов.|
||1|Включает проверенные итераторы и отключает отладку итераторов.|
||2 (по умолчанию)|Включает отладку итераторов; проверенные итераторы не имеют значения.|
|**Релиз**|||
||0 (по умолчанию)|Отключает проверенные итераторы.|
||1|Включает проверенные итераторы; отладка итераторов не имеет значения.|

В режиме выпуска компилятор создает ошибку, при указании _ITERATOR_DEBUG_LEVEL как 2.

## <a name="remarks"></a>Примечания

Элементы управления макрос _ITERATOR_DEBUG_LEVEL ли [проверенные итераторы](../standard-library/checked-iterators.md) и в режиме отладки, является ли [поддержки отладки итераторов](../standard-library/debug-iterator-support.md) включен. Если _ITERATOR_DEBUG_LEVEL определен как 1 или 2, проверенные итераторы гарантируют, что границы ваших контейнеров не перезаписываются. При 0 _ITERATOR_DEBUG_LEVEL итераторы не проверяются. Если _ITERATOR_DEBUG_LEVEL определен как 1, любой небезопасный итератор может вызвать ошибку во время выполнения и программа будет завершена. Когда _ITERATOR_DEBUG_LEVEL определяется как 2, небезопасный итератор используйте приводит к тому, assert и диалоговое окно ошибки среды выполнения, которая позволяет переключиться в режим отладчика.

Так как макрос _ITERATOR_DEBUG_LEVEL поддерживает функции, аналогичные _SECURE_SCL и _HAS_ITERATOR_DEBUGGING макросы, может быть уверены какие макросы и значения макросов для использования в конкретной ситуации. Чтобы избежать путаницы, рекомендуется использовать только макрос _ITERATOR_DEBUG_LEVEL. Эта таблица описывает значение макроса эквивалентное _ITERATOR_DEBUG_LEVEL для различных значений _SECURE_SCL и _HAS_ITERATOR_DEBUGGING в имеющемся коде.

|**_ITERATOR_DEBUG_LEVEL** |**_SECURE_SCL** |**_HAS_ITERATOR_DEBUGGING**|
|---|---|---|
|0 (значение по умолчанию для релиза)|0 (отключено)|0 (отключено)|
|1|1 (включено)|0 (отключено)|
|2 (значение по умолчанию для отладки)|(неприменимо)|1 (включено в режиме отладки)|

Сведения о том, как отключить предупреждения о проверенных итераторах, см. в разделе [_SCL_SECURE_NO_WARNINGS](../standard-library/scl-secure-no-warnings.md).

### <a name="example"></a>Пример

Чтобы указать значение для макроса _ITERATOR_DEBUG_LEVEL, используйте [/D](../build/reference/d-preprocessor-definitions.md) параметр компилятора, чтобы определить его в командной строке, или использовать `#define` перед стандартной библиотеки C++ они включаются в исходных файлах. Например, в командной строке, чтобы скомпилировать *sample.cpp* в режиме отладки и использования поддержки отладки итераторов, можно указать определение макроса _ITERATOR_DEBUG_LEVEL:

`cl /EHsc /Zi /MDd /D_ITERATOR_DEBUG_LEVEL=1 sample.cpp`

В исходном файле укажите макрос перед любыми заголовками стандартной библиотеки, определяющими итераторы.

```cpp
// sample.cpp

#define _ITERATOR_DEBUG_LEVEL 1

#include <vector>

// ...
```

## <a name="see-also"></a>См. также

[Checked Iterators](../standard-library/checked-iterators.md)<br/>
[Debug Iterator Support](../standard-library/debug-iterator-support.md)<br/>
[Безопасные библиотеки: стандартная библиотека C++](../standard-library/safe-libraries-cpp-standard-library.md)<br/>
