---
title: Использование CToolTipCtrl для создания объекта CToolTipCtrl и управления | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-mfc
ms.topic: conceptual
f1_keywords:
- CToolTipCtrl
dev_langs:
- C++
helpviewer_keywords:
- tool tips [MFC], creating
- CToolTipCtrl class [MFC], using
ms.assetid: 0a34583f-f66d-46a1-a239-31b80ea395ad
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 186972164496889b471ebfc11e19017129ad943b
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46378986"
---
# <a name="using-ctooltipctrl-to-create-and-manipulate-a-ctooltipctrl-object"></a>Использование CToolTipCtrl для создания объекта CToolTipCtrl и управления им

Ниже приведен пример [CToolTipCtrl](../mfc/reference/ctooltipctrl-class.md) использования:

### <a name="to-create-and-manipulate-a-ctooltipctrl"></a>Для создания и обработки CToolTipCtrl

1. Создать `CToolTipCtrl` объекта.

1. Вызовите [создать](../mfc/reference/ctooltipctrl-class.md#create) для создания общих Windows/всплывающая подсказка и присоединить его к `CToolTipCtrl` объекта.

1. Вызовите [AddTool](../mfc/reference/ctooltipctrl-class.md#addtool) для регистрации средством управления всплывающей подсказки, так что сведениями, хранящимися в подсказке отображается в том случае, когда курсор находится в средстве.

1. Вызовите [SetToolInfo](../mfc/reference/ctooltipctrl-class.md#settoolinfo) для задания данных, поддерживающий во всплывающей подсказке инструмента.

1. Вызовите [SetToolRect](../mfc/reference/ctooltipctrl-class.md#settoolrect) присвоить новый ограничивающий прямоугольник для средства.

1. Вызовите [HitTest](../mfc/reference/ctooltipctrl-class.md#hittest) для тестирования точку, чтобы определить, будь то внутри ограничивающего прямоугольника данное средство и если да, получить информацию об этом инструменте.

1. Вызовите [GetToolCount](../mfc/reference/ctooltipctrl-class.md#gettoolcount) для извлечения количества средств, зарегистрированные с элементом управления всплывающей подсказки.

## <a name="see-also"></a>См. также

[Использование CToolTipCtrl](../mfc/using-ctooltipctrl.md)<br/>
[Элементы управления](../mfc/controls-mfc.md)

