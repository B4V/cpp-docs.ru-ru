---
title: Класс sub_match | Документы Майкрософт
ms.custom: ''
ms.date: 09/10/2018
ms.technology:
- cpp-standard-libraries
ms.topic: reference
f1_keywords:
- regex/std::sub_match
- regex/std::sub_match::matched
- regex/std::sub_match::compare
- regex/std::sub_match::length
- regex/std::sub_match::str
- regex/std::sub_match::difference_type
- regex/std::sub_match::iterator
- regex/std::sub_match::value_type
dev_langs:
- C++
helpviewer_keywords:
- std::sub_match [C++]
- std::sub_match [C++], matched
- std::sub_match [C++], compare
- std::sub_match [C++], length
- std::sub_match [C++], str
- std::sub_match [C++], difference_type
- std::sub_match [C++], iterator
- std::sub_match [C++], value_type
ms.assetid: 804e2b9e-d16a-4c4c-ac60-024e0b2dd0e8
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 65d873c4e7188b3000cee65e03c4ce6edcad8046
ms.sourcegitcommit: 1d9bd38cacbc783fccd3884b7b92062161c91c84
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/03/2018
ms.locfileid: "48235338"
---
# <a name="submatch-class"></a>Класс sub_match

Описывает подстроку соответствия.

## <a name="syntax"></a>Синтаксис

```cpp
template <class BidIt>
class sub_match
    : public std::pair<BidIt, BidIt>
```

## <a name="parameters"></a>Параметры

*BidIt*<br/>
Тип итератора для подстрок соответствия.

## <a name="remarks"></a>Примечания

