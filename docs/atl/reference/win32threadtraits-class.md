---
title: Класс Win32ThreadTraits | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-atl
ms.topic: reference
f1_keywords:
- Win32ThreadTraits
- ATLBASE/ATL::Win32ThreadTraits
- ATLBASE/ATL::Win32ThreadTraits::CreateThread
dev_langs:
- C++
helpviewer_keywords:
- threading [ATL], Windows threads
- threading [ATL], creation functions
- Win32ThreadTraits class
ms.assetid: 50279c38-eae1-4301-9ea6-97ccea580f3e
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: baab04880c19cac1e0c291f2b4d8a274dea1c21b
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46044942"
---
# <a name="win32threadtraits-class"></a>Класс Win32ThreadTraits

Этот класс предоставляет функции создания для потока Windows. Этот класс используется в том случае, если поток не будет использовать функции CRT.

> [!IMPORTANT]
>  Этот класс и его члены не может использоваться в приложениях, выполняемых в среде выполнения Windows.

## <a name="syntax"></a>Синтаксис

```
class Win32ThreadTraits
```

## <a name="members"></a>Участники

### <a name="public-methods"></a>Открытые методы

|Имя|Описание|
|----------|-----------------|
|[Win32ThreadTraits::CreateThread](#createthread)|(Статический) Вызывайте эту функцию для создания потока, который не следует использовать функции CRT.|

## <a name="remarks"></a>Примечания

Поток признаки являются классы, предоставляющие функции создания для определенного типа потока. Функция создания совпадает с той же сигнатуре и семантику Windows [CreateThread](/windows/desktop/api/processthreadsapi/nf-processthreadsapi-createthread) функции.

Поток признаки используются следующие классы:

- [CThreadPool](../../atl/reference/cthreadpool-class.md)

- [CWorkerThread](../../atl/reference/cworkerthread-class.md)

Если поток будет использовать функции CRT, используйте [CRTThreadTraits](../../atl/reference/crtthreadtraits-class.md) вместо этого.

## <a name="requirements"></a>Требования

**Заголовок:** atlbase.h

##  <a name="createthread"></a>  Win32ThreadTraits::CreateThread

Вызывайте эту функцию для создания потока, который не следует использовать функции CRT.

```
static HANDLE CreateThread(
    LPSECURITY_ATTRIBUTES lpsa,
    DWORD dwStackSize,
    LPTHREAD_START_ROUTINE pfnThreadProc,
    void* pvParam,
    DWORD dwCreationFlags,
    DWORD* pdwThreadId) throw();
```

### <a name="parameters"></a>Параметры

*lpsa*<br/>
Атрибуты безопасности для нового потока.

*dwStackSize*<br/>
Размер стека для нового потока.

*pfnThreadProc*<br/>
Процедура потока нового потока.

*pvParam*<br/>
Параметр, передаваемый в процедуру потока.

*dwCreationFlags*<br/>
Создание флагов ("0" или "CREATE_SUSPENDED").

*pdwThreadId*<br/>
[out] Адрес переменной DWORD, который, в случае успешного выполнения получает идентификатор только что созданному потоку.

### <a name="return-value"></a>Возвращаемое значение

Возвращает дескриптор в только что созданному потоку или значение NULL в случае сбоя. Вызовите [GetLastError](https://msdn.microsoft.com/library/windows/desktop/ms679360) Чтобы получить расширенные сведения об ошибке.

### <a name="remarks"></a>Примечания

См. в разделе [CreateThread](/windows/desktop/api/processthreadsapi/nf-processthreadsapi-createthread) для получения дополнительных сведений о параметрах для этой функции.

Эта функция вызывает `CreateThread` при создании потока.

## <a name="see-also"></a>См. также

[Общие сведения о классе](../../atl/atl-class-overview.md)
