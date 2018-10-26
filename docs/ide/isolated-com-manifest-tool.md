---
title: Свойства изолированной COM для инструмента манифеста (Visual C++) | Документы Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-ide
ms.topic: conceptual
f1_keywords:
- VC.Project.VCManifestTool.RegistrarScriptFile
- VC.Project.VCManifestTool.ComponentFileName
- VC.Project.VCManifestTool.TypeLibraryFile
- VC.Project.VCManifestTool.ReplacementsFile
dev_langs:
- C++
ms.assetid: 457582b8-cfde-49c0-92e3-3a6b9e8c08eb
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: cdb472ce082809a48dd3e42afd4481149eff3a28
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46407562"
---
# <a name="isolated-com-manifest-tool-configuration-properties-ltprojectnamegt-property-pages-dialog-box"></a>Диалоговое окно страниц свойств &lt;Имя_проекта&gt; "Свойства конфигурации", "Инструмент манифеста", "Изолированный COM"

Используйте это диалоговое окно для указания параметров **Изолированный COM** для [Mt.exe](https://msdn.microsoft.com/library/aa375649).

Чтобы открыть это диалоговое окно страницы свойств, откройте страницы свойств для своего проекта или свою страницу свойств. Разверните узел**Инструмент манифеста** в области **Общие свойства**, а затем выберите элемент **Изолированный COM**.

## <a name="task-list"></a>список задач

- [Практическое руководство. Сборка изолированных приложений, использующих компоненты СОМ](../build/how-to-build-isolated-applications-to-consume-com-components.md)

## <a name="uielement-list"></a>Список элементов пользовательского интерфейса

- **Файл библиотеки типов**

   Использует параметр /tlb, чтобы указать имя файла библиотеки типов (TLB-файл), который инструмент манифеста будет использовать для создания файла манифеста.

- **Файл скрипта регистратора**

   Использует параметр /rgs, чтобы указать имя файла скрипта регистратора (RGS-файл), который инструмент манифеста будет использовать для создания файла манифеста.

- **Имя файла компонента**

   Использует параметр /dll, чтобы указать имя ресурса, который инструмент манифеста будет создавать. Для этого свойства нужно ввести значение, если указан параметр **Файл библиотеки типов** или **Файл скрипта регистратора**.

- **Файл замен**

   Использует параметр /replacements, чтобы указать полный путь к файлу, содержащему значения для заменяемых строк в RGS-файле.

## <a name="see-also"></a>См. также

[Изолированные приложения](/windows/desktop/SbsCs/isolated-applications)<br>
[Манифест приложения ClickOnce](/visualstudio/deployment/clickonce-application-manifest)<br>
[Страницы свойств инструмента манифеста](../ide/manifest-tool-property-pages.md)<br>
[Работа со свойствами проектов](../ide/working-with-project-properties.md)