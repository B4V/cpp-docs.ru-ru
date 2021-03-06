---
title: Использование элемента управления RichEdit 1.0 с MFC | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-windows
ms.topic: conceptual
dev_langs:
- C++
helpviewer_keywords:
- RichEdit 1.0 control
- rich edit controls [C++], RichEdit 1.0
ms.assetid: 5a9060dd-44d8-4ef3-956e-16152f7e23d2
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
- uwp
ms.openlocfilehash: 63bda924a91bb1f86494d844af037386d6e30292
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46406351"
---
# <a name="using-the-richedit-10-control-with-mfc"></a>Использование элемента управления RichEdit 1.0 с MFC

Чтобы использовать элемент управления RichEdit, необходимо сначала вызвать [AfxInitRichEdit2](../mfc/reference/application-information-and-management.md#afxinitrichedit2) загрузить элемент управления RichEdit 2.0 (библиотеки RICHED20. Библиотека DLL), или вызвать [AfxInitRichEdit](../mfc/reference/application-information-and-management.md#afxinitrichedit) для загрузки более старых элемента управления RichEdit 1.0 (RICHED32. БИБЛИОТЕКА DLL).

Вы можете использовать текущий [CRichEditCtrl](../mfc/reference/cricheditctrl-class.md) класса с помощью более старых элемента управления RichEdit 1.0, но `CRichEditCtrl` предназначена только для поддержки управления RichEdit 2.0. Поскольку RichEdit 1.0 и RichEdit 2.0 очень похожи, будет работать большинство методов; Тем не менее Обратите внимание, что существуют некоторые различия между 1.0 и 2.0 элементы управления, поэтому некоторые методы могут работать неправильно или вообще не работать.

## <a name="requirements"></a>Требования

MFC

## <a name="see-also"></a>См. также

[Устранение неполадок редактора диалоговых окон](../windows/troubleshooting-the-dialog-editor.md)<br/>
[Редактор диалоговых окон](../windows/dialog-editor.md)