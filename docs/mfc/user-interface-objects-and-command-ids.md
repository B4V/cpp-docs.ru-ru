---
title: Объекты пользовательского интерфейса и идентификаторы команд | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-mfc
ms.topic: conceptual
dev_langs:
- C++
helpviewer_keywords:
- keyboard shortcuts, associating with IDs
- MFC, command routing
- toolbar controls [MFC], command ID
- menu items, associating with IDs
- user interface objects [MFC], associating with IDs
- command IDs, user interface objects
- command routing [MFC], MFC
- command handling [MFC], user-interface objects
ms.assetid: 4ea19e9b-ed1e-452e-bd33-7f509107a45b
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: e8a61699ddd2c48e36bdfd5936fb4ab7aa56e0a9
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46416127"
---
# <a name="user-interface-objects-and-command-ids"></a>Объекты пользовательского интерфейса и идентификаторы команд

Элементы меню, кнопки панели инструментов и сочетания клавиш являются «объекты пользовательского интерфейса» для создания команды. Каждый такой объект пользовательского интерфейса имеет идентификатор. Связать объект пользовательского интерфейса с помощью команды путем назначения и тот же идентификатор объекта и команды. Как описано в [сообщений](../mfc/messages.md), команды, реализуются в виде специальных сообщений. На рисунке «Команд в Framework» ниже показано, как среда управляет команды. Когда объект пользовательского интерфейса генерирует команды, такие как `ID_EDIT_CLEAR_ALL`, один из объектов в приложении обрабатывает команду, на рисунке ниже, объект документа `OnEditClearAll` функция вызывается через схему сообщений для документа.

![Команды платформы](../mfc/media/vc385p1.gif "vc385p1") команды платформы

На рисунке «Команда обновления в Framework» ниже показано, как MFC обновляет объекты пользовательского интерфейса, такие как элементы меню и кнопки панели инструментов. Прежде чем раскрывающимся меню, или во время цикла простоя в случае кнопки панели инструментов, MFC направляет команды update. На рисунке ниже, объект документа, вызывает обработчик команды обновлений, `OnUpdateEditClearAll`, чтобы включить или отключить объект пользовательского интерфейса.

![Команда обновления в структуре](../mfc/media/vc385p2.png "vc385p2") обновление команды в Framework

## <a name="see-also"></a>См. также

[Сообщения и команды платформы](../mfc/messages-and-commands-in-the-framework.md)

