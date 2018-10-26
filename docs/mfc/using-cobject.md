---
title: Использование CObject | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-mfc
ms.topic: conceptual
f1_keywords:
- CObject
dev_langs:
- C++
helpviewer_keywords:
- examples [MFC], CObject
- root base class for MFC
- derived classes [MFC], from CObject
- MFC, base class
- CObject class [MFC]
ms.assetid: d0cd19bb-2856-4b41-abbc-620fd64cb223
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 734f9f66a37828b1fed04fc5366dd545e6c5e370
ms.sourcegitcommit: 3a141cf07b5411d5f1fdf6cf67c4ce928cf389c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/11/2018
ms.locfileid: "49082193"
---
# <a name="using-cobject"></a>Использование CObject

[CObject](../mfc/reference/cobject-class.md) является корневой базовый класс для большинства из Microsoft Foundation Class Library (MFC). `CObject` Класс содержит множество полезных функций, которые можно внедрить в собственные объекты программы, включая поддержку сериализации, сведения о классе среды выполнения и диагностических выходных данных объекта. Если вы наследуете от класса `CObject`, ваш класс может использовать эти `CObject` функции.

## <a name="what-do-you-want-to-do"></a>Что Вы хотите делать

- [Создать класс, производный от CObject](../mfc/deriving-a-class-from-cobject.md)

- [Добавить поддержку сведения о классе среды выполнения, динамическое создание и сериализации для моего производного класса](../mfc/specifying-levels-of-functionality.md)

- [Сведения о классе во время выполнения доступ](../mfc/accessing-run-time-class-information.md)

- [Динамическое создание объектов](../mfc/dynamic-object-creation.md)

- [Дамп объекта данных для диагностики](/previous-versions/visualstudio/visual-studio-2010/sc15kz85)

- Проверка внутреннего состояния объекта (см. в разделе [MFC ASSERT_VALID и CObject::AssertValid](reference/diagnostic-services.md#assert_valid))

- [Класс сериализоваться в постоянное хранилище](../mfc/serialization-in-mfc.md)

- Просмотреть список [CObject часто задаваемые вопросы](../mfc/cobject-class-frequently-asked-questions.md)

## <a name="see-also"></a>См. также

[Основные понятия](../mfc/mfc-concepts.md)<br/>
[Общие разделы по MFC](../mfc/general-mfc-topics.md)<br/>
[Структура CRuntimeClass](../mfc/reference/cruntimeclass-structure.md)<br/>
[Файлы](../mfc/files-in-mfc.md)<br/>
[Сериализация](../mfc/serialization-in-mfc.md)

