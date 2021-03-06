---
title: Ключевые слова в C | Документы Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-language
ms.topic: language-reference
dev_langs:
- C++
helpviewer_keywords:
- keywords [C]
- redefining keywords
- Microsoft-specific keywords
ms.assetid: 2d932335-97bf-45cd-b367-4ae00db0ff42
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 80c1f0d4ac5d843732771281202612e31a4073c2
ms.sourcegitcommit: 997e6b7d336cddb388bb6e9e56527725fcaa0624
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/08/2018
ms.locfileid: "48860892"
---
# <a name="c-keywords"></a>Ключевые слова в C

Ключевыми словами называются слова, которые имеют особое значение для компилятора C. На 7 и 8 этапах трансляции идентификатор не может иметь такое же написание и регистр записи, что и ключевое слово C. (См. описание [этапов трансляции](../preprocessor/phases-of-translation.md) в *Справочнике по препроцессору*. Дополнительные сведения об идентификаторах см. в разделе [Идентификаторы](../c-language/c-identifiers.md).) В языке C используются следующие ключевые слова:

|||||
|-|-|-|-|
|**auto**|**double**|**int**|**struct**|
|**break**|**else**|**long**|**switch**|
|**case**|**enum**|**register**|**typedef**|
|**char**|**extern**|**return**|**объединение**|
|**const**|**float**|**short**|**unsigned**|
|**continue**|**for**|**signed**|**void**|
|**default**|**goto**|**sizeof**|**volatile**|
|**do**|**if**|**static**|**while**|

Переопределить ключевые слова невозможно. Но с помощью [директив препроцессора](../preprocessor/preprocessor-directives.md) C можно определить текст, который будет использоваться вместо ключевых слов.

**Блок, относящийся только к системам Microsoft**

Стандарт ANSI C позволяет зарезервировать идентификаторы, начинающиеся с двух символов подчеркивания, для реализаций компилятора. Поэтому в системах Microsoft действует соглашение, что используемые в них ключевые слова начинаются с двух символов подчеркивания. Эти слова невозможно использовать как имена идентификаторов. Описание правил именования идентификаторов в ANSI, включая использование двойных знаков подчеркивания, см. в разделе [Идентификаторы](../c-language/c-identifiers.md).

Компилятор Microsoft C распознает следующие ключевые слова и особые идентификаторы.

|||||
|-|-|-|-|
|**__asm**|**dllimport**<sup>2</sup>|**__int8**|**naked**<sup>2</sup>|
|**__based**<sup>1</sup>|**__except**|**__int16**|**__stdcall**|
|**__cdecl**|**__fastcall**|**__int32**|**thread**<sup>2</sup>|
|**__declspec**|**__finally**|**__int64**|**__try**|
|**dllexport**<sup>2</sup>|**__inline**|**__leave**||

<sup>1</sup> Ключевое слово **__based** имеет ограниченное применение: в компиляциях для 32- и 64-разрядных платформ.

<sup>2</sup> Если эти ключевые слова используются с ключевым словом **__declspec**, они являются особыми идентификаторами. В других контекстах они могут использоваться без ограничений.

Расширения Microsoft по умолчанию включены. Для того чтобы ваши программы были полностью переносимы, расширения Microsoft можно отключить, установив во время компиляции параметр /Za (компилировать для совместимости с ANSI). При этом ключевые слова для систем Microsoft будут отключены.

Когда расширения Microsoft включены, в программах можно использовать перечисленные выше ключевые слова. Для совместимости со стандартом ANSI большинство этих ключевых слов начинаются с двух символов подчеркивания. Четыре исключения, **dllexport**, **dllimport**, **naked** и **thread**, используются только с ключевым словом **__declspec** и поэтому не требуют двойного знака подчеркивания. Для всех остальных ключевых слов поддерживаются версии с одним символом подчеркивания. Это сделано для обеспечения обратной совместимости.

**Завершение блока, относящегося только к системам Майкрософт**

## <a name="see-also"></a>См. также

[Элементы языка C](../c-language/elements-of-c.md)
