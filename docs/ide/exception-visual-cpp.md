---
title: '&lt;exception&gt; (Visual C++) | Документы Майкрософт'
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-ide
ms.topic: conceptual
f1_keywords:
- exception
- <exception>
dev_langs:
- C++
helpviewer_keywords:
- <exception> C++ XML tag
- exception C++ XML tag
ms.assetid: 24451e79-9b89-4b77-98fb-702c6516b818
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: bb7b5f4e153ca892cf10f8c5cbe6fe1bebbd20f2
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46419975"
---
# <a name="ltexceptiongt-visual-c"></a>&lt;exception&gt; (Visual C++)

Тег \<exception> служит для указания возможных исключений. Этот тег применяется к определению метода.

## <a name="syntax"></a>Синтаксис

```
<exception cref="member">description</exception>
```

#### <a name="parameters"></a>Параметры

*member*<br/>
Ссылка на исключение, которое доступно из текущей среды компиляции. Используя правила подстановки имен, компилятор проверяет, существует ли исключение, и приводит `member` к каноническому имени элемента в выходных XML-данных.  Если компилятору не удается найти `member`, он выдает предупреждение.

Заключите имя в одинарные или двойные кавычки.

Дополнительные сведения о создании ссылки cref на универсальный тип см. в разделе [\<see>](../ide/see-visual-cpp.md).

*description*<br/>
Описание.

## <a name="remarks"></a>Примечания

Чтобы обработать и сохранить комментарии документации в файл, при компиляции необходимо использовать параметр [/doc](../build/reference/doc-process-documentation-comments-c-cpp.md).

Компилятор Visual C++ будет пытаться разрешить ссылки cref за один проход по комментариям документации.  Поэтому если при использовании правил поиска C++ компилятор не найдет символ, ссылка будет помечена как не разрешенная. Дополнительные сведения см. в описании [\<seealso>](../ide/seealso-visual-cpp.md).

## <a name="example"></a>Пример

```
// xml_exception_tag.cpp
// compile with: /clr /doc /LD
// post-build command: xdcmake xml_exception_tag.dll
using namespace System;

/// Text for class EClass.
public ref class EClass : public Exception {
   // class definition ...
};

/// <exception cref="System.Exception">Thrown when... .</exception>
public ref class TestClass {
   void Test() {
      try {
      }
      catch(EClass^) {
      }
   }
};
```

## <a name="see-also"></a>См. также

[Документация XML](../ide/xml-documentation-visual-cpp.md)