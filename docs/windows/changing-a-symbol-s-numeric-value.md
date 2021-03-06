---
title: Изменение символа&#39;числовое значение s | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-windows
ms.topic: conceptual
f1_keywords:
- vc.editors.symbol.changing.value
dev_langs:
- C++
helpviewer_keywords:
- numeric values
- symbols [C++], numeric values
- numeric values, changing symbols
ms.assetid: 468e903b-9c07-4251-ae09-3b6cb754cc2b
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
- uwp
ms.openlocfilehash: a7b16bb7563bcba3781982952d97b744c0ff86c5
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46403835"
---
# <a name="changing-a-symbol39s-numeric-value"></a>Изменение символа&#39;s числовое значение

Для символов, связанных с одним ресурсом, можно использовать [окно "Свойства"](/visualstudio/ide/reference/properties-window) для изменения значения символа. Можно использовать [символы ресурсов-диалоговое окно](../windows/resource-symbols-dialog-box.md) для изменения значения символов, в настоящее время не назначен ресурс. Дополнительные сведения см. в разделе [изменение неназначенных символов](../windows/changing-unassigned-symbols.md).

### <a name="to-change-a-symbol-value-assigned-to-a-single-resource-or-object"></a>Изменение значения символа, назначенного одному ресурсу или объекту

1. В [представление ресурсов](../windows/resource-view-window.md), выберите ресурс.

   > [!NOTE]
   > Если в проекте еще нет RC-файла, см. раздел [Создание нового файла описания ресурсов](../windows/how-to-create-a-resource-script-file.md).

2. В **свойства** введите имя символа за которым следует знак равенства и целое число в **идентификатор** поле, например:

    ```
    IDC_EDITNAME=5100
    ```

Новое значение будет сохранено в файле символов заголовков при очередном сохранении проекта. В поле "Идентификатор" будет отображаться только имя символа. Знак равенства и значение не будут отображаться после проверки.

Сведения о добавлении ресурсов в управляемые проекты см. в разделе [ресурсы в приложениях для настольных систем](/dotnet/framework/resources/index) в *руководства разработчика .NET Framework*. Сведения о вручную добавлять файлы ресурсов в управляемые проекты, осуществлять доступ к ресурсам отображать статические ресурсы и назначение ресурсов строки свойства.

## <a name="requirements"></a>Требования

Win32

## <a name="see-also"></a>См. также

[Ограничения для символьных значений](../windows/symbol-value-restrictions.md)<br/>
[Стандартные идентификаторы символов](../windows/predefined-symbol-ids.md)