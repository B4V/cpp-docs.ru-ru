---
title: Функция Exit | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-language
ms.topic: language-reference
f1_keywords:
- Exit
dev_langs:
- C++
helpviewer_keywords:
- exit function
ms.assetid: 26ce439f-81e2-431c-9ff8-a09a96f32127
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 71bff42495c4b6b7bf4016f0f08e7127c2b278ac
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46075180"
---
# <a name="exit-function"></a>Функция exit

**Выйти из** функции, объявленные в стандартном включаемом файле \<stdlib.h >, завершает программу C++.

Значение, указанное в качестве аргумента **выйти из** возвращается в операционную систему, как ее возвращаемое код или код выхода. Принято, чтобы нулевым кодом возврата обозначалось, что программа завершена успешно.

> [!NOTE]
>  Можно использовать константы, EXIT_FAILURE и EXIT_SUCCESS, определенные в \<stdlib.h >, чтобы указать на успех или сбой программы.

Выдача **возвращают** инструкции от `main` функция эквивалентно вызову **выйти из** функции с возвращаемым значением в качестве аргумента.

Дополнительные сведения см. в разделе [выйти из](../c-runtime-library/reference/exit-exit-exit.md) в *Справочник по библиотеке времени выполнения*.

## <a name="see-also"></a>См. также

[Завершение программы](../cpp/program-termination.md)