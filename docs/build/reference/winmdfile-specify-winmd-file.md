---
title: -WINMDFILE (указание файла winmd) | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-tools
ms.topic: reference
f1_keywords:
- VC.Project.VCLinkerTool.GenerateWindowsMetadataFile
dev_langs:
- C++
ms.assetid: 062b41b3-14d6-432c-a361-fdb66e918931
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: d34bdfd2d80690efae8efbc1f95ba0c50a530af3
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46425788"
---
# <a name="winmdfile-specify-winmd-file"></a>/WINMDFILE (укажите файл winmd)

Задает имя файла для выходного файла метаданных среды выполнения Windows (.winmd), созданного [/WINMD](../../build/reference/winmd-generate-windows-metadata.md) параметр компоновщика.

```
/WINMDFILE:filename
```

## <a name="remarks"></a>Примечания

Используйте значение, которое указано в `filename` для переопределения используемого по умолчанию имя файла .winmd (`binaryname`.winmd). Обратите внимание на то, что вы не добавляете «.winmd» `filename`.  Если несколько значений в списке на **/WINMDFILE** командной строки, последний имеет приоритет.

### <a name="to-set-this-linker-option-in-the-visual-studio-development-environment"></a>Задание данного параметра компоновщика в среде разработки Visual Studio

1. Откройте диалоговое окно **Страницы свойств** проекта. Дополнительные сведения см. в разделе [Работа со свойствами проекта](../../ide/working-with-project-properties.md).

1. Выберите **компоновщика** папки.

1. Выберите **метаданных Windows** страницу свойств.

1. В **файл метаданных Windows** введите нужный файл.

## <a name="see-also"></a>См. также

[/WINMD (создание метаданных Windows)](../../build/reference/winmd-generate-windows-metadata.md)<br/>
[Настройка параметров компоновщика](../../build/reference/setting-linker-options.md)<br/>
[Параметры компоновщика](../../build/reference/linker-options.md)