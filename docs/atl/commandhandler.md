---
title: CommandHandler | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-atl
ms.topic: reference
f1_keywords:
- CommandHandler
dev_langs:
- C++
helpviewer_keywords:
- CommandHandler function
ms.assetid: 662bc7bf-4a10-42b3-986d-d8bae4f63551
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 841630266778389969ead9191f7a2a31e20e7975
ms.sourcegitcommit: a9dcbcc85b4c28eed280d8e451c494a00d8c4c25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2018
ms.locfileid: "50055155"
---
# <a name="commandhandler"></a>CommandHandler

`CommandHandler` функция, определяемая параметром третий параметр макроса COMMAND_HANDLER в схему сообщения.

## <a name="syntax"></a>Синтаксис

```cpp
LRESULT CommandHandler(
    WORD wNotifyCode,
    WORD wID,
    HWND hWndCtl,
    BOOL& bHandled);
```

#### <a name="parameters"></a>Параметры

*wNotifyCode*<br/>
Код уведомления.

*wID*<br/>
Идентификатор пункта меню, элемент управления или сочетаний клавиш.

*hWndCtl*<br/>
Дескриптор окна элемента управления.

*bHandled*<br/>
Карта наборов сообщений *bHandled* значение TRUE перед `CommandHandler` вызывается. Если `CommandHandler` не полностью обрабатывает сообщение, она должна задать *bHandled* значение false, чтобы указать, должна дальнейшей обработки сообщения.

## <a name="return-value"></a>Возвращаемое значение

Результат обработки сообщения. 0 в случае успеха.

## <a name="remarks"></a>Примечания

Пример использования этого обработчика сообщений в схеме сообщений, см. в разделе [COMMAND_HANDLER](reference/message-map-macros-atl.md#command_handler).

## <a name="see-also"></a>См. также

[Реализация окна](../atl/implementing-a-window.md)<br/>
[Схемы сообщений](../atl/message-maps-atl.md)<br/>
[WM_NOTIFY](https://msdn.microsoft.com/library/windows/desktop/bb775583)

