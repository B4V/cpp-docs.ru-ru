---
title: Мастер приложений Win32 | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-windows
ms.topic: conceptual
f1_keywords:
- vc.appwiz.win32.overview
dev_langs:
- C++
helpviewer_keywords:
- Win32 Application Wizard
- Win32 Project Wizard
ms.assetid: 5d7b3a5e-8461-479a-969a-67b7883725b9
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
- uwp
ms.openlocfilehash: 26282ef73f6a979cd564bd7597f8418c6535179a
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46390523"
---
# <a name="win32-application-wizard"></a>мастер приложений Win32

Мастер приложений Win32 Visual C++ позволяет создавать любой из четырех типов проектов (указаны в заголовке таблицы ниже). В каждом случае можно указать дополнительные параметры, подходящие для открытого вами типа проекта. В таблице ниже показано, какие параметры доступны для каждого типа приложения.

|Тип поддержки|Консольное приложение|Исполняемое приложение (Windows)|Библиотека динамической компоновки|Статическая библиотека|
|---------------------|-------------------------|----------------------------------------|---------------------------|--------------------|
|**Пустой проект**|Да|Да|Да|Нет|
|**Символы экспорта**|Нет|Нет|Да|Нет|
|**Предкомпилированный заголовок**|Нет|Нет|Нет|Да|
|**поддержка ATL**|Да|Нет|Нет|Нет|
|**поддержка MFC**|Да|Нет|Нет|Да|

## <a name="overview"></a>Обзор

На этой странице мастера описываются текущие параметры проекта для создаваемого приложения Win32. По умолчанию заданы следующие параметры:

- проект является приложением Windows;

- проект не пустой;

- проект не содержит символов экспорта;

- проект не использует файл предкомпилированного заголовка (этот параметр доступен только для проектов статической библиотеки);

- проект не включает поддержку MFC и ATL.

Чтобы изменить эти значения по умолчанию, перейдите на вкладку [Параметры приложения](../windows/application-settings-win-32-project-wizard.md) в левом столбце мастера и внесите необходимые изменения.

Создав классическое приложение Windows, можно добавить универсальные классы C++ с помощью мастера [универсального](../ide/generic-cpp-class-wizard.md) кода. Можно добавить другие элементы, такие как файлы HTML, файлы заголовков, ресурсы или текстовые файлы.

> [!NOTE]
> Классы ATL добавить нельзя, а классы MFC можно добавить только в те типы классических приложений Windows, которые поддерживают MFC (см. предыдущую таблицу).

Файлы, созданные мастером для проекта, можно просмотреть в **обозревателе решений**. Дополнительные сведения о файлах, мастер создает для проекта, см. в файле, созданном для проекта `ReadMe.txt`. Дополнительные сведения о типах файлов см. в разделе [Типы файлов, создаваемых для проектов Visual C++](../ide/file-types-created-for-visual-cpp-projects.md).

## <a name="see-also"></a>См. также

[Создание пустого классического приложения Windows](../windows/creating-an-empty-windows-desktop-application.md)<br/>
[Типы проектов Visual C++](../ide/visual-cpp-project-types.md)