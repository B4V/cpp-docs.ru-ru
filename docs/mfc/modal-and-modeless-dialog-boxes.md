---
title: Модальные и немодальные диалоговые окна | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-mfc
ms.topic: conceptual
dev_langs:
- C++
helpviewer_keywords:
- MFC dialog boxes [MFC], modeless
- modeless dialog boxes [MFC]
- MFC dialog boxes [MFC], modal
- modal dialog boxes [MFC]
ms.assetid: e83df336-5994-4b8f-8233-7942f997315b
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 6e355c3bcef9edb68e49903dafbf4719fe0aa925
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46417531"
---
# <a name="modal-and-modeless-dialog-boxes"></a>Модальные и немодальные диалоговые окна

Можно использовать класс [CDialog](../mfc/reference/cdialog-class.md) для управления два вида диалоговых окон:

- *Модальные диалоговые окна*, который пользователь должен ответить перед продолжением работы программы

- *Безрежимные диалоговые окна*, который оставаться на экране и доступны для использования в любое время, но разрешить другие действия пользователя

Редактирование ресурсов и процедуры по созданию шаблона диалогового окна одинаковы для модальные и немодальные диалоговые окна.

Создание диалогового окна для программы необходимо выполнить следующие действия:

1. Используйте [редактор диалоговых окон](../windows/dialog-editor.md) проектировать диалоговое окно и создать его ресурса шаблона диалогового окна.

1. Создание класса диалогового окна.

1. Подключение [ресурса диалогового окна элементы управления для обработчиков сообщений](../windows/adding-event-handlers-for-dialog-box-controls.md) в классе диалогового окна.

1. Добавление членов данных, связанных с элементами управления диалогового окна, а также для указания [обмен данными диалоговых окон](../mfc/dialog-data-exchange.md) и [проверки данных диалогового окна](../mfc/dialog-data-validation.md) для элементов управления.

## <a name="see-also"></a>См. также

[Диалоговые окна](../mfc/dialog-boxes.md)<br/>
[Жизненный цикл диалогового окна](../mfc/life-cycle-of-a-dialog-box.md)

