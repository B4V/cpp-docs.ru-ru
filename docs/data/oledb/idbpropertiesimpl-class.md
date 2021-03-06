---
title: Класс IDBPropertiesImpl | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-data
ms.topic: reference
f1_keywords:
- IDBPropertiesImpl
- ATL.IDBPropertiesImpl
- ATL.IDBPropertiesImpl<T>
- ATL::IDBPropertiesImpl<T>
- ATL::IDBPropertiesImpl
- IDBPropertiesImpl::GetProperties
- IDBPropertiesImpl.GetProperties
- GetProperties
- IDBPropertiesImpl::GetPropertyInfo
- IDBPropertiesImpl.GetPropertyInfo
- GetPropertyInfo
- IDBPropertiesImpl.SetProperties
- SetProperties
- IDBPropertiesImpl::SetProperties
dev_langs:
- C++
helpviewer_keywords:
- IDBPropertiesImpl class
- GetProperties method
- GetPropertyInfo method
- SetProperties method
ms.assetid: a7f15a8b-95b2-4316-b944-d5d03f8d74ab
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
- data-storage
ms.openlocfilehash: fc27506657e1e2eeb7fdb7d0d5ef9147d5442dbc
ms.sourcegitcommit: a9dcbcc85b4c28eed280d8e451c494a00d8c4c25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2018
ms.locfileid: "50060798"
---
# <a name="idbpropertiesimpl-class"></a>Класс IDBPropertiesImpl

Предоставляет реализацию для `IDBProperties` интерфейс.

## <a name="syntax"></a>Синтаксис

```cpp
template <class T>
class ATL_NO_VTABLE IDBPropertiesImpl
   : public IDBProperties, public CUtlProps<T>
```

### <a name="parameters"></a>Параметры

*T*<br/>
Ваш класс, производный от `IDBPropertiesImpl`.

## <a name="requirements"></a>Требования

**Заголовок:** atldb.h

## <a name="members"></a>Участники

### <a name="interface-methods"></a>Методы интерфейса

|||
|-|-|
|[GetProperties](#getproperties)|Возвращает значения свойств источника данных, источника данных и инициализации свойства групп, заданных в настоящее время на объекте источника данных или значений свойств в группе свойств инициализации, заданных в настоящее время на перечислитель.|
|[GetPropertyInfo](#getpropertyinfo)|Возвращает сведения обо всех свойствах, поддерживаемых поставщиком.|
|[SetProperties](#setproperties)|Задает свойства в источнике данных и инициализации групп свойств, для объектов источников данных, или группу свойств инициализации, для перечислителей.|

## <a name="remarks"></a>Примечания

[IDBProperties](/previous-versions/windows/desktop/ms719607) обязательный интерфейс для объектов источников данных и дополнительный интерфейс для перечислителей. Тем не менее если перечислитель предоставляет [IDBInitialize](/previous-versions/windows/desktop/ms713706), она должна предоставлять `IDBProperties`. `IDBPropertiesImpl` реализует `IDBProperties` с помощью статической функции, определяемые [BEGIN_PROPSET_MAP](../../data/oledb/begin-propset-map.md).

## <a name="getproperties"></a> IDBPropertiesImpl::GetProperties

Возвращает значения свойств источника данных, источника данных и инициализации свойства групп, заданных в настоящее время на объекте источника данных или значений свойств в группе свойств инициализации, заданных в настоящее время на перечислитель.

### <a name="syntax"></a>Синтаксис

```cpp
STDMETHOD(GetProperties)(ULONG cPropertySets, 
   const DBPROPIDSET rgPropertySets[], 
   ULONG * pcProperties, 
   DBPROPSET ** prgProperties);
```

#### <a name="parameters"></a>Параметры

См. в разделе [IDBProperties::GetProperties](/previous-versions/windows/desktop/ms714344) в *справочнике программиста OLE DB*.

Некоторые параметры соответствуют *Справочник программиста OLE DB по* параметры разные имена, которые описаны в `IDBProperties::GetProperties`:

|Параметры шаблона OLE DB|*Справочник программиста OLE DB по* параметров|
|--------------------------------|------------------------------------------------|
|*cPropertySets*|*cPropertyIDSets*|
|*rgPropertySets*|*rgPropertyIDSets*|
|*pcProperties*|*pcPropertySets*|
|*prgProperties*|*prgPropertySets*|

### <a name="remarks"></a>Примечания

При инициализации, этот метод возвращает значения свойств в DBPROPSET_DATASOURCE, DBPROPSET_DATASOURCEINFO, DBPROPSET_DBINIT группы свойств, которые в настоящее время заданы на объекте источника данных. Если поставщик не инициализирован, он возвращает только свойства группы DBPROPSET_DBINIT.

## <a name="getpropertyinfo"></a> IDBPropertiesImpl::GetPropertyInfo

Возвращает сведения о свойствах, поддерживаемых источником данных.

### <a name="syntax"></a>Синтаксис

```cpp
STDMETHOD(GetPropertyInfo)(ULONG cPropertySets, 
   const DBPROPIDSET rgPropertySets[], 
   ULONG * pcPropertyInfoSets, 
   DBPROPINFOSET ** prgPropertyInfoSets, 
   OLECHAR ** ppDescBuffer);
```

#### <a name="parameters"></a>Параметры

См. в разделе [IDBProperties::GetPropertyInfo](/previous-versions/windows/desktop/ms718175) в *справочнике программиста OLE DB*.

Некоторые параметры соответствуют *Справочник программиста OLE DB по* параметры разные имена, которые описаны в `IDBProperties::GetPropertyInfo`:

|Параметры шаблона OLE DB|*Справочник программиста OLE DB по* параметров|
|--------------------------------|------------------------------------------------|
|*cPropertySets*|*cPropertyIDSets*|
|*rgPropertySets*|*rgPropertyIDSets*|

### <a name="remarks"></a>Примечания

Использует [IDBInitializeImpl::m_pCUtlPropInfo](../../data/oledb/idbinitializeimpl-m-pcutlpropinfo.md) для реализации этой функции.

## <a name="setproperties"></a> IDBPropertiesImpl::SetProperties

Задает свойства в источнике данных и инициализации групп свойств, для объектов источников данных, или группу свойств инициализации, для перечислителей.

### <a name="syntax"></a>Синтаксис

```cpp
STDMETHOD(SetProperties)(ULONG cPropertySets, 
   DBPROPSET rgPropertySets[]);
```

#### <a name="parameters"></a>Параметры

См. в разделе [IDBProperties::SetProperties](/previous-versions/windows/desktop/ms723049) в *справочнике программиста OLE DB*.

### <a name="remarks"></a>Примечания

При инициализации, этот метод задает значения свойств в DBPROPSET_DATASOURCE, DBPROPSET_DATASOURCEINFO, групп свойств DBPROPSET_DBINIT для объекта источника данных. Если поставщик не инициализирован, он задает DBPROPSET_DBINIT только свойства группы.

## <a name="see-also"></a>См. также

[Шаблоны поставщика OLE DB](../../data/oledb/ole-db-provider-templates-cpp.md)<br/>
[Архитектура шаблона поставщика OLE DB](../../data/oledb/ole-db-provider-template-architecture.md)