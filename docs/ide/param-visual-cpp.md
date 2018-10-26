---
title: '&lt;param&gt; (Visual C++) | Документы Майкрософт'
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-ide
ms.topic: conceptual
f1_keywords:
- param
- <param>
dev_langs:
- C++
helpviewer_keywords:
- param C++ XML tag
- <param> C++ XML tag
ms.assetid: 66c1a1c3-4f98-4bcf-8c7d-9a40308982fb
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 94382cb1f2bab59fae6c397f8ad6dadee221c96b
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46434847"
---
# <a name="ltparamgt-visual-c"></a>&lt;param&gt; (Visual C++)

Тег \<param> следует использовать в комментариях к объявлению метода для описания одного из параметров такого метода.

## <a name="syntax"></a>Синтаксис

```
<param name='name'>description</param>
```

#### <a name="parameters"></a>Параметры

*name*<br/>
Имя параметра метода.  Заключите имя в одинарные или двойные кавычки.  Если компилятору не удается найти `name`, он выдает предупреждение.

*description*<br/>
Описание параметра.

## <a name="remarks"></a>Примечания

Текст тега \<param> будет отображаться в IntelliSense, в [обозревателе объектов](/visualstudio/ide/viewing-the-structure-of-code) и в веб-отчете комментариев кода.

Чтобы обработать и сохранить комментарии документации в файл, при компиляции необходимо использовать параметр [/doc](../build/reference/doc-process-documentation-comments-c-cpp.md).

## <a name="example"></a>Пример

```cpp
// xml_param_tag.cpp
// compile with: /clr /doc /LD
// post-build command: xdcmake xml_param_tag.dll
/// Text for class MyClass.
public ref class MyClass {
   /// <param name="Int1">Used to indicate status.</param>
   void MyMethod(int Int1) {
   }
};
```

## <a name="see-also"></a>См. также

[Документация XML](../ide/xml-documentation-visual-cpp.md)