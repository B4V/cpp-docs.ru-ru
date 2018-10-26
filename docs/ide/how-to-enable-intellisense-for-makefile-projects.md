---
title: Практическое руководство. Использование IntelliSense для проекта makefile | Документы Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-ide
ms.topic: conceptual
f1_keywords:
- VC.Project.VCNMakeTool.IntelliSense
dev_langs:
- C++
helpviewer_keywords:
- Makefile projects, IntelliSense
- IntelliSense, Makefile projects
ms.assetid: 9443f453-f18f-4f12-a9a1-ef9dbf8b188f
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 1dda7b485c5aef7b6277da3141f293e16ac7523b
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46433729"
---
# <a name="how-to-enable-intellisense-for-makefile-projects"></a>Практическое руководство. Использование IntelliSense для проекта Makefile

IntelliSense не работает в интегрированной среде разработки для проектов makefile Visual C++, если определенные параметры проекта или компилятора заданы неправильно. Эта процедура позволяет настроить проекты makefile Visual C++, чтобы технология IntelliSense работала при открытии проектов makefile в среде разработки Visual Studio.

### <a name="to-enable-intellisense-for-makefile-projects-in-the-ide"></a>Включение IntelliSense для проектов makefile в интегрированной среде разработки

1. Откройте диалоговое окно **Страницы свойств**. Дополнительные сведения см. в разделе [Работа со свойствами проекта](../ide/working-with-project-properties.md).

1. Разверните узел **Свойства конфигурации**.

1. Выберите страницу свойств **NMake** и соответствующим образом измените свойства в разделе **IntelliSense**.

   - Задайте свойство **Определения препроцессора**, чтобы определить символы препроцессора в проекте makefile. Дополнительные сведения см. в разделе [/D (определения препроцессора)](../build/reference/d-preprocessor-definitions.md).

   - Задайте свойство **Путь поиска включаемых файлов**, чтобы указать список каталогов, где компилятор будет производить поиск для разрешения ссылок на файлы, передаваемых в директивы препроцессора в новом проекте makefile. Дополнительные сведения см. в разделе [/I (дополнительные каталоги включения)](../build/reference/i-additional-include-directories.md).

         For projects that are built using CL.EXE from a Command Window, set the **INCLUDE** environment variable to specify directories that the compiler will search to resolve file references that are passed to preprocessor directives in your makefile project.

   - Задайте свойство **Принудительно включаемые файлы**, чтобы указать файлы заголовков, обрабатываемые при сборке проекта makefile. Дополнительные сведения см. в разделе [/FI (имя принудительно включаемого файла)](../build/reference/fi-name-forced-include-file.md).

   - Задайте свойство **Путь поиска сборок**, чтобы указать список каталогов, где компилятор будет производить поиск для разрешения ссылок на сборки .NET в проекте. Дополнительные сведения см. в разделе [/AI (указание каталогов метаданных)](../build/reference/ai-specify-metadata-directories.md).

   - Задайте свойство **Обязательно используемые сборки**, чтобы указать, какие сборки .NET обрабатываются при сборке проекта makefile. Дополнительные сведения см. в разделе [/FU (именование файла с принудительно используемым атрибутом #using)](../build/reference/fu-name-forced-hash-using-file.md).

   - Задайте свойство **Дополнительные параметры**, чтобы указать дополнительные параметры компилятора, которые должны использоваться IntelliSense при анализе файлов C++.

1. Нажмите кнопку **ОК**, чтобы закрыть страницы свойств.

1. Используйте команду **Сохранить все**, чтобы сохранить измененные параметры проекта.

При следующем открытии проекта makefile в среде разработки Visual Studio запустите команду **Очистить решение**, а затем — команду **Собрать решение** для проекта makefile. Технология IntelliSense должна работать в интегрированной среде разработки правильно.

## <a name="see-also"></a>См. также

[Использование технологии IntelliSense](/visualstudio/ide/using-intellisense)<br>
[Справочник по программе NMAKE](../build/nmake-reference.md)<br>
[Практическое руководство. Создание проекта C++ из существующего кода](../ide/how-to-create-a-cpp-project-from-existing-code.md)