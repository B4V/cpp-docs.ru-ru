---
title: Форматирование символов в элементы управления Rich Edit | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-mfc
ms.topic: conceptual
dev_langs:
- C++
helpviewer_keywords:
- formatting [MFC], characters
- rich edit controls [MFC], character formatting in
- CRichEditCtrl class [MFC], character formatting in
ms.assetid: c80f4305-75ad-45f9-8d17-d83d0fe79be5
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 75ac8637e5157434cd5729695b30a443bbd31cf5
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46403166"
---
# <a name="character-formatting-in-rich-edit-controls"></a>Форматирование знаков с использованием элементов управления "Rich Edit"

Можно использовать функции-члены элемента управления форматированным редактированием ([CRichEditCtrl](../mfc/reference/cricheditctrl-class.md)) для форматирования символов и получить сведения о форматировании. Для символов можно указать шрифт, размер, цвет и эффекты, например полужирный шрифт, курсив и защищены.

Можно применить форматирование символов с помощью [SetSelectionCharFormat](../mfc/reference/cricheditctrl-class.md#setselectioncharformat) и [SetWordCharFormat](../mfc/reference/cricheditctrl-class.md#setwordcharformat) функций-членов. Чтобы определить текущий символ форматирование для выделенного текста, используйте [GetSelectionCharFormat](../mfc/reference/cricheditctrl-class.md#getselectioncharformat) функция-член. [CHARFORMAT](/windows/desktop/api/richedit/ns-richedit-_charformat) структура будет использована в эти функции-члены для указания атрибутов символов. Один из важные члены **CHARFORMAT** — **dwMask**. В `SetSelectionCharFormat` и `SetWordCharFormat`, **dwMask** указывает, какие атрибуты символ установит этим вызовом функции. `GetSelectionCharFormat` Представляет атрибуты первого символа в выделенном фрагменте; **dwMask** указывает атрибуты, которые они единообразны во всем выделения.

Можно также получить и «по умолчанию форматирование,» это форматирование, применяемое к любой впоследствии вставленные символы. Например если приложение устанавливает символ по умолчанию форматирование будут выводиться полужирным шрифтом, а затем вводе символа, этот символ имеет полужирное начертание. Чтобы получить и форматирование по умолчанию, используйте [GetDefaultCharFormat](../mfc/reference/cricheditctrl-class.md#getdefaultcharformat) и [SetDefaultCharFormat](../mfc/reference/cricheditctrl-class.md#setdefaultcharformat) функций-членов.

Атрибут «защищенной» символ не изменяет внешний вид текста. Если пользователь пытается изменить защищенный текст, в элементе управления rich edit отправляет своему родительскому окну **EN_PROTECTED** сообщение уведомления, позволяя родительского окна, можно разрешить или запретить изменение. Чтобы получить это сообщение уведомления, необходимо включить его с помощью [SetEventMask](../mfc/reference/cricheditctrl-class.md#seteventmask) функция-член. Дополнительные сведения о маску события, см. в разделе [уведомления от изменить элемент управления форматированием](../mfc/notifications-from-a-rich-edit-control.md)далее в этом разделе.

Цвет переднего плана является атрибутом символа, но цвет фона является свойством элемента управления форматированным редактированием. Чтобы задать цвет фона, используйте [SetBackgroundColor](../mfc/reference/cricheditctrl-class.md#setbackgroundcolor) функция-член.

## <a name="see-also"></a>См. также

[Использование CRichEditCtrl](../mfc/using-cricheditctrl.md)<br/>
[Элементы управления](../mfc/controls-mfc.md)

