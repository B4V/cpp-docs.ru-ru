---
title: Создание новой кнопки панели инструментов (C++) | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-windows
ms.topic: conceptual
f1_keywords:
- vc.editors.toolbar
dev_langs:
- C++
helpviewer_keywords:
- Toolbar editor [C++], creating buttons
- toolbar buttons [C++], button image
- toolbar buttons [C++], creating
- toolbar buttons (in Toolbar editor)
ms.assetid: 46c120fe-4f2a-4887-a08f-bd1fea04b3f4
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
- uwp
ms.openlocfilehash: 8de12d1b421fd78fb9ed2a45cc14826541f72757
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46441699"
---
# <a name="creating-a-new-toolbar-button-c"></a>Создание новой кнопки панели инструментов (C++)

### <a name="to-create-a-new-toolbar-button"></a>Чтобы создать новую кнопку панели инструментов

1. В [представление ресурсов](../windows/resource-view-window.md) разверните папку ресурсов (например, Project1.rc).

   > [!NOTE]
   > Если в проекте еще нет RC-файла, см. раздел [Создание нового файла описания ресурсов](../windows/how-to-create-a-resource-script-file.md).

2. Разверните **инструментов** папку и выберите панель инструментов для редактирования.

3. Назначение идентификатора пустую кнопку в правом конце панели инструментов. Это можно сделать, изменив **идентификатор** свойство в [окно "Свойства"](/visualstudio/ide/reference/properties-window). Например можно предоставить один и тот же идентификатор как пункт меню для кнопки панели инструментов. В этом случае используйте поле с раскрывающимся списком для выбора **идентификатор** пункта меню.

   - или -

   Выберите пустую кнопку в правом конце панели инструментов (в **инструментов представления** области) и начала рисования. Идентификатор команды кнопки по умолчанию назначается (ID_BUTTON\<n >).

Кроме того, можно скопировать и вставить изображение на панель инструментов в качестве новой кнопки.

### <a name="to-add-an-image-to-a-toolbar-as-a-button"></a>Добавление изображения на панель инструментов, как кнопка

1. В [представление ресурсов](../windows/resource-view-window.md), откройте панель инструментов, дважды щелкнув его.

2. Затем откройте образ, который вы хотите добавить на панель инструментов.

   > [!NOTE]
   > При открытии изображения в Visual Studio, он открывается в **изображение** редактора. Можно также открыть изображение в других графических программ.

3. Из **изменить** меню, выберите **копирования**.

4. Переключитесь на панель инструментов, щелкнув вкладку в верхней части окна исходного кода.

5. Из **изменить** меню, выберите **вставить**.

   Изображение будет отображаться на панели инструментов, как новая кнопка.

Сведения о добавлении ресурсов в управляемые проекты см. в разделе [ресурсы в приложениях для настольных систем](/dotnet/framework/resources/index) в *руководства разработчика .NET Framework*. Сведения о вручную добавлять файлы ресурсов в управляемые проекты, осуществлять доступ к ресурсам, отображать статические ресурсы и присваивать строки ресурсов свойствам, см. в разделе [Создание файлов ресурсов для приложений рабочего стола](/dotnet/framework/resources/creating-resource-files-for-desktop-apps). Сведения о глобализации и локализации ресурсов в управляемых приложениях, см. в разделе [Globalizing and Localizing .NET Framework Applications](/dotnet/standard/globalization-localization/index).

## <a name="requirements"></a>Требования

MFC или ATL

## <a name="see-also"></a>См. также

[Свойства кнопок на панели инструментов](../windows/toolbar-button-properties.md)<br/>
[Создание, перемещение и редактирование кнопок на панели инструментов](../windows/creating-moving-and-editing-toolbar-buttons.md)<br/>
[Редактор панелей инструментов](../windows/toolbar-editor.md)