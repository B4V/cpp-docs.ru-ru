---
title: Реализация CComObjectRootEx | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-atl
ms.topic: conceptual
f1_keywords:
- CComObjectRootEx
dev_langs:
- C++
helpviewer_keywords:
- CComObjectRoot class, implementing
- CComObjectRootEx class
ms.assetid: 79630c44-f2df-4e9e-b730-400a0ebfbd2b
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: f91346febbb84ab7c1978740e0cbc6f0c43cbb4b
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46052638"
---
# <a name="implementing-ccomobjectrootex"></a>Реализация CComObjectRootEx

[CComObjectRootEx](../atl/reference/ccomobjectrootex-class.md) необходим; все объекты ATL должны иметь один экземпляр `CComObjectRootEx` или [CComObjectRoot](../atl/reference/ccomobjectroot-class.md) в своем наследовании. `CComObjectRootEx` предоставляет механизм по умолчанию `QueryInterface`, основанный на записях сопоставления COM.

Посредством его сопоставления COM интерфейсы объекта предоставляются клиенту, когда он запрашивает интерфейс. Запрос выполняется с помощью `CComObjectRootEx::InternalQueryInterface`. `InternalQueryInterface` обрабатывает интерфейсы только в таблице сопоставлений COM.

Вы можете ввести интерфейсы в таблицу сопоставлений COM с [COM_INTERFACE_ENTRY](reference/com-interface-entry-macros.md#com_interface_entry) макрос или одного из его вариантов. Например, следующий код вводит интерфейсы `IDispatch`, `IBeeper` и `ISupportErrorInfo` в таблицу сопоставлений COM:

[!code-cpp[NVC_ATL_COM#1](../atl/codesnippet/cpp/implementing-ccomobjectrootex_1.h)]

## <a name="see-also"></a>См. также

[Основы COM-объектов ATL](../atl/fundamentals-of-atl-com-objects.md)<br/>
[Макросы сопоставления COM](../atl/reference/com-map-macros.md)

