---
title: Структура DELETEITEMSTRUCT | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-mfc
ms.topic: reference
f1_keywords:
- DELETEITEMSTRUCT
dev_langs:
- C++
helpviewer_keywords:
- DELETEITEMSTRUCT structure [MFC]
ms.assetid: 48d3998c-f4a8-402a-bf90-df3770a78685
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 9061205bdf3697e492b846d160a5b4dd2d154bb9
ms.sourcegitcommit: a9dcbcc85b4c28eed280d8e451c494a00d8c4c25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2018
ms.locfileid: "50065022"
---
# <a name="deleteitemstruct-structure"></a>Структура DELETEITEMSTRUCT

`DELETEITEMSTRUCT` Структура описывает удаленного определяемый владельцем список или поле со списком элемента.

## <a name="syntax"></a>Синтаксис

```
typedef struct tagDELETEITEMSTRUCT { /* ditms */
    UINT CtlType;
    UINT CtlID;
    UINT itemID;
    HWND hwndItem;
    UINT itemData;
} DELETEITEMSTRUCT;
```

#### <a name="parameters"></a>Параметры

*CtlType*<br/>
Указывает ODT_LISTBOX (-владельцем список) или ODT_COMBOBOX (рисуемое владельцем со списком).

*CtlID*<br/>
Указывает идентификатор в поле со списком или в поле со списком.

*Идентификатор элемента*<br/>
Указывает индекс элемента в список или поле со списком для удаления.

*hwndItem*<br/>
Определяет элемент управления.

*itemData*<br/>
Задает определяемые приложением данные для элемента. Это значение передается в элемент управления в *lParam* параметр сообщения, который добавляет элемент в список или поле со списком.

## <a name="remarks"></a>Примечания

При удалении элемента из списка или поля со списком или при уничтожении список или поле со списком, Windows отправляет сообщение WM_DELETEITEM владельца для каждого удаляемого элемента. *LParam* параметр сообщения содержит указатель на структуру.

## <a name="requirements"></a>Требования

**Заголовок:** atldbcli.h

## <a name="see-also"></a>См. также

[Структуры, стили, обратные вызовы и схемы сообщений](../../mfc/reference/structures-styles-callbacks-and-message-maps.md)<br/>
[CWnd::OnDeleteItem](../../mfc/reference/cwnd-class.md#ondeleteitem)

