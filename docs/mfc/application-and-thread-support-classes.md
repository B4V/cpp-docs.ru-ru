---
title: Приложения и поток поддержки классов | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-mfc
ms.topic: conceptual
f1_keywords:
- vc.classes.support
dev_langs:
- C++
helpviewer_keywords:
- application objects [MFC], thread support classes
- lock classes [MFC]
- thread support classes [MFC]
- threading [MFC]
- synchronization classes [MFC], multithreading
- application support classes [MFC]
ms.assetid: 3c1d14fd-c35c-48f1-86ce-1e0f9a32c36d
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: ce9c799c8dbc2a98c7d45dfa9a2e444024c9a7a2
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46412327"
---
# <a name="application-and-thread-support-classes"></a>Классы поддержки приложений и потоков

Каждое приложение имеет только один объект приложения; Этот объект координирует другими объектами в выполняющейся программе и является производным от `CWinApp`.

Библиотека Microsoft Foundation Class (MFC) поддерживает несколько потоков выполнения в приложении. Все приложения должны иметь хотя бы один поток; поток, используемый вашей `CWinApp` объект является этот основной поток.

`CWinThread` Инкапсулирует часть возможностей потоков операционной системы. Чтобы сделать использование нескольких потоков, MFC также обеспечивает синхронизацию классы объектов для обеспечения интерфейса C++, для объектов синхронизации Win32.

## <a name="application-and-thread-classes"></a>Классы приложений и потоков

[CWinApp](../mfc/reference/cwinapp-class.md)<br/>
Инкапсулирует код для инициализации, запуска и завершения работы приложения. Объект приложения будет наследовать от этого класса.

[CWinThread](../mfc/reference/cwinthread-class.md)<br/>
Базовый класс для всех потоков. Использовать непосредственно или являются производными от класса `CWinThread` Если поток выполняет функции пользовательского интерфейса. Класс `CWinApp` является производным от `CWinThread`.

## <a name="synchronization-object-classes"></a>Классы объектов синхронизации

[CSyncObject](../mfc/reference/csyncobject-class.md)<br/>
Базовый класс для классов объектов синхронизации.

[CCriticalSection](../mfc/reference/ccriticalsection-class.md)<br/>
Класс синхронизации, который позволяет только один поток в одном процессе для доступа к объекту.

[CSemaphore](../mfc/reference/csemaphore-class.md)<br/>
Класс синхронизации, который позволяет от одного до указанное максимальное количество одновременных обращений к объекту.

[CMutex](../mfc/reference/cmutex-class.md)<br/>
Класс синхронизации, который позволяет только один поток в любое количество процессов для доступа к объекту.

[CEvent](../mfc/reference/cevent-class.md)<br/>
Класс синхронизации, который уведомляет приложение о том, когда произошло событие.

[Класс CSingleLock](../mfc/reference/csinglelock-class.md)<br/>
Используется в функции-члены потокобезопасные классы для блокировки на один объект синхронизации.

[CMultiLock](../mfc/reference/cmultilock-class.md)<br/>
Используется в функции-члены потокобезопасные классы для блокировки на один или несколько объектов синхронизации, расположенные в массиве объектов синхронизации.

## <a name="related-classes"></a>Связанные классы

[CCommandLineInfo](../mfc/reference/ccommandlineinfo-class.md)<br/>
Выполняет синтаксический анализ командной строки, с которой запущена программа.

[CWaitCursor](../mfc/reference/cwaitcursor-class.md)<br/>
Помещает курсор ожидания на экране. Используется во время длительных операций.

[CDockState](../mfc/reference/cdockstate-class.md)<br/>
Обрабатывает постоянного хранения закрепление данные о состоянии для панелей элементов управления.

[CRecentFileList](../mfc/reference/crecentfilelist-class.md)<br/>
Поддерживает наиболее часто используемое список файлов (MRU).

## <a name="see-also"></a>См. также

[Общие сведения о классе](../mfc/class-library-overview.md)

