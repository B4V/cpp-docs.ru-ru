---
title: HelpContext (атрибут COM C++) | Документация Майкрософт
ms.custom: ''
ms.date: 10/02/2018
ms.technology:
- cpp-windows
ms.topic: reference
f1_keywords:
- vc-attr.helpcontext
dev_langs:
- C++
helpviewer_keywords:
- helpcontext attribute
ms.assetid: 6fbb022d-a4b7-4989-a02f-7f18a9b0ad96
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
- uwp
ms.openlocfilehash: 831ca61f82eee913efd1ab2b1420fefb011d6c1a
ms.sourcegitcommit: a9dcbcc85b4c28eed280d8e451c494a00d8c4c25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2018
ms.locfileid: "50062838"
---
# <a name="helpcontext"></a>helpcontext

Указывает идентификатор контекста, который позволяет пользователю просматривать сведения об этом элементе в **помочь** файл.

## <a name="syntax"></a>Синтаксис

```cpp
[ helpcontext(id) ]
```

### <a name="parameters"></a>Параметры

*id*<br/>
Идентификатор контекста справки. См. в разделе [HTML-справки: Context-Sensitive для ваших программ](../../mfc/html-help-context-sensitive-help-for-your-programs.md) Дополнительные сведения о контексте идентификаторы.

## <a name="remarks"></a>Примечания

**Helpcontext** атрибут C++ имеет ту же функциональность, что [helpcontext](/windows/desktop/Midl/helpcontext) описании атрибута MIDL.

## <a name="example"></a>Пример

См. в примере [defaultvalue](defaultvalue.md) пример демонстрирует использование **helpcontext**.

## <a name="requirements"></a>Требования

### <a name="attribute-context"></a>Контекст атрибута

|||
|-|-|
|**Применение**|**интерфейс**, **typedef**, **класс**, метод, свойство|
|**Повторяемый**|Нет|
|**Обязательные атрибуты**|Нет|
|**Недопустимые атрибуты**|Нет|

Дополнительные сведения см. в разделе [Контексты атрибутов](cpp-attributes-com-net.md#contexts).

## <a name="see-also"></a>См. также

[Атрибуты IDL](idl-attributes.md)<br/>
[Атрибуты интерфейса](interface-attributes.md)<br/>
[Атрибуты классов](class-attributes.md)<br/>
[Атрибуты метода](method-attributes.md)<br/>
[Атрибуты Typedef, Enum, Union и Struct](typedef-enum-union-and-struct-attributes.md)<br/>
[helpfile](helpfile.md)<br/>
[helpstring](helpstring.md)