---
title: 'Элементов управления MFC ActiveX: События | Документация Майкрософт'
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-mfc
ms.topic: conceptual
dev_langs:
- C++
helpviewer_keywords:
- MFC ActiveX controls [MFC], events
- notifications [MFC], notifying containers of events
- custom events [MFC], adding to ActiveX controls
- events [MFC], mapping
- COleControl class [MFC], handling of events
- mappings [MFC], events
- stock events [MFC]
- container events [MFC]
- events [MFC], ActiveX controls
- OLE events [MFC]
ms.assetid: e1e57e0c-206b-4923-a0b5-682c26564f74
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: a4c60c949832f03df6b7bb0e69cfdd95dfafc137
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46422874"
---
# <a name="mfc-activex-controls-events"></a>Элементы управления ActiveX в MFC. События

Элементы управления ActiveX использовать события для уведомления о контейнере, что что-то произошло в элемент управления. Распространенные примеры событий включают щелчков мыши на элементе управления, данные, введенные с помощью клавиатуры и изменения в состоянии элемента управления. При возникновении этих действий, элемент управления вызывает событие для оповещения в контейнер.

События также вызываются сообщения.

MFC поддерживает два типа событий: стандартных и пользовательских. Событий биржевых являются те события, которые класс [COleControl](../mfc/reference/colecontrol-class.md) обрабатывает автоматически. Полный список событий хранения, см. в статье [элементы ActiveX в MFC: Добавление события Stock](../mfc/mfc-activex-controls-adding-stock-events-to-an-activex-control.md). Пользовательские события позволяют элемент управления может уведомлять контейнера, когда происходит действие, относящиеся к данному элементу. Некоторые примеры будет взиматься плата за внутреннее состояние элемента управления или получения определенного сообщения окна.

Элемент управления для порождения событий должным образом классе элемента управления необходимо сопоставить каждое событие элемента управления на функцию-член, который должен быть вызван при возникновении соответствующего события. Этот механизм сопоставления (называется картой событий) позволяет централизовать сведения о событии и позволяет легко получать доступ и управлять события элемента управления Visual Studio. Эта карта событие объявляется с следующий макрос, расположенный в заголовке (. H) файл объявления класса элемента управления:

[!code-cpp[NVC_MFC_AxUI#2](../mfc/codesnippet/cpp/mfc-activex-controls-events_1.h)]

После объявления карты событий, он должен быть определен в реализации элемента управления (. Файл CPP). Следующие строки кода определяют карты событий, что элемент управления для запуска определенных событий:

[!code-cpp[NVC_MFC_AxUI#3](../mfc/codesnippet/cpp/mfc-activex-controls-events_2.cpp)]
[!code-cpp[NVC_MFC_AxUI#4](../mfc/codesnippet/cpp/mfc-activex-controls-events_3.cpp)]

Если вы используете мастер элементов управления ActiveX MFC для создания проекта, автоматически добавляет эти строки. Если вы не используете мастер элементов управления MFC ActiveX, необходимо добавить следующие строки вручную.

В представлении класса, можно добавить акций события, поддерживаемые классом `COleControl` или пользовательские события, определенных вами. Для каждого нового события представление классов автоматически добавляет соответствующие записи карты событий элемента управления и элемента управления. IDL-файла.

Два других статьях рассматриваются события подробно:

- [Элементы ActiveX в MFC: Добавление событий хранения](../mfc/mfc-activex-controls-adding-stock-events-to-an-activex-control.md)

- [Элементы ActiveX в MFC. Добавление пользовательских событий](../mfc/mfc-activex-controls-adding-custom-events.md)

## <a name="see-also"></a>См. также

[Элементы ActiveX библиотеки MFC](../mfc/mfc-activex-controls.md)<br/>
[Элементы ActiveX в MFC. Методы](../mfc/mfc-activex-controls-methods.md)<br/>
[Класс COleControl](../mfc/reference/colecontrol-class.md)
