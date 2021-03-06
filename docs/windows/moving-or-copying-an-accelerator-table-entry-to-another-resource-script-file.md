---
title: Перемещение или копирование элемента таблицы сочетаний клавиш в другой файл описания ресурсов (C++) | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-windows
ms.topic: conceptual
dev_langs:
- C++
helpviewer_keywords:
- accelerator tables [C++], copying entries
- rc files [C++], moving an accelerator table entry
- .rc files [C++], moving accelerator table entries
- accelerator tables [C++], moving entries
ms.assetid: 7b4dc149-c972-4ab2-8477-76c52b6feb5b
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
- uwp
ms.openlocfilehash: 0d3f75ef8c2820c227716e3208ff2cded54d1fd7
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46414736"
---
# <a name="moving-or-copying-an-accelerator-table-entry-to-another-resource-script-file-c"></a>Перемещение или копирование элемента таблицы сочетаний клавиш в другой файл описания ресурсов (C++)

### <a name="to-move-or-copy-an-accelerator-table-entry-to-another-resource-script-file"></a>Перемещение или копирование записи таблицы сочетаний клавиш в другой файл описания ресурсов

1. Откройте таблицы сочетаний клавиш в обоих файлах описания ресурсов.

   > [!NOTE]
   > Если в проекте еще нет RC-файла, см. раздел [Создание нового файла описания ресурсов](../windows/how-to-create-a-resource-script-file.md).

2. Выберите запись, которую требуется переместить.

3. Из **изменить** меню, выберите **копирования** или **Вырезать**.

4. Выберите запись в целевом файле описания ресурсов.

5. Из **изменить** меню, выберите **вставить**.

   > [!NOTE]
   > Для копирования и вставки можно также использовать сочетания клавиш.

## <a name="requirements"></a>Требования

Win32

## <a name="see-also"></a>См. также

[Редактирование в таблицах сочетаний клавиш](../windows/editing-accelerator-tables.md)<br/>
[Редактор сочетаний клавиш](../windows/accelerator-editor.md)