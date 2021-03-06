---
title: С помощью MFC исходные файлы | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-mfc
ms.topic: conceptual
dev_langs:
- C++
helpviewer_keywords:
- public members
- source files
- MFC, source files
- MFC source files
- comments, MFC
- private member access
- protected member access
- source files, MFC
ms.assetid: 3230e8fb-3b69-4ddf-9538-365ac7ea5e72
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: e63383e372227dc14ce90843b03b6cb0c029b52a
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46383861"
---
# <a name="using-the-mfc-source-files"></a>Использование файлов с исходным кодом MFC

Библиотека Microsoft Foundation Class (MFC) предоставляет полный исходный код. Файлы заголовков (.h) находятся в каталоге \atlmfc\include; файлы реализации (.cpp) находятся в каталоге \atlmfc\src\mfc.

Этот сборник статей объясняет условные обозначения, MFC использует преобразовывать в комментарии различные части каждого класса, что означают эти комментарии и следует ожидать для поиска в каждом разделе. Мастера Visual C++ используют аналогичные соглашения для классов, которые они создают для вас, и можно обнаружить эти соглашения полезны для вашего кода.

Вы можете быть знакомы с **открытый**, **защищенные**, и **частного** ключевые слова C++. Если взглянуть на файлах заголовков MFC, вы обнаружите, что каждый класс может иметь несколько каждого из них. Например, может быть открытый член переменных и функций в более чем одном **открытый** ключевое слово. Это обусловлено MFC разделяет переменные-члены и функции в зависимости от их использования не по типу доступа. MFC использует **частного** минимально; даже те элементы считаются детали реализации, обычно защищены и зачастую являются открытыми. Несмотря на то, что доступ к деталям реализации, не рекомендуется, MFC оставляет решение для вас.

В исходных файлах MFC и файлы, которые создает мастер приложений MFC вы найдете комментарии этих функций в объявлениях классов (обычно в указанном порядке):

`// Constructors`

`// Attributes`

`// Operations`

`// Overridables`

`// Implementation`

В этот сборник статей рассматриваются:

- [Пример комментариев](../mfc/an-example-of-the-comments.md)

- [/ / Комментарий реализации](../mfc/decrement-implementation-comment.md)

- [/ / Комментарий конструкторов](../mfc/decrement-constructors-comment.md)

- [/ / Комментарий атрибутов](../mfc/decrement-attributes-comment.md)

- [/ / Комментарий операций](../mfc/decrement-operations-comment.md)

- [/ / Комментарий Переопределяемости](../mfc/decrement-overridables-comment.md)

## <a name="see-also"></a>См. также

[Общие разделы по MFC](../mfc/general-mfc-topics.md)

