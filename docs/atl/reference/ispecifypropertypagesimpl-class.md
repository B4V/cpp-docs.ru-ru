---
title: Класс ISpecifyPropertyPagesImpl | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-atl
ms.topic: reference
f1_keywords:
- ISpecifyPropertyPagesImpl
- ATLCOM/ATL::ISpecifyPropertyPagesImpl
- ATLCOM/ATL::ISpecifyPropertyPagesImpl::GetPages
dev_langs:
- C++
helpviewer_keywords:
- property pages, CLSIDs associated with
- ISpecifyPropertyPages
- ISpecifyPropertyPagesImpl class
ms.assetid: 4e4b9795-b656-4d56-9b8c-85941e7731f9
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 86ad1f489553d1637683ac1310bfe2b9be04ffb0
ms.sourcegitcommit: a9dcbcc85b4c28eed280d8e451c494a00d8c4c25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2018
ms.locfileid: "50064762"
---
# <a name="ispecifypropertypagesimpl-class"></a>Класс ISpecifyPropertyPagesImpl

Этот класс реализует `IUnknown` и предоставляет реализацию по умолчанию [ISpecifyPropertyPages](/windows/desktop/api/ocidl/nn-ocidl-ispecifypropertypages) интерфейс.

> [!IMPORTANT]
>  Этот класс и его члены не может использоваться в приложениях, выполняемых в среде выполнения Windows.

## <a name="syntax"></a>Синтаксис

```
template<class T>
class ATL_NO_VTABLE ISpecifyPropertyPagesImpl
   : public ISpecifyPropertyPages
```

#### <a name="parameters"></a>Параметры

*T*<br/>
Ваш класс, производный от `ISpecifyPropertyPagesImpl`.

## <a name="members"></a>Участники

### <a name="public-methods"></a>Открытые методы

|Имя|Описание|
|----------|-----------------|
|[ISpecifyPropertyPagesImpl::GetPages](#getpages)|Заполняет значения подсчета массив UUID. Каждый UUID соответствует CLSID для одного из страницы свойств, которые могут отображаться в окне свойств объекта.|

## <a name="remarks"></a>Примечания

[ISpecifyPropertyPages](/windows/desktop/api/ocidl/nn-ocidl-ispecifypropertypages) интерфейс позволяет клиенту получить список идентификаторов CLSID для страниц свойств, поддерживаемых объектом. Класс `ISpecifyPropertyPagesImpl` предоставляет стандартную реализацию этого интерфейса и реализует `IUnknown` , отправляя данные в дамп сборок устройства в режиме отладки.

> [!NOTE]
>  Не предоставляйте `ISpecifyPropertyPages` интерфейс, если объект поддерживает страницы свойств.

**Связанные статьи** [учебник по ATL](../../atl/active-template-library-atl-tutorial.md), [Создание проекта ATL](../../atl/reference/creating-an-atl-project.md)

## <a name="inheritance-hierarchy"></a>Иерархия наследования

`ISpecifyPropertyPages`

`ISpecifyPropertyPagesImpl`

## <a name="requirements"></a>Требования

**Заголовок:** atlcom.h

##  <a name="getpages"></a>  ISpecifyPropertyPagesImpl::GetPages

Заполняет массив [CAUUID](/windows/desktop/api/ocidl/ns-ocidl-tagcauuid) структуру с CLSID для страниц свойств, которые могут отображаться в окне свойств объекта.

```
STDMETHOD(GetPages)(CAUUID* pPages);
```

### <a name="remarks"></a>Примечания

ATL использует сопоставление свойств объекта для получения каждого CLSID.

См. в разделе [ISpecifyPropertyPages::GetPages](/windows/desktop/api/ocidl/nf-ocidl-ispecifypropertypages-getpages) в Windows SDK.

## <a name="see-also"></a>См. также

[Класс IPropertyPageImpl](../../atl/reference/ipropertypageimpl-class.md)<br/>
[Класс IPerPropertyBrowsingImpl](../../atl/reference/iperpropertybrowsingimpl-class.md)<br/>
[Общие сведения о классе](../../atl/atl-class-overview.md)
