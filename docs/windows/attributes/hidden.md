---
title: скрытые (атрибут COM C++) | Документация Майкрософт
ms.custom: ''
ms.date: 10/02/2018
ms.technology:
- cpp-windows
ms.topic: reference
f1_keywords:
- vc-attr.hidden
dev_langs:
- C++
helpviewer_keywords:
- hidden attribute
ms.assetid: 199c96dd-fc07-46c7-af93-92020aebebe7
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
- uwp
ms.openlocfilehash: 9934f1f66bf520e8da65953dc3355d447d1844e6
ms.sourcegitcommit: a9dcbcc85b4c28eed280d8e451c494a00d8c4c25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2018
ms.locfileid: "50072964"
---
# <a name="hidden"></a>hidden

Указывает, что элемент существует, но не должен отображаться в пользовательском браузере.

## <a name="syntax"></a>Синтаксис

```cpp
[hidden]
```

## <a name="remarks"></a>Примечания

**Скрытые** атрибут C++ имеет ту же функциональность, что [скрытые](/windows/desktop/Midl/hidden) описании атрибута MIDL.

## <a name="example"></a>Пример

См. в примере [bindable](bindable.md) пример демонстрирует использование **скрытые**.

## <a name="requirements"></a>Требования

### <a name="attribute-context"></a>Контекст атрибута

|||
|-|-|
|**Применение**|**интерфейс**, **класс**, **структуры**, метод, свойство|
|**Повторяемый**|Нет|
|**Обязательные атрибуты**|**Компонентный класс** (при применении к **класс** или **структуры**)|
|**Недопустимые атрибуты**|Нет|

Дополнительные сведения см. в разделе [Контексты атрибутов](cpp-attributes-com-net.md#contexts).

## <a name="see-also"></a>См. также

[Атрибуты IDL](idl-attributes.md)<br/>
[Атрибуты интерфейса](interface-attributes.md)<br/>
[Атрибуты классов](class-attributes.md)<br/>
[Атрибуты метода](method-attributes.md)