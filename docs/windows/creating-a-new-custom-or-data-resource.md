---
title: Создание нового настраиваемого ресурса или ресурса данных (C++) | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-windows
ms.topic: conceptual
f1_keywords:
- vc.editors.binary
dev_langs:
- C++
helpviewer_keywords:
- custom resources [C++]
- data resources [C++]
- resources [C++], creating
ms.assetid: 9918bf96-38fa-43a1-a384-572f95d84950
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
- uwp
ms.openlocfilehash: 2e2939c7f0a68401b4c1a8c43b5c6335a0acfcb3
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46403948"
---
# <a name="creating-a-new-custom-or-data-resource-c"></a>Создание нового настраиваемого ресурса или ресурса данных (C++)

Можно создать новый ресурс настраиваемого ресурса или данных, можно разместить ресурс в отдельном файле с помощью обычного синтаксиса скрипта ресурсов (.rc) файла, а затем включить этот файл правой кнопкой мыши проект в **обозревателе решений** и щелкнув  **Включает ресурсов** в контекстном меню.

### <a name="to-create-a-new-custom-or-data-resource"></a>Создание настраиваемого ресурса или ресурса данных

1. [Создайте RC-файл](../windows/how-to-create-a-resource-script-file.md) , который содержит настраиваемый ресурс или ресурс данных.

   Пользовательские данные можно ввести в RC-файл в виде строк в кавычках, заканчивающихся символом null, или как целочисленные значения в десятичном, шестнадцатеричном или восьмеричном формате.

2. В **обозревателе решений**щелкните правой кнопкой мыши RC-файл проекта, а затем выберите в контекстном меню пункт **Включения ресурсов** .

3. В **директивы времени компиляции** введите `#include` инструкцию, которая предоставляет имя файла, содержащего настраиваемый ресурс. Пример:

    ```cpp
    #include mydata.rc
    ```

   Проверьте синтаксис и орфографию введенных данных. Содержимое поля **Директивы времени компиляции** будет добавляться в файл описания ресурсов в том виде, в каком оно было введено вами.

4. Нажмите кнопку **ОК** , чтобы записать внесенные изменения.

Настраиваемый ресурс также можно создать другим способом — импортировав внешний файл. Дополнительные сведения см. в разделе [Импорт и экспорт ресурсов](../windows/how-to-import-and-export-resources.md).

Сведения о добавлении ресурсов в управляемые проекты см. в разделе [ресурсы в приложениях для настольных систем](/dotnet/framework/resources/index) в *руководства разработчика .NET Framework*. Сведения о вручную добавлять файлы ресурсов в управляемые проекты, осуществлять доступ к ресурсам, отображать статические ресурсы и присваивать строки ресурсов свойствам, см. в разделе [Создание файлов ресурсов для приложений рабочего стола](/dotnet/framework/resources/creating-resource-files-for-desktop-apps). Сведения о глобализации и локализации ресурсов в управляемых приложениях, см. в разделе [Globalizing and Localizing .NET Framework Applications](/dotnet/standard/globalization-localization/index).

## <a name="requirements"></a>Требования

Win32

## <a name="see-also"></a>См. также

[Binary Editor](binary-editor.md)