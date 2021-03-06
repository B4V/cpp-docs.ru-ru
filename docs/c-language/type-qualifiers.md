---
title: Квалификаторы типов | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-language
ms.topic: language-reference
dev_langs:
- C++
helpviewer_keywords:
- volatile keyword [C], type qualifier
- type qualifiers
- volatile keyword [C]
- qualifiers for types
- const keyword [C]
- memory, access using volatile
- volatile keyword [C], type specifier
ms.assetid: bb4c6744-1dd7-40a8-b4eb-f5585be30908
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 8ecac60a1b9cbd2758090e52d917c7a65259d62d
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46094395"
---
# <a name="type-qualifiers"></a>Квалификаторы типов

Квалификаторы типов предоставляют идентификатору одно из двух свойств. Квалификатор типа **const** объявляет объект как неизменяемый. Квалификатор типа `volatile` объявляет элемент, значение которого можно изменить допустимым образом с помощью средств, недоступных программе, в которой он находится, таких как выполняемый в данный момент поток.

Квалификаторы типов **const** и `volatile` могут использоваться в объявлении только один раз. Квалификаторы типов могут использоваться с любым описателем типа; однако они не могут находиться после первой запятой в объявлении нескольких элементов. Например, следующие объявления допустимы.

```
typedef volatile int VI;
const int ci;
```

Следующие объявления не допустимы.

```
typedef int *i, volatile *vi;
float f, const cf;
```

Квалификаторы типов имеют смысл только при обращении к идентификаторам как к l-значениям в выражениях. Дополнительные сведения о левосторонних значениях и выражениях см. в статье [Выражения L-Value и R-Value](../c-language/l-value-and-r-value-expressions.md).

## <a name="syntax"></a>Синтаксис

*type-qualifier*: **constvolatile**

Ниже представлены допустимые объявления **const`volatile` и** .

```
int const *p_ci;       /* Pointer to constant int */
int const (*p_ci);     /* Pointer to constant int */
int *const cp_i;       /* Constant pointer to int */
int (*const cp_i);     /* Constant pointer to int */
int volatile vint;     /* Volatile integer        */
```

Если спецификация типа массива включает квалификаторы типов, определяется элемент, а не тип массива. Если спецификация типа функции включает квалификаторы, поведение не определено. Ни `volatile`, ни **const** не влияют на диапазон значений или арифметические свойства объекта.

В следующем списке описано использование **const** и `volatile`.

- Ключевое слово **const** можно использовать для изменения любого фундаментального или агрегатного типа, указателя на объект любого типа или `typedef`. Если элемент объявлен только с квалификатором типа **const**, считается, что он имеет тип **const int**. Переменную с квалификатором **const** можно инициализировать в области хранения, доступной только для чтения, или переместить в такую область. Ключевое слово **const** полезно при объявлении указателей на значения **const**. Так вы сообщите функции, что этот указатель нельзя изменять.

- Компилятор предполагает, что в любом месте программы к переменной `volatile` можно получить доступ в ходе неизвестного процесса, в котором используется или изменяется ее значение. Следовательно, независимо от оптимизаций, указанных в командной строке, необходимо создать код для каждого назначения переменной `volatile` или ссылки на нее, даже если кажется, что это ничего не изменит.

     Если `volatile` используется отдельно, предполагается `int`. Описатель типа `volatile` можно использовать для предоставления надежного доступа к специальным адресам памяти. Используйте `volatile` с объектами данных, к которым можно получить доступ или которые можно изменить с помощью обработчиков сигналов, одновременного выполнения программ или специального оборудования, например регистров управления MMIO. Можно объявить переменную как `volatile` на протяжении ее времени жизни или привести одну ссылку ко значению `volatile`.

- Элемент может одновременно быть **const** и `volatile`, и тогда его невозможно изменить допустимым образом в собственной программе, но можно изменить в некотором асинхронном процессе.

## <a name="see-also"></a>См. также

[Объявления и типы](../c-language/declarations-and-types.md)