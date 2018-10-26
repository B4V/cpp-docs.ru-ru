---
title: Класс CWinTraits | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-atl
ms.topic: reference
f1_keywords:
- CWinTraits
- ATLWIN/ATL::CWinTraits
- ATLWIN/ATL::CWinTraits::GetWndExStyle
- ATLWIN/ATL::CWinTraits::GetWndStyle
dev_langs:
- C++
helpviewer_keywords:
- CMDIChildWinTraits class
- window styles, default values for ATL
- CWinTraits class
- CFrameWinTraits class
- CControlWinTraits class
ms.assetid: f78f486e-6d9c-42c6-8e86-371e05aa7e59
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 69ea4cf411e0ded0f1c324cea439d5a5a4c0c553
ms.sourcegitcommit: a9dcbcc85b4c28eed280d8e451c494a00d8c4c25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2018
ms.locfileid: "50062474"
---
# <a name="cwintraits-class"></a>Класс CWinTraits

Этот класс предоставляет метод для стандартизации стилей, которые используются при создании объекта окна.

> [!IMPORTANT]
>  Этот класс и его члены не может использоваться в приложениях, выполняемых в среде выполнения Windows.

## <a name="syntax"></a>Синтаксис

```
template <DWORD t_dwStyle = 0, DWORD t_dwExStyle = 0>  class CWinTraits
```

#### <a name="parameters"></a>Параметры

*t_dwStyle*<br/>
Стандартное окно Стили по умолчанию.

*t_dwExStyle*<br/>
По умолчанию расширенные стили окна.

## <a name="members"></a>Участники

### <a name="public-methods"></a>Открытые методы

|Имя|Описание|
|----------|-----------------|
|[CWinTraits::GetWndExStyle](#getwndexstyle)|(Статический) Извлекает расширенные стили для `CWinTraits` объекта.|
|[CWinTraits::GetWndStyle](#getwndstyle)|(Статический) Извлекает стандартный стили `CWinTraits` объекта.|

## <a name="remarks"></a>Примечания

Это [характеристиках окна](../../atl/understanding-window-traits.md) класс предоставляет простой метод стандартизации стилей, которые используются для создания объекта ATL окна. Использование специализации этого класса в качестве параметра шаблона для [CWindowImpl](../../atl/reference/cwindowimpl-class.md) или иной классы окон ATL чтобы указать значение по умолчанию стандартные и расширенные стили, используемые для экземпляров этого класса окна.

Этот шаблон используется, когда необходимо предоставить значение по умолчанию стили окна, которые будут использоваться только в том случае, когда другие стили не указаны в вызове [CWindowImpl::Create](../../atl/reference/cwindowimpl-class.md#create).

Библиотека ATL предоставляет три стандартных специализации этого шаблона для часто используемых сочетаний стили окна:

- `CControlWinTraits`

   Предназначен для стандартного элемента управления окна. Используются следующие стандартные стили: WS_CHILD, WS_VISIBLE, WS_CLIPCHILDREN и WS_CLIPSIBLINGS. Существуют не расширенные стили.

- `CFrameWinTraits`

   Предназначен для стандартных фрейме окна. Включают стандартные стили, используемые: WS_OVERLAPPEDWINDOW WS_CLIPCHILDREN и WS_CLIPSIBLINGS. Включить расширенные стили, используемые: WS_EX_APPWINDOW и WS_EX_WINDOWEDGE.

- `CMDIChildWinTraits`

   Предназначен для стандартных дочернего окна интерфейса MDI. Включают стандартные стили, используемые: WS_OVERLAPPEDWINDOW, WS_CHILD, WS_VISIBLE, WS_CLIPCHILDREN и WS_CLIPSIBLINGS. Включить расширенные стили, используемые: WS_EX_MDICHILD.

Если вы хотите убедиться, что некоторые стили заданы для всех экземпляров класса окна одновременно разрешая другие стили, чтобы быть заданы для каждого экземпляра, используйте [CWinTraitsOR](../../atl/reference/cwintraitsor-class.md) вместо этого.

## <a name="requirements"></a>Требования

**Заголовок:** atlwin.h

##  <a name="getwndstyle"></a>  CWinTraits::GetWndStyle

Вызывайте эту функцию для получения стандартных стилей `CWinTraits` объекта.

```
static DWORD GetWndStyle(DWORD dwStyle);
```

### <a name="parameters"></a>Параметры

*dwStyle*<br/>
Стандартные стили, используемые для создания окна. Если *dwStyle* равно 0, значения стиля шаблона (`t_dwStyle`) возвращаются. Если *dwStyle* не равно нулю, *dwStyle* возвращается.

### <a name="return-value"></a>Возвращаемое значение

Стили стандартное окно объекта.

##  <a name="getwndexstyle"></a>  CWinTraits::GetWndExStyle

Вызывайте эту функцию для получения расширенных стилей `CWinTraits` объекта.

```
static DWORD GetWndExStyle(DWORD dwExStyle);
```

### <a name="parameters"></a>Параметры

*dwExStyle*<br/>
Расширенные стили, используемые для создания окна. Если *dwExStyle* равно 0, значения стиля шаблона (`t_dwExStyle`) возвращаются. Если *dwExStyle* не равно нулю, *dwExStyle* возвращается.

### <a name="return-value"></a>Возвращаемое значение

Расширенные стили окна объекта.

## <a name="see-also"></a>См. также

[Общие сведения о классе](../../atl/atl-class-overview.md)<br/>
[Основные сведения о характеристиках окна](../../atl/understanding-window-traits.md)
