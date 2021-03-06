---
title: Классы общих диалоговых окон OLE | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-mfc
ms.topic: conceptual
f1_keywords:
- vc.classes.ole
dev_langs:
- C++
helpviewer_keywords:
- ActiveX classes [MFC]
- dialog classes [MFC], OLE
- OLE common dialog classes [MFC]
- common dialog classes [MFC]
ms.assetid: 706526ae-f94f-4909-a0f8-6b5fe954fd97
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: c6ef5a7aed288331322243d316dde58d9f36cbd9
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46430427"
---
# <a name="ole-common-dialog-classes"></a>Классы общих диалоговых окон OLE

Эти классы выполнения общих задач OLE, реализовав ряд стандартных диалоговых окон OLE. Они также обеспечивают единый пользовательский интерфейс для функциональных возможностей OLE.

[COleDialog](../mfc/reference/coledialog-class.md)<br/>
Используется платформой для хранения реализаций для всех диалоговых окон OLE. Все классы диалоговых окон в категории пользовательского интерфейса являются производными от этого базового класса. `COleDialog` нельзя использовать напрямую.

[COleInsertDialog](../mfc/reference/coleinsertdialog-class.md)<br/>
Отображаются диалоговом окне Вставка объекта в стандартный пользовательский интерфейс для вставки новых OLE связанных или внедренных элементов.

[COlePasteSpecialDialog](../mfc/reference/colepastespecialdialog-class.md)<br/>
Отображает Специальная вставка диалоговое окно, стандартный пользовательский интерфейс для реализации Специальная вставка команды.

[COleLinksDialog](../mfc/reference/colelinksdialog-class.md)<br/>
Отображает диалоговое окно Изменение связей, стандартный пользовательский интерфейс для изменения сведений о связанных элементах.

[COleChangeIconDialog](../mfc/reference/colechangeicondialog-class.md)<br/>
Отображает диалоговое окно Смена значка, стандартный пользовательский интерфейс для изменения значка, связанного с OLE-внедренные или связанный элемент.

[COleConvertDialog](../mfc/reference/coleconvertdialog-class.md)<br/>
Отображает диалоговое окно Convert, стандартный пользовательский интерфейс для преобразования элементов OLE из одного типа в другой.

[COlePropertiesDialog](../mfc/reference/colepropertiesdialog-class.md)<br/>
Инкапсулирует диалоговое окно общих свойств OLE Windows. Общие диалоговые окна свойств OLE предоставляют простой способ отображения и изменения свойств элемента документа OLE в соответствии со стандартами Windows.

[COleUpdateDialog](../mfc/reference/coleupdatedialog-class.md)<br/>
Отображает диалоговое окно обновления стандартный пользовательский интерфейс для обновления всех ссылок в документе. Диалоговое окно содержит индикатор хода выполнения, чтобы указать, насколько близко процедуры обновления является до завершения.

[COleChangeSourceDialog](../mfc/reference/colechangesourcedialog-class.md)<br/>
Отображает диалоговое окно Изменить источник, стандартный пользовательский интерфейс для изменения назначения или источника связи.

[COleBusyDialog](../mfc/reference/colebusydialog-class.md)<br/>
Отображает сервер занят диалоговые окна и сервер не отвечает, стандартный пользовательский интерфейс для обработки вызовов занят приложений. Обычно отображается автоматически `COleMessageFilter` реализации.

## <a name="see-also"></a>См. также

[Общие сведения о классе](../mfc/class-library-overview.md)

