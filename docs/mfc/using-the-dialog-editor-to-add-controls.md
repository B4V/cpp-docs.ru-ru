---
title: Использование редактора диалоговых окон для добавления элементов управления | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-mfc
ms.topic: conceptual
dev_langs:
- C++
helpviewer_keywords:
- Windows common controls [MFC], adding
- dialog box controls [MFC], adding to dialog boxes
- controls [MFC], adding to dialog boxes
- Dialog editor, creating controls
- common controls [MFC], adding
ms.assetid: d3f9f994-7e54-4656-a545-42c204557c36
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: ffbfad4025e9daf72a9555ca69a8639cba6d68c5
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46374727"
---
# <a name="using-the-dialog-editor-to-add-controls"></a>Использование редактора диалоговых окон для добавления элементов управления

При создании ресурса шаблона диалогового окна с [редактор диалоговых окон](../windows/dialog-editor.md), перетащите элементы управления из палитры элементов управления и перетащить их в диалоговом окне. Это добавляет спецификации для данного типа элемента управления ресурса шаблона диалогового окна. При создании объекта диалогового окна и вызовите его `Create` или `DoModal` функция-член, платформа создает элемент управления Windows и помещает его в диалоговом окне на экране.

Вы можете вместо этого [вручную создавать элементы управления](../mfc/adding-controls-by-hand.md) Если требуется. Это больше работы.

## <a name="see-also"></a>См. также

[Создание и использование элементов управления](../mfc/making-and-using-controls.md)<br/>
[Элементы управления](../mfc/controls-mfc.md)

