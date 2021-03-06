---
title: Установка курсора&#39;гиперобъект s (редактор изображений для значков) | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-windows
ms.topic: conceptual
f1_keywords:
- vc.editors.image.editing
dev_langs:
- C++
helpviewer_keywords:
- cursors [C++], hot spots
- hot spots
ms.assetid: a610388a-45c8-43cd-98a2-fd31f29238b8
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
- uwp
ms.openlocfilehash: 9246d7a26c9764e31cca9c861ec0a15d4792c115
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46389102"
---
# <a name="setting-a-cursor39s-hot-spot-image-editor-for-icons"></a>Установка курсора&#39;гиперобъект s (редактор изображений для значков)

Активная точка [курсор](../windows/icons-and-cursors-image-resources-for-display-devices-image-editor-for-icons.md) представляет собой точку на которую ссылается Windows при отслеживании позиции курсора. По умолчанию активная точка будет присвоено верхнего левого угла курсора (координаты 0,0). **Хот-Спот** свойство в [окно "Свойства"](/visualstudio/ide/reference/properties-window) координаты активной точки отображаются.

### <a name="to-set-a-cursors-hot-spot"></a>Чтобы задать активной точки курсора

1. На [панель инструментов редактора изображений](../windows/toolbar-image-editor-for-icons.md), нажмите кнопку **задать активную зону** средство.

2. Щелкните пикселей, которые вы хотите назначить в качестве активной точки указателя мыши.

   **Хот-Спот** свойство в **свойства** окно отображает новые координаты.

   > [!TIP]
   > Всплывающие подсказки отображаются при наведении курсора на кнопку панели инструментов. Эти советы помогут определить назначение каждой кнопки.

Сведения о добавлении ресурсов в управляемые проекты см. в разделе [ресурсы в приложениях для настольных систем](/dotnet/framework/resources/index) в *руководства разработчика .NET Framework*. Сведения о вручную добавлять файлы ресурсов в управляемые проекты, осуществлять доступ к ресурсам, отображать статические ресурсы и присваивать строки ресурсов свойствам, см. в разделе [Создание файлов ресурсов для приложений рабочего стола](/dotnet/framework/resources/creating-resource-files-for-desktop-apps). Сведения о глобализации и локализации ресурсов в управляемых приложениях, см. в разделе [Globalizing and Localizing .NET Framework Applications](/dotnet/standard/globalization-localization/index).

## <a name="requirements"></a>Требования

Нет

## <a name="see-also"></a>См. также

[Сочетания клавиш](../windows/accelerator-keys-image-editor-for-icons.md)<br/>
[Значки и курсоры: ресурсы изображений для устройств отображения](../windows/icons-and-cursors-image-resources-for-display-devices-image-editor-for-icons.md)