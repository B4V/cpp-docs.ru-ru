---
title: Последовательность операций для создания приложений OLE | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-mfc
ms.topic: conceptual
dev_langs:
- C++
helpviewer_keywords:
- OLE applications [MFC], creating
- OLE applications [MFC]
- applications [OLE], creating
- applications [OLE]
ms.assetid: 84b0f606-36c1-4253-9cea-44427f0074b9
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 02542f8a4eb382ff4d7a88f98163b0052be09f75
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46392527"
---
# <a name="sequence-of-operations-for-creating-ole-applications"></a>Последовательность операций для создания приложений OLE

Следующая таблица показывает роль и роль платформы при создании OLE связь и внедрение приложений. Они представляют собой параметры доступны, а не последовательность шагов для выполнения.

### <a name="creating-ole-applications"></a>Создания приложений OLE

|Задача|Вы|Платформы|
|----------|------------|------------------------|
|Создание COM-компонента.|Запустите мастер приложений MFC. Выберите **полносерверные** или **минисерверные** в **поддержка составных документов** вкладки.|Платформа создает скелет приложения с включенной возможностью компонент COM. Все возможности COM могут передаваться в существующее приложение с помощью только внести небольшие изменения.|
|Создание приложения-контейнера с нуля.|Запустите мастер приложений MFC. Выберите **контейнера** в **поддержка составных документов** вкладки. С помощью представления класса, перейдите к редактора исходного кода. Введите код для функций COM обработчика.|Платформа создает скелет приложения, которое можно вставить COM-объекты, создаваемые приложениями COM компонента (сервер).|
|Создайте приложение с поддержкой автоматизации с нуля.|Запустите мастер приложений MFC. Выберите **автоматизации** из **дополнительные функции** вкладки. Используйте представление класса для предоставляют методы и свойства приложения для автоматизации.|Платформа создает скелет приложения, которое можно активировать и автоматизировать за счет других приложений.|

## <a name="see-also"></a>См. также

[Сборка в платформе](../mfc/building-on-the-framework.md)<br/>
[Последовательность операций для сборки приложений MFC](../mfc/sequence-of-operations-for-building-mfc-applications.md)<br/>
[Последовательность операций при создании элементов управления ActiveX](../mfc/sequence-of-operations-for-creating-activex-controls.md)<br/>
[Последовательность операций для создания приложений баз данных](../mfc/sequence-of-operations-for-creating-database-applications.md)

