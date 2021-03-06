---
title: -volatile (Интерпретация ключевого слова volatile) | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-tools
ms.topic: reference
f1_keywords:
- /volatile:iso
- /volatile:ms
- /volatile
dev_langs:
- C++
helpviewer_keywords:
- /volatile compiler option
- /volatile compiler option [C++]
- -volatile compiler option
- volatile compiler option [C++]
- volatile compiler option
- -volatile compiler option [C++]
ms.assetid: 9d08fcc6-5bda-44c8-8151-8d8d54f164b8
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 4204d602d1390bf30080a800174426513faf0467
ms.sourcegitcommit: 92f2fff4ce77387b57a4546de1bd4bd464fb51b6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/17/2018
ms.locfileid: "45723638"
---
# <a name="volatile-volatile-keyword-interpretation"></a>/volatile (интерпретация ключевого слова volatile)

Указывает, каким образом [volatile](../../cpp/volatile-cpp.md) ключевое слово будет интерпретироваться.

## <a name="syntax"></a>Синтаксис

> **/ volatile:**{**iso**|**ms**}

## <a name="arguments"></a>Аргументы

**/volatile:ISO**<br/>
Выделяет строгую `volatile` семантику в соответствии с определением языка C++ стандарта ISO. Семантика получения и освобождения не гарантируется переменном обращении. Если компилятор нацелен на ARM, это Интерпретация по умолчанию `volatile`.

**/volatile:MS**<br/>
Выбирает расширенные Майкрософт `volatile` семантику, которая добавляет гарантии за пределы языка C++ стандарта ISO упорядочения памяти. Семантика получения и освобождения гарантируется при переменном обращении. Тем не менее этот параметр также заставляет компилятор генерировать барьеры памяти оборудования, которые могут добавлять значительную нагрузку на ARM и другие архитектуры слабым упорядочиванием памяти. Если компилятор нацелен на любой платформе, за исключением ARM, это Интерпретация по умолчанию `volatile`.

## <a name="remarks"></a>Примечания

Мы настоятельно рекомендуем использовать **/volatile:iso** вместе с явными примитивами синхронизации и встроенными компилятора при работе с памятью, который разделяется между потоками. Дополнительные сведения см. в разделе [volatile](../../cpp/volatile-cpp.md).

Если перенести существующий код или изменить этот параметр посередине проекта, может оказаться полезным включить предупреждение [C4746](../../error-messages/compiler-warnings/compiler-warning-c4746.md) определить расположения кода, затронутые отличиями в семантике.

Существует не `#pragma` эквивалентно элементу управления этот параметр.

### <a name="to-set-the-volatile-compiler-option-in-visual-studio"></a>Чтобы задать/volatile-параметр компилятора в Visual Studio

1. Откройте **страницы свойств** диалоговое окно для проекта. Дополнительные сведения см. в разделе [Работа со свойствами проекта](../../ide/working-with-project-properties.md).

1. Выберите **свойства конфигурации** > **C/C++** > **командной строки** страницу свойств.

1. В **Дополнительные параметры** , добавьте **/volatile:iso** или **/volatile:ms** и выберите **ОК** или **применить** для сохранения изменений.

## <a name="see-also"></a>См. также

[volatile](../../cpp/volatile-cpp.md)<br/>
[Параметры компилятора](../../build/reference/compiler-options.md)<br/>
[Настройка параметров компилятора](../../build/reference/setting-compiler-options.md)
