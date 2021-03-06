---
title: 'Практическое: Настройка панели быстрого доступа | Документация Майкрософт'
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-mfc
ms.topic: conceptual
dev_langs:
- C++
helpviewer_keywords:
- quick access toolbar [MFC], customization
ms.assetid: 2554099b-0c89-4605-9249-31bf9cbcefe0
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 0f3ec14971b69788892690c26ef2759f3b35d55f
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46419110"
---
# <a name="how-to-customize-the-quick-access-toolbar"></a>Практическое руководство. Настройка панели быстрого доступа

Панель инструментов быстрого доступа (QAT) — это настраиваемая панель инструментов, который содержит набор команд, которые являются либо отображается рядом с кнопкой приложения или на вкладках категории. Ниже показан типичный быстрого доступа.

![Панель быстрого доступа ленты MFC](../mfc/media/quick_access_toolbar.png "quick_access_toolbar")

Чтобы настроить панель быстрого доступа, откройте его в **свойства** окна, измените его команды, а затем просмотреть элемент управления на ленте.

### <a name="to-open-the-quick-access-toolbar-in-the-properties-window"></a>Чтобы открыть панель быстрого доступа в окне «Свойства»

1. В Visual Studio на **представление** меню, щелкните **представление ресурсов**.

1. В **представление ресурсов**, дважды щелкните ресурс ленты, чтобы отобразить ее в рабочей области конструирования.

1. В области конструктора щелкните правой кнопкой мыши в меню быстрого доступа и нажмите кнопку **свойства**.

## <a name="quick-access-toolbar-properties"></a>Свойства панели инструментов быстрого доступа

Следующая таблица определяет свойства быстрого доступа.

|Свойство.|Определение|
|--------------|----------------|
|Положение QAT|Задает положение панели быстрого доступа, при запуске приложения. Положение может быть либо **выше** или **ниже** элемент управления на ленте.|
|Элементы QAT|Задает команды, доступные для быстрого доступа.|

#### <a name="to-add-or-remove-commands-on-the-quick-access-toolbar"></a>Чтобы добавить или удалить команды из панели быстрого доступа

1. В **свойства** окно, нажмите кнопку **элементы QAT**, а затем нажмите кнопку с многоточием **(...)** .

1. В **редактор элементов QAT** диалоговом окне **добавить** и **удалить** кнопки для изменения списка команд на панели инструментов быстрого доступа.

1. Если требуется, чтобы команда на панели быстрого доступа и в меню быстрого доступа, выберите поле рядом с командой. Если требуется, чтобы команда появилась только в меню, снимите флажок.

## <a name="previewing-the-ribbon"></a>Предварительный просмотр ленты

Быстрые команды панели доступа не отображаются в области конструктора. Чтобы просмотреть их, необходимо просмотреть ленту или запустить приложение.

#### <a name="to-preview-the-ribbon-control"></a>Для предварительного просмотра элемента управления ленты

- На **панели инструментов редактора ленты**, нажмите кнопку **проверить ленту**.

## <a name="see-also"></a>См. также

[Конструктор ленты (MFC)](../mfc/ribbon-designer-mfc.md)