Класс шаблона описывает объект, который определяет последовательность символов, соответствующих группе записи в вызове [regex_match](../standard-library/regex-functions.md#regex_match) или [regex_search](../standard-library/regex-functions.md#regex_search). Объекты типа [Класс match_results](../standard-library/match-results-class.md) содержат массив таких объектов, по одному для каждой группы записи в регулярном выражении, которое использовалось при поиске.

Если группа записи не соответствует члену данных объекта, `matched` содержит значение false, а два итератора `first` и `second` (наследуются от базового класса `std::pair`) равны. Если обнаружено соответствие группе записи, `matched` содержит значение true, итератор `first` указывает на первый символ в целевой последовательности, которая соответствует группе записи, а итератор `second` указывает на одну позицию после последнего символа в целевой последовательности, которая соответствует группе записи. Обратите внимание, что для соответствия нулевой длины член `matched` должен содержать значение true, два итератора быть эквиваленты и оба указывать на одну позицию соответствия.

Соответствие нулевой длины может возникать, когда группа записи состоит только из утверждения или из повторения, допускающего нулевые повторы. Пример:

"^" соответствует целевой последовательности "a"; объект `sub_match` , соответствующий группе записи 0, содержит два итератора, которые указывают на первый символ в последовательности.

"b(a*)b" соответствует целевой последовательности "bb"; объект `sub_match` , соответствующий группе записи 1, содержит два итератора, которые указывают на второй символ в последовательности.

### <a name="typedefs"></a>Определения типов

|Имя типа|Описание|
|-|-|
|[difference_type](#difference_type)|Тип разницы итератора.|
|[iterator](#iterator)|Тип итератора.|
|[value_type](#value_type)|Тип элемента.|

### <a name="member-functions"></a>Функции-члены

|Функция-член|Описание|
|-|-|
|[compare](#compare)|Сравнение подстроки и последовательности.|
|[length](#length)|Возвращает длину частичного совпадения.|
|[соответствует](#matched)|Указывает, успешно ли выполнено сопоставление.|
|[str](#str)|Преобразует подстроку в строку.|

### <a name="operators"></a>Операторы

|Оператор|Описание|
|-|-|
|[Operator basic_string < value_type >](#op_basic_string_lt_value_type_gt)|Приводит подстроку соответствия к строке.|

## <a name="example"></a>Пример

```cpp
// std__regex__sub_match.cpp
// compile with: /EHsc
#include <regex>
#include <iostream>

int main()
    {
    std::regex rx("c(a*)|(b)");
    std::cmatch mr;

    std::regex_search("xcaaay", mr, rx);

    std::csub_match sub = mr[1];
    std::cout << "matched == " << std::boolalpha
        << sub.matched << std::endl;
    std::cout << "length == " << sub.length() << std::endl;

    std::csub_match::difference_type dif = std::distance(sub.first, sub.second);
    std::cout << "difference == " << dif << std::endl;

    std::csub_match::iterator first = sub.first;
    std::csub_match::iterator last = sub.second;
    std::cout << "range == " << std::string(first, last)
        << std::endl;
    std::cout << "string == " << sub << std::endl;

    std::csub_match::value_type const *ptr = "aab";
    std::cout << "compare(\"aab\") == "
        << sub.compare(ptr) << std::endl;
    std::cout << "compare(string) == "
        << sub.compare(std::string("AAA")) << std::endl;
    std::cout << "compare(sub) == "
        << sub.compare(sub) << std::endl;

    return (0);
    }
```

```Output
matched == true
length == 3
difference == 3
range == aaa
string == aaa
compare("aab") == -1
compare(string) == 1
compare(sub) == 0
```

## <a name="requirements"></a>Требования

**Заголовок:** \<regex>

**Пространство имен:** std

## <a name="compare"></a>  sub_match::compare

Сравнение подстроки и последовательности.

```cpp
int compare(const sub_match& right) const;
int compare(const basic_string<value_type>& str) const;
int compare(const value_type *ptr) const;
```

### <a name="parameters"></a>Параметры

*right*<br/>
Подстрока для сравнения.

*str*<br/>
Строка для сравнения.

*ptr*<br/>
Последовательность, оканчивающаяся нулевым символом, для сравнения.

### <a name="remarks"></a>Примечания

Первая функция-член сравнивает совпадающую последовательность `[first, second)` с совпадающей последовательностью `[right.first, right.second)`. Вторая функция-член сравнивает совпадающую последовательность `[first, second)` с последовательностью символов `[right.begin(), right.end())`. Третья функция-член сравнивает совпадающую последовательность `[first, second)` с последовательностью символов `[right, right + std::char_traits<value_type>::length(right))`.

Каждая функция возвращает:

отрицательное значение, если первое отличающееся значение в совпадающей последовательности оказывается меньше, чем соответствующий элемент в последовательности операнда (определяется `std::char_traits<value_type>::compare`), либо, если они имеют одинаковый префикс, но целевая последовательность длиннее;

нуль, если обе последовательности поэлементно совпадают и имеют одинаковую длину;

в противном случае — положительное значение.

## <a name="difference_type"></a>  sub_match::difference_type

Тип разницы итератора.

```cpp
typedef typename iterator_traits<BidIt>::difference_type difference_type;
```

### <a name="remarks"></a>Примечания

Typedef является синонимом `iterator_traits<BidIt>::difference_type`.

## <a name="iterator"></a>  sub_match::iterator

Тип итератора.

```cpp
typedef BidIt iterator;
```

### <a name="remarks"></a>Примечания

Typedef является синонимом параметра шаблона `Bidit`.

## <a name="length"></a>  sub_match::length

Возвращает длину частичного совпадения.

```cpp
difference_type length() const;
```

### <a name="remarks"></a>Примечания

Функция-член возвращает длину совпадающей последовательности либо нуль, если последовательность не совпадает.

## <a name="matched"></a>  sub_match::matched

Указывает, успешно ли выполнено сопоставление.

```cpp
bool matched;
```

### <a name="remarks"></a>Примечания

Член содержит **true** только в том случае, если группа захвата, связанная с `*this` входил в состав совпадения регулярного выражения.

## <a name="op_basic_string_lt_value_type_gt"></a>  sub_match::operator basic_string&lt;value_type&gt;

Приводит подстроку соответствия к строке.

```cpp
operator basic_string<value_type>() const;
```

### <a name="remarks"></a>Примечания

Оператор-член возвращает `str()`.

## <a name="str"></a>  sub_match::str

Преобразует подстроку в строку.

```cpp
basic_string<value_type> str() const;
```

### <a name="remarks"></a>Примечания

Функция-член возвращает значение `basic_string<value_type>(first, second)`.

## <a name="value_type"></a>  sub_match::value_type

Тип элемента.

```cpp
typedef typename iterator_traits<BidIt>::value_type value_type;
```

### <a name="remarks"></a>Примечания

Typedef является синонимом `iterator_traits<BidIt>::value_type`.

## <a name="see-also"></a>См. также

[\<regex>](../standard-library/regex.md)<br/>
[sub_match](../standard-library/sub-match-class.md)<br/>
