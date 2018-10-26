---
title: Страница свойств управляемых ресурсов | Документы Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-ide
ms.topic: conceptual
f1_keywords:
- VC.Project.VCManagedResourceCompilerTool.ResourceFileName
- VC.Project.VCManagedResourceCompilerTool.OutputFileName
- VC.Project.VCManagedResourceCompilerTool.DefaultLocalizedResources
dev_langs:
- C++
helpviewer_keywords:
- Managed Resources property page
ms.assetid: 80b80384-ee55-494d-9f0e-907bb98cfc19
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 687203787bdab69751aabf0672fe1269974b3014
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46399613"
---
# <a name="managed-resources-property-page"></a>страница свойств управляемых ресурсов

Включает параметры для компилятора ресурсов.

Страница свойств **Управляемые ресурсы** содержит следующие свойства.

- **Логическое имя ресурса**

   Указывает *логическое имя* для созданного промежуточного файла RESOURCES. Логическое имя используется для загрузки ресурса. Если логическое имя не указано, вместо него используется имя файла ресурсов (RESX).

- **Имя выходного файла**

   Указывает имя окончательного выходного файла, в который направляется этот файл ресурсов (RESX).

- **Локализованные ресурсы по умолчанию**

   Указывает, направляется ли данный файл RESX в ресурсы по умолчанию либо во вспомогательную библиотеку DLL.

Сведения о доступе к страницам свойств **Управляемые ресурсы** см. в разделе [Работа со свойствами проектов](../ide/working-with-project-properties.md).

## <a name="see-also"></a>См. также

[Использование компилятора ресурсов (командная строка RC)](/windows/desktop/menurc/using-rc-the-rc-command-line-)<br>
[Страницы свойств](../ide/property-pages-visual-cpp.md)<br>
[/ASSEMBLYRESOURCE (внедрение управляемого ресурса)](../build/reference/assemblyresource-embed-a-managed-resource.md)