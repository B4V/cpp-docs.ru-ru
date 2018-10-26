---
title: Derefhelper-структура | Документация Майкрософт
ms.custom: ''
ms.date: 10/03/2018
ms.technology:
- cpp-windows
ms.topic: reference
f1_keywords:
- async/Microsoft::WRL::Details::DerefHelper
dev_langs:
- C++
helpviewer_keywords:
- DerefHelper structure
ms.assetid: 86ded58b-c3ee-4a4f-bb86-4f67b895d427
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
- uwp
ms.openlocfilehash: 2d9339256d4dfda717d52b11da965b3600a53cd1
ms.sourcegitcommit: 955ef0f9d966e7c9c65e040f1e28fa83abe102a5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/04/2018
ms.locfileid: "48788361"
---
# <a name="derefhelper-structure"></a>DerefHelper - структура

Поддерживает инфраструктуру WRL и не предназначен для использования непосредственно из программного кода.

## <a name="syntax"></a>Синтаксис

```cpp
template <typename T>
struct DerefHelper;

template <typename T>
struct DerefHelper<T*>;
```

### <a name="parameters"></a>Параметры

*T*<br/>
Параметр шаблона.

## <a name="remarks"></a>Примечания

Представляет разыменованный указатель на параметр шаблона `T*`.

**DerefHelper** используется в выражении, например: `ComPtr<Details::DerefHelper<ProgressTraits::Arg1Type>::DerefType> operationInterface;`.

## <a name="members"></a>Участники

### <a name="public-typedefs"></a>Общедоступные определения типов

|Имя|Описание|
|----------|-----------------|
|`DerefType`|Идентификатор для разыменованного параметра шаблона `T*`.|

## <a name="inheritance-hierarchy"></a>Иерархия наследования

`DerefHelper`

## <a name="requirements"></a>Требования

**Заголовок:** async.h

**Пространство имен:** Microsoft::wrl:: Details

## <a name="see-also"></a>См. также

[Пространство имен Microsoft::WRL::Details](../windows/microsoft-wrl-details-namespace.md)