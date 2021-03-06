---
title: 'Практическое: Импорт и экспорт ресурсов (C++) | Документация Майкрософт'
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-windows
ms.topic: conceptual
f1_keywords:
- vs.resvw.resource.importing
- vc.resvw.resource.importing
dev_langs:
- C++
helpviewer_keywords:
- resources [C++], exporting
- graphics [C++], exporting
- graphics [C++], importing
- resources [C++], importing
- bitmaps [C++], importing and exporting
- toolbars [C++], importing
- images [C++], importing
- toolbars [C++], exporting
- cursors [C++], importing and exporting
- images [C++], exporting
ms.assetid: 3c9329dc-dcb8-4edd-a600-78e3e572bd89
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
- uwp
ms.openlocfilehash: e2fcbd51e472614104cd74df4bf5697512a2e0df
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46419441"
---
# <a name="how-to-import-and-export-resources"></a>Практическое руководство. Импорт и экспорт ресурсов

Графические ресурсы (растровые изображения, значки, курсоры, панели инструментов), HTML-файлы и пользовательские ресурсы можно импортировать для использования в Visual C++. Эти же типы ресурсов можно экспортировать из проекта Visual C++ в виде отдельных файлов, которые можно использовать за пределами среды разработки.

> [!NOTE]
> Такие типы ресурсов, как сочетания клавиш, диалоговые окна и таблицы строк, нельзя импортировать или экспортировать, поскольку они не являются типами отдельных файлов.

### <a name="to-import-an-individual-resource-into-your-current-resource-file"></a>Импорт отдельного ресурса в текущий файл ресурса

1. В [представление ресурсов](../windows/resource-view-window.md), щелкните правой кнопкой мыши узел описания ресурсов (* .rc) файла, к которому вы хотите добавить ресурс.

2. Нажмите кнопку **импорта** в контекстном меню.

3. Найдите и выберите файл растрового изображения (.bmp), значка (.ico), курсора (.cur), HTML-файл (.htm) или другой файл, который требуется импортировать.

4. Нажмите кнопку **ОК** для добавления ресурса в выбранный файл в **ресурсов** представления.

   > [!NOTE]
   > Процедура импорта выполняется одинаково независимо от конкретного типа выбранного ресурса. Импортированный ресурс автоматически добавляется в соответствующий узел для этого типа ресурса.

### <a name="to-export-a-bitmap-icon-or-cursor-as-a-separate-file-for-use-outside-of-visual-c"></a>Экспорт растрового изображения, значка или курсора в отдельный файл (для использования за пределами Visual C++)

1. В **ресурсов** просмотра, щелкните правой кнопкой мыши ресурс, который вы хотите экспортировать.

2. Нажмите кнопку **Экспорт** в контекстном меню.

3. В **Экспорт ресурса** диалогового окна поле примите текущее имя файла или введите новое.

4. Перейдите к папке, где вы хотите сохранить файл и нажмите кнопку **Экспорт**.

## <a name="requirements"></a>Требования

Win32

## <a name="see-also"></a>См. также

[Файлы ресурсов](../windows/resource-files-visual-studio.md)<br/>
[Редакторы ресурсов](../windows/resource-editors.md)