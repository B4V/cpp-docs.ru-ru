---
title: Блоки | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-language
ms.topic: language-reference
dev_langs:
- C++
helpviewer_keywords:
- function definitions, blocks in code
- blocks
- compound statements
- statements, compound
ms.assetid: be231a92-c712-464e-ae25-a4becb20f7f5
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 9704b499106fc59364f5cc9ae97277939e835a77
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46025326"
---
# <a name="blocks"></a>Blocks

Последовательность объявлений, определений и операторов, заключенная в фигурные скобки (**{ }**), называется "блоком". Существует два типа блоков в С. «Составной оператор» оператор, состоящие из одной или нескольких инструкций (см. [составной оператор](../c-language/compound-statement-c.md)), один тип блока. Второй тип блоков — определение функции — состоит из составного оператора (тело функции) и связанного заголовка функции (имя функции, тип возвращаемого значения и формальные параметры). Блок, находящийся в другом блоке, называется вложенным.

Обратите внимание, что хотя все составные операторы заключены в фигурные скобки, не все элементы, заключенные в фигурные скобки, являются составным оператором. Например, несмотря на то что спецификации элементов массива, структуры или перечисления могут быть заключены в фигурные скобки, они не являются составными операторами.

## <a name="see-also"></a>См. также

[Файлы с исходным кодом и исходные программы](../c-language/source-files-and-source-programs.md)