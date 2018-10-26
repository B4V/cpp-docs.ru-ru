---
title: Что сделать фрейма Windows | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-mfc
ms.topic: conceptual
dev_langs:
- C++
helpviewer_keywords:
- frame windows [MFC], about frame windows
- frame windows [MFC], tasks
- MFC, frame windows
ms.assetid: 1148a952-6786-4622-b5a8-68a2d7eae584
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: bf97fb086f9ede43f9679e66a7c917b800f97dc8
ms.sourcegitcommit: e4a690bf33b44432179de0bc537e26616d13c553
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2018
ms.locfileid: "48892193"
---
# <a name="what-frame-windows-do"></a>Функция окон фрейма

Помимо просто кадрирования представления, окон фреймов несут ответственность за многочисленные задачи, связанные с координацию фрейма с ее представлением, а также с приложением. [CMDIFrameWnd](../mfc/reference/cmdiframewnd-class.md) и [CMDIChildWnd](../mfc/reference/cmdichildwnd-class.md) наследовать от [CFrameWnd](../mfc/reference/cframewnd-class.md)и поэтому имеют `CFrameWnd` возможности, а также новые возможности, добавляющие их. Дочерние окна примеры представлений, элементов управления, таких как кнопки и списки с множественным и панели элементов управления, включая диалоговое окно панелей, панели инструментов и строки состояния.

Окна фрейма отвечает за управление макет из его дочерних окон. В платформе MFC окна фрейма помещает любой панели элементов управления, представления и другие дочерние окна внутри клиентской области.

Фрейм окна также перенаправляет команды, чтобы его представлений и может обрабатывать сообщения уведомления из элемента управления windows.

## <a name="what-do-you-want-to-know-more-about"></a>Выберите для получения дополнительных сведений

- [Панели элементов управления (их месте в окне фрейма)](../mfc/control-bars.md)

- [Управление меню, панелей элементов управления и ускорители (их месте в окне фрейма)](../mfc/managing-menus-control-bars-and-accelerators.md)

- [Маршрутизация команд (из окна фрейма для ее просмотра и другие целевые объекты команд)](../mfc/command-routing.md)

- [Архитектура документа/View](../mfc/document-view-architecture.md)

- [Панели элементов управления](../mfc/control-bars.md)

- [Элементы управления](../mfc/controls-mfc.md)

## <a name="see-also"></a>См. также

[Окна фрейма](../mfc/frame-windows.md)

