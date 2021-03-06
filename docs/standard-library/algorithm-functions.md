---
title: '&lt;&gt; алгоритмов | Документы Майкрософт'
ms.custom: ''
ms.date: 11/04/2016
ms.topic: reference
f1_keywords:
- algorithm/std::adjacent_find
- algorithm/std::all_of
- algorithm/std::any_of
- algorithm/std::binary_search
- algorithm/std::copy
- algorithm/std::copy_backward
- algorithm/std::copy_if
- algorithm/std::copy_n
- algorithm/std::equal
- algorithm/std::equal_range
- algorithm/std::fill
- algorithm/std::fill_n
- algorithm/std::find
- algorithm/std::find_end
- algorithm/std::find_first_of
- algorithm/std::find_if
- algorithm/std::find_if_not
- algorithm/std::for_each
- algorithm/std::generate
- algorithm/std::generate_n
- algorithm/std::includes
- algorithm/std::inplace_merge
- algorithm/std::is_heap
- algorithm/std::is_heap_until
- algorithm/std::is_partitioned
- algorithm/std::is_permutation
- algorithm/std::is_sorted
- algorithm/std::is_sorted_until
- algorithm/std::iter_swap
- algorithm/std::lexicographical_compare
- algorithm/std::lower_bound
- algorithm/std::make_heap
- algorithm/std::max
- algorithm/std::max_element
- algorithm/std::merge
- algorithm/std::min
- algorithm/std::minmax
- algorithm/std::minmax_element
- algorithm/std::min_element
- algorithm/std::mismatch
- algorithm/std::move
- algorithm/std::move_backward
- algorithm/std::next_permutation
- algorithm/std::none_of
- algorithm/std::nth_element
- algorithm/std::partial_sort
- algorithm/std::partial_sort_copy
- algorithm/std::partition
- algorithm/std::partition_point
- algorithm/std::pop_heap
- algorithm/std::prev_permutation
- algorithm/std::push_heap
- algorithm/std::random_shuffle
- algorithm/std::remove
- algorithm/std::remove_copy
- algorithm/std::remove_copy_if
- algorithm/std::remove_if
- algorithm/std::replace
- algorithm/std::replace_copy
- algorithm/std::replace_copy_if
- algorithm/std::replace_if
- algorithm/std::reverse
- algorithm/std::reverse_copy
- algorithm/std::rotate
- algorithm/std::rotate_copy
- algorithm/std::search
- algorithm/std::search_n
- algorithm/std::set_difference
- algorithm/std::set_intersection
- algorithm/std::set_symmetric_difference
- algorithm/std::set_union
- algorithm/std::shuffle
- algorithm/std::sort
- algorithm/std::sort_heap
- algorithm/std::stable_partition
- algorithm/std::stable_sort
- algorithm/std::swap_ranges
- algorithm/std::transform
- algorithm/std::unique
- algorithm/std::unique_copy
- algorithm/std::upper_bound
- xutility/std::copy
- xutility/std::copy_backward
- xutility/std::copy_n
- xutility/std::count
- xutility/std::equal
- xutility/std::fill
- xutility/std::fill_n
- xutility/std::find
- xutility/std::is_permutation
- xutility/std::lexicographical_compare
- xutility/std::move
- xutility/std::move_backward
- xutility/std::reverse
- xutility/std::rotate
- algorithm/std::count_if
- algorithm/std::partition_copy
- algorithm/std::swap
dev_langs:
- C++
ms.assetid: c10b0c65-410c-4c83-abf8-8b7f61bba8d0
author: corob-msft
ms.author: corob
helpviewer_keywords:
- std::adjacent_find [C++]
- std::all_of [C++]
- std::any_of [C++]
- std::binary_search [C++]
- std::copy [C++]
- std::copy_backward [C++]
- std::copy_if [C++]
- std::copy_n [C++]
- std::equal [C++]
- std::equal_range [C++]
- std::fill [C++]
- std::fill_n [C++]
- std::find [C++]
- std::find_end [C++]
- std::find_first_of [C++]
- std::find_if [C++]
- std::find_if_not [C++]
- std::for_each [C++]
- std::generate [C++]
- std::generate_n [C++]
- std::includes [C++]
- std::inplace_merge [C++]
- std::is_heap [C++]
- std::is_heap_until [C++]
- std::is_partitioned [C++]
- std::is_permutation [C++]
- std::is_sorted [C++]
- std::is_sorted_until [C++]
- std::iter_swap [C++]
- std::lexicographical_compare [C++]
- std::lower_bound [C++]
- std::make_heap [C++]
- std::max [C++]
- std::max_element [C++]
- std::merge [C++]
- std::min [C++]
- std::minmax [C++]
- std::minmax_element [C++]
- std::min_element [C++]
- std::mismatch [C++]
- std::move [C++]
- std::move_backward [C++]
- std::next_permutation [C++]
- std::none_of [C++]
- std::nth_element [C++]
- std::partial_sort [C++]
- std::partial_sort_copy [C++]
- std::partition [C++]
- std::partition_point [C++]
- std::pop_heap [C++]
- std::prev_permutation [C++]
- std::push_heap [C++]
- std::random_shuffle [C++]
- std::remove [C++]
- std::remove_copy [C++]
- std::remove_copy_if [C++]
- std::remove_if [C++]
- std::replace [C++]
- std::replace_copy [C++]
- std::replace_copy_if [C++]
- std::replace_if [C++]
- std::reverse [C++]
- std::reverse_copy [C++]
- std::rotate [C++]
- std::rotate_copy [C++]
- std::search [C++]
- std::search_n [C++]
- std::set_difference [C++]
- std::set_intersection [C++]
- std::set_symmetric_difference [C++]
- std::set_union [C++]
- std::shuffle [C++]
- std::sort [C++]
- std::sort_heap [C++]
- std::stable_partition [C++]
- std::stable_sort [C++]
- std::swap_ranges [C++]
- std::transform [C++]
- std::unique [C++]
- std::unique_copy [C++]
- std::upper_bound [C++]
- std::copy [C++]
- std::copy_backward [C++]
- std::copy_n [C++]
- std::count [C++]
- std::equal [C++]
- std::fill [C++]
- std::fill_n [C++]
- std::find [C++]
- std::is_permutation [C++]
- std::lexicographical_compare [C++]
- std::move [C++]
- std::move_backward [C++]
- std::reverse [C++]
- std::rotate [C++]
- std::count_if [C++]
- std::partition_copy [C++]
- std::swap [C++]
ms.workload:
- cplusplus
ms.openlocfilehash: a21dc4e0687ece8583b2291b71ed55980127805c
ms.sourcegitcommit: a9dcbcc85b4c28eed280d8e451c494a00d8c4c25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2018
ms.locfileid: "50082753"
---
# <a name="ltalgorithmgt-functions"></a>&lt;функции&gt; алгоритмов

||||
|-|-|-|
|[move](#alg_move)|[adjacent_find](#adjacent_find)|[all_of](#all_of)|
|[any_of](#any_of)|[binary_search](#binary_search)|[copy](#copy)|
|[copy_backward](#copy_backward)|[copy_if](#copy_if)|[copy_n](#copy_n)|
|[count](#count)|[count_if](#count_if)|[equal](#equal)|
|[equal_range](#equal_range)|[fill](#fill)|[fill_n](#fill_n)|
|[find](#find)|[find_end](#find_end)|[find_first_of](#find_first_of)|
|[find_if](#find_if)|[find_if_not](#find_if_not)|[for_each](#for_each)|
|[generate](#generate)|[generate_n](#generate_n)|[includes](#includes)|
|[inplace_merge](#inplace_merge)|[is_heap](#is_heap)|[is_heap_until](#is_heap_until)|
|[is_partitioned](#is_partitioned)|[is_permutation](#is_permutation)|[is_sorted](#is_sorted)|
|[is_sorted_until](#is_sorted_until)|[iter_swap](#iter_swap)|[lexicographical_compare](#lexicographical_compare)|
|[lower_bound](#lower_bound)|[make_heap](#make_heap)|[max](#max)|
|[max_element](#max_element)|[merge](#merge)|[min](#min)|
|[min_element](#min_element)|[minmax](#minmax)|[minmax_element](#minmax_element)|
|[mismatch](#mismatch)|[move_backward](#move_backward)|[next_permutation](#next_permutation)|
|[none_of](#none_of)|[nth_element](#nth_element)|[partial_sort](#partial_sort)|
|[partial_sort_copy](#partial_sort_copy)|[partition](#partition)|[partition_copy](#partition_copy)|
|[partition_point](#partition_point)|[pop_heap](#pop_heap)|[prev_permutation](#prev_permutation)|
|[push_heap](#push_heap)|[random_shuffle](#random_shuffle)|[remove](#remove)|
|[remove_copy](#remove_copy)|[remove_copy_if](#remove_copy_if)|[remove_if](#remove_if)|
|[replace](#replace)|[replace_copy](#replace_copy)|[replace_copy_if](#replace_copy_if)|
|[replace_if](#replace_if)|[reverse](#reverse)|[reverse_copy](#reverse_copy)|
|[rotate](#rotate)|[rotate_copy](#rotate_copy)|[search](#search)|
|[search_n](#search_n)|[set_difference](#set_difference)|[set_intersection](#set_intersection)|
|[set_symmetric_difference](#set_symmetric_difference)|[set_union](#set_union)|[sort](#sort)|
|[sort_heap](#sort_heap)|[stable_partition](#stable_partition)|[stable_sort](#stable_sort)|
|[shuffle](#shuffle)|[swap](#swap)|[swap_ranges](#swap_ranges)|
|[transform](#transform)|[unique](#unique)|[unique_copy](#unique_copy)|
|[upper_bound](#upper_bound)|

## <a name="adjacent_find"></a>  adjacent_find

Поиск двух соседних элементов, которые либо равны, либо удовлетворяют указанному условию.

```cpp
template<class ForwardIterator>
ForwardIterator adjacent_find(
    ForwardIterator first,
    ForwardIterator last);

template<class ForwardIterator , class BinaryPredicate>
ForwardIterator adjacent_find(
    ForwardIterator first,
    ForwardIterator last,
    BinaryPredicate comp);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Прямой итератор, адресующий положение первого элемента в диапазоне для поиска.

*последний*<br/>
Прямой итератор, адресующий положение на единицу после последнего элемента в диапазоне для поиска.

*Зап.*<br/>
Двоичный предикат, задающий условие, которому должны удовлетворять значения соседних элементов в диапазоне, по которому выполняется поиск.

### <a name="return-value"></a>Возвращаемое значение

Прямой итератор на первый элемент из пары соседних элементов, которые либо равны друг другу (в первой версии), либо удовлетворяют условию двоичного предиката (во второй версии), если такая пара элементов найдена. В противном случае — итератор, указывающий на *последнего* возвращается.

### <a name="remarks"></a>Примечания

Алгоритм `adjacent_find` не изменяет последовательность. Диапазон, по которому ведется поиск, должен быть допустимым; все указатели должны поддерживать сброс ссылок должна быть возможность достижения последнего положения с первого путем приращения. Временная сложность алгоритма линейно зависит от количества элементов в диапазоне.

`operator==`, используемый для определения совпадения между элементами, налагает отношение эквивалентности между своими операндами.

### <a name="example"></a>Пример

```cpp
// alg_adj_fnd.cpp
// compile with: /EHsc
#include <list>
#include <algorithm>
#include <iostream>

// Returns whether second element is twice the first
bool twice (int elem1, int elem2 )
{
   return elem1 * 2 == elem2;
}

int main()
{
   using namespace std;
   list <int> L;
   list <int>::iterator Iter;
   list <int>::iterator result1, result2;

   L.push_back( 50 );
   L.push_back( 40 );
   L.push_back( 10 );
   L.push_back( 20 );
   L.push_back( 20 );

   cout << "L = ( " ;
   for ( Iter = L.begin( ) ; Iter != L.end( ) ; Iter++ )
      cout << *Iter << " ";
   cout << ")" << endl;

   result1 = adjacent_find( L.begin( ), L.end( ) );
   if ( result1 == L.end( ) )
      cout << "There are not two adjacent elements that are equal."
           << endl;
   else
      cout << "There are two adjacent elements that are equal."
           << "\n They have a value of "
           <<  *( result1 ) << "." << endl;

   result2 = adjacent_find( L.begin( ), L.end( ), twice );
   if ( result2 == L.end( ) )
      cout << "There are not two adjacent elements where the "
           << " second is twice the first." << endl;
   else
      cout << "There are two adjacent elements where "
           << "the second is twice the first."
           << "\n They have values of " << *(result2++);
      cout << " & " << *result2 << "." << endl;
}
```

```Output
L = ( 50 40 10 20 20 )
There are two adjacent elements that are equal.
They have a value of 20.
There are two adjacent elements where the second is twice the first.
They have values of 10 & 20.
```

## <a name="all_of"></a>  all_of

Возвращает **true** когда условие выполняется каждым элементом заданного диапазона.

```cpp
template<class InputIterator, class Predicate>
bool all_of(
    InputIterator first,
    InputIterator last,
    BinaryPredicatecomp);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Входной итератор, указывающий, откуда должна начинаться проверка условия. Итератор отмечает, где начинается диапазон элементов.

*последний*<br/>
Входной итератор, указывающий конец диапазона элементов для проверки условия.

*Зап.*<br/>
Условие для проверки. Это определенный пользователем объект функции предиката, задающий условие, которому должен соответствовать проверяемый элемент. Предикат принимает один аргумент и возвращает значение **true** или **false**.

### <a name="return-value"></a>Возвращаемое значение

Возвращает **true** при обнаружении этого условия в каждом элементе в указанном диапазоне соответствует условию, и **false** Если условие не будет обнаружен по крайней мере один раз.

### <a name="remarks"></a>Примечания

Функция шаблона возвращает **true** только если для каждого `N` в диапазоне `[0,Last - first)`, предикат `comp(*(_First + N))` — **true**.

## <a name="any_of"></a>  any_of

Возвращает **true** Если условие выполняется хотя бы один раз в указанный диапазон элементов.

```cpp
template<class InputIterator, class UnaryPredicate>
bool any_of(
    InputIterator first,
    InputIterator last,
    UnaryPredicate comp);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Входной итератор, указывающий, откуда должна начинаться проверка диапазона элементов на соответствие условию.

*последний*<br/>
Входной итератор, указывающий конец диапазона элементов для проверки условия.

*Зап.*<br/>
Условие для проверки. Оно предоставляется определенным пользователем объектом функции предиката. Предикат задает условие, которому должен соответствовать проверяемый элемент. Предикат принимает один аргумент и возвращает значение **true** или **false**.

### <a name="return-value"></a>Возвращаемое значение

Возвращает **true** обнаруживается условие, по крайней мере один раз в указанном диапазоне соответствует условию, **false** Если условие никогда не обнаружено.

### <a name="remarks"></a>Примечания

Функция шаблона возвращает **true** только если для некоторых `N` в диапазоне

`[0, last - first)`, предикат `comp(*(first + N))` имеет значение true.

## <a name="binary_search"></a>  binary_search

Проверяет, есть ли в отсортированном диапазоне элемент, равный указанному значению или эквивалентный ему в смысле, заданном двоичным предикатом.

```cpp
template<class ForwardIterator, class Type>
bool binary_search(
    ForwardIterator first,
    ForwardIterator last,
    const Type& value);

template<class ForwardIterator,  class Type,  class BinaryPredicate>
bool binary_search(
    ForwardIterator first,
    ForwardIterator last,
    const Type& value,
    BinaryPredicate comp);

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Прямой итератор, адресующий положение первого элемента в диапазоне для поиска.

*последний*<br/>
Прямой итератор, адресующий положение на единицу после последнего элемента в диапазоне для поиска.

*значение*<br/>
Значение должно соответствовать значению элемента или удовлетворять условию со значением элемента, заданному двоичным предикатом.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, задающий условие, когда один элемент меньше другого. Двоичный предикат принимает два аргумента и возвращает **true** , если условие удовлетворено, или **false** , если условие не удовлетворено.

### <a name="return-value"></a>Возвращаемое значение

**значение true,** Если обнаруживается элемент, который равен или эквивалентное указанному значению; в противном случае — значение в диапазоне **false**.

### <a name="remarks"></a>Примечания

Упорядоченный исходный диапазон, на который указывает ссылка, должен быть допустим. Все указатели должны поддерживать отмену ссылок. В последовательности должна иметься возможность достижения последней позиции с первой путем приращения.

Предварительное условие для применения алгоритма `binary_search` состоит в том, что каждый упорядоченный диапазон должен быть упорядочен в соответствии с теми же правилами, которые будут использоваться этим алгоритмом для сортировки объединенных диапазонов.

Алгоритм `binary_search` не изменяет исходные диапазоны.

В целях упорядочения типы значений прямых итераторов должны подлежать сравнению "меньше чем", чтобы при наличии двух элементов можно было определить, что они равны (т. е. ни один не меньше другого) или что один меньше другого. Это приводит к упорядочению неравнозначных элементов.

Сложность алгоритма является логарифмической для итераторов произвольного доступа и линейной в противном случае с числом шагов, пропорциональным значению (`last` - `first`).

### <a name="example"></a>Пример

```cpp
// alg_bin_srch.cpp
// compile with: /EHsc
#include <list>
#include <vector>
#include <algorithm>
#include <functional>      // greater<int>( )
#include <iostream>

// Return whether modulus of elem1 is less than modulus of elem2
bool mod_lesser( int elem1, int elem2 )
{
    if (elem1 < 0)
        elem1 = - elem1;
    if (elem2 < 0)
        elem2 = - elem2;
    return elem1 < elem2;
}

int main()
{
    using namespace std;

    list <int> List1;

    List1.push_back( 50 );
    List1.push_back( 10 );
    List1.push_back( 30 );
    List1.push_back( 20 );
    List1.push_back( 25 );
    List1.push_back( 5 );

    List1.sort();

    cout << "List1 = ( " ;
    for ( auto Iter : List1 )
        cout << Iter << " ";
    cout << ")" << endl;

    // default binary search for 10
    if ( binary_search(List1.begin(), List1.end(), 10) )
        cout << "There is an element in list List1 with a value equal to 10."
        << endl;
    else
        cout << "There is no element in list List1 with a value equal to 10."
        << endl;

    // a binary_search under the binary predicate greater
    List1.sort(greater<int>());
    if ( binary_search(List1.begin(), List1.end(), 10, greater<int>()) )
        cout << "There is an element in list List1 with a value greater than 10 "
        << "under greater than." << endl;
    else
        cout << "No element in list List1 with a value greater than 10 "
        << "under greater than." << endl;

    // a binary_search under the user-defined binary predicate mod_lesser
    vector<int> v1;

    for ( auto i = -2; i <= 4; ++i )
    {
        v1.push_back(i);
    }

    sort(v1.begin(), v1.end(), mod_lesser);

    cout << "Ordered using mod_lesser, vector v1 = ( " ;
    for ( auto Iter : v1 )
        cout << Iter << " ";
    cout << ")" << endl;

    if ( binary_search(v1.begin(), v1.end(), -3, mod_lesser) )
        cout << "There is an element with a value equivalent to -3 "
        << "under mod_lesser." << endl;
    else
        cout << "There is not an element with a value equivalent to -3 "
        << "under mod_lesser." << endl;
}
```

## <a name="copy"></a>  copy

Присваивает значения элементов из исходного диапазона диапазону назначения, выполняя итерации в исходной последовательности элементов и присваивая им новые позиции в прямом направлении.

```cpp
template<class InputIterator, class OutputIterator>
OutputIterator copy(
    InputIterator first,
    InputIterator last,
    OutputIterator destBeg);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Итератор ввода, обращающийся к позиции первого элемента в исходном диапазоне.

*последний*<br/>
Итератор ввода, обращающийся к позиции, которая на единицу превышает позицию завершающего элемента в исходном диапазоне.

*destBeg*<br/>
Итератор вывода указывает на позицию первого элемента в диапазоне назначения.

### <a name="return-value"></a>Возвращаемое значение

Выходной итератор, указывающий положение, следующее за последним элементом в диапазоне назначения, то есть, данный итератор обращается `result` + (*последнего* - *первый*).

### <a name="remarks"></a>Примечания

Диапазон источника должен быть допустимым, а в месте назначения должно быть достаточно свободного пространства для всех скопированных элементов.

Так как алгоритм копирует исходные элементы в порядке, начиная с первого элемента, диапазон назначения может перекрывать исходный диапазон *последнего* позиции исходного диапазона не содержится в месте назначения диапазон. `copy` можно использовать для сдвигания элементов влево, но не вправо, если исходный и конечный диапазоны не перекрываются. Для сдвига вправо на любое количество позиций используйте алгоритм [copy_backward](../standard-library/algorithm-functions.md#copy_backward).

Алгоритм `copy` изменяет только значения, на которые указывают итераторы, задавая новые значения элементам в диапазоне назначения. Его нельзя использовать для создания новых элементов и для вставки элементов напрямую в пустой контейнер.

### <a name="example"></a>Пример

```cpp
// alg_copy.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <iostream>

int main() {
   using namespace std;
   vector <int> v1, v2;
   vector <int>::iterator Iter1, Iter2;

   int i;
   for ( i = 0 ; i <= 5 ; i++ )
      v1.push_back( 10 * i );

   int ii;
   for ( ii = 0 ; ii <= 10 ; ii++ )
      v2.push_back( 3 * ii );

   cout << "v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;

   cout << "v2 = ( " ;
   for ( Iter2 = v2.begin( ) ; Iter2 != v2.end( ) ; Iter2++ )
      cout << *Iter2 << " ";
   cout << ")" << endl;

   // To copy the first 3 elements of v1 into the middle of v2
   copy( v1.begin( ), v1.begin( ) + 3, v2.begin( ) + 4 );

   cout << "v2 with v1 insert = ( " ;
   for ( Iter2 = v2.begin( ) ; Iter2 != v2.end( ) ; Iter2++ )
      cout << *Iter2 << " ";
   cout << ")" << endl;

   // To shift the elements inserted into v2 two positions
   // to the left
   copy( v2.begin( )+4, v2.begin( ) + 7, v2.begin( ) + 2 );

   cout << "v2 with shifted insert = ( " ;
   for ( Iter2 = v2.begin( ) ; Iter2 != v2.end( ) ; Iter2++ )
      cout << *Iter2 << " ";
   cout << ")" << endl;
}
```

```Output
v1 = ( 0 10 20 30 40 50 )
v2 = ( 0 3 6 9 12 15 18 21 24 27 30 )
v2 with v1 insert = ( 0 3 6 9 0 10 20 21 24 27 30 )
v2 with shifted insert = ( 0 3 0 10 20 10 20 21 24 27 30 )
```

## <a name="copy_backward"></a>  copy_backward

Присваивает значения элементов из исходного диапазона диапазону назначения, выполняя итерации в исходной последовательности элементов и присваивая им новые позиции в обратном направлении.

```cpp
template<class BidirectionalIterator1, class BidirectionalIterator2>
BidirectionalIterator2 copy_backward(
    BidirectionalIterator1 first,
    BidirectionalIterator1 last,
    BidirectionalIterator2 destEnd);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Двунаправленный итератор, обращающийся к положению первого элемента в исходном диапазоне.

*последний*<br/>
Двунаправленный итератор, обращающийся к позиции, которая на единицу превышает позицию завершающего элемента в исходном диапазоне.

*destEnd*<br/>
Двунаправленный итератор, обращающийся к позиции, которая на единицу превышает позицию завершающего элемента в диапазоне назначения.

### <a name="return-value"></a>Возвращаемое значение

Выходной итератор, указывающий положение, следующее за последним элементом в диапазоне назначения, то есть, данный итератор обращается *destEnd* -(*последнего* - *первый*).

### <a name="remarks"></a>Примечания

Диапазон источника должен быть допустимым, а в месте назначения должно быть достаточно свободного пространства для всех скопированных элементов.

Алгоритм `copy_backward` обладает более строгими требованиями, чем алгоритм копирования. Его итераторы ввода и вывода должны быть двунаправленными.

Алгоритмы `copy_backward` и [move_backward](../standard-library/algorithm-functions.md#move_backward) — единственные алгоритмы в библиотеке стандартных программ C++, назначающие выходной диапазон с итератором, указывающим на конец диапазона назначения.

Так как алгоритм копирует исходные элементы в порядке, начиная с последнего элемента, диапазон назначения может перекрывать исходный диапазон *первый* положение исходного диапазона не содержится в месте назначения диапазон. `copy_backward` можно использовать для сдвигания элементов вправо, но не влево, кроме случаев, когда исходный диапазон и диапазон назначения перекрывают друг друга. Для сдвига влево на любое количество позиций используйте алгоритм [copy](../standard-library/algorithm-functions.md#copy).

Алгоритм `copy_backward` изменяет только значения, на которые указывают итераторы, задавая новые значения элементам в диапазоне назначения. Его нельзя использовать для создания новых элементов и для вставки элементов напрямую в пустой контейнер.

### <a name="example"></a>Пример

```cpp
// alg_copy_bkwd.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <iostream>

int main() {
   using namespace std;
   vector <int> v1, v2;
   vector <int>::iterator Iter1, Iter2;

   int i;
   for ( i = 0 ; i <= 5 ; ++i )
      v1.push_back( 10 * i );

   int ii;
   for ( ii = 0 ; ii <= 10 ; ++ii )
      v2.push_back( 3 * ii );

   cout << "v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; ++Iter1 )
      cout << *Iter1 << " ";
   cout << ")" << endl;

   cout << "v2 = ( " ;
   for ( Iter2 = v2.begin( ) ; Iter2 != v2.end( ) ; ++Iter2 )
      cout << *Iter2 << " ";
   cout << ")" << endl;

   // To copy_backward the first 3 elements of v1 into the middle of v2
   copy_backward( v1.begin( ), v1.begin( ) + 3, v2.begin( ) + 7 );

   cout << "v2 with v1 insert = ( " ;
   for ( Iter2 = v2.begin( ) ; Iter2 != v2.end( ) ; ++Iter2 )
      cout << *Iter2 << " ";
   cout << ")" << endl;

   // To shift the elements inserted into v2 two positions
   // to the right
   copy_backward( v2.begin( )+4, v2.begin( ) + 7, v2.begin( ) + 9 );

   cout << "v2 with shifted insert = ( " ;
   for ( Iter2 = v2.begin( ) ; Iter2 != v2.end( ) ; ++Iter2 )
      cout << *Iter2 << " ";
   cout << ")" << endl;
}
```

## <a name="copy_if"></a>  copy_if

Копирует диапазон элементов, элементы, которые являются **true** заданного условия.

```cpp
template<class InputIterator, class OutputIterator, class BinaryPredicate>
OutputIterator copy_if(
    InputIterator first,
    InputIterator last,
    OutputIterator dest,
    Predicate pred);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Входной итератор, указывающий начало диапазона для проверки условия.

*последний*<br/>
Входной итератор, указывающий конец диапазона.

*dest*<br/>
Выходной итератор, указывающий место назначения для скопированных элементов.

*_Pred*<br/>
Условие, на соответствие которому проверяется каждый элемент в диапазоне. Это условие предоставляется определенным пользователем объектом функции предиката. Предикат принимает один аргумент и возвращает **true** или **false**.

### <a name="return-value"></a>Возвращаемое значение

Выходной итератор, который равен *dest* единицу после каждого элемента, удовлетворяющего условию. Другими словами, возвращаемое значение минус *dest* равно количеству скопированных элементов.

### <a name="remarks"></a>Примечания

Функция шаблона проверяет

`if (pred(*_First + N)) * dest++ = *(_First + N))`

один раз для каждого `N` в диапазоне `[0, last - first)` строго на увеличение значений `N`, начиная с наименьшего значения. Если *dest* и *первый* обозначают области хранилища, *dest* не должны находиться в диапазоне `[ first, last )`.

## <a name="copy_n"></a>  copy_n

Копирует указанное количество элементов.

```cpp
template<class InputIterator, class Size, class OutputIterator>
OutputIterator copy_n(
    InputIterator first,
    Size count,
    OutputIterator dest);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Входной итератор, указывающий, откуда копировать элементы.

*count*<br/>
Целое число со знаком или без знака, указывающее количество копируемых элементов.

*dest*<br/>
Выходной итератор, указывающий, куда копировать элементы.

### <a name="return-value"></a>Возвращаемое значение

Возвращает выходной итератор, куда были скопированы элементы. Он совпадает со значением возвращаемое значение третьего параметра *dest*.

### <a name="remarks"></a>Примечания

Функция шаблона проверяет `*(dest + N) = *(first + N))` один раз для каждого `N` в диапазоне `[0, count)`, строго на увеличение значений `N` начиная с наименьшего значения. Затем оно возвращает значение `dest + N`. Если *dest* и *первый* обозначают области хранилища, *dest* не должны находиться в диапазоне `[first, last)`.

## <a name="count"></a>  count

Возвращает количество элементов в диапазоне, значения которых соответствуют заданному значению.

```cpp
template<class InputIterator, class Type>
typename iterator_traits<InputIterator>::difference_type count(
    InputIterator first,
    InputIterator last,
    const Type& val);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Входной итератор, адресующий положение первого элемента в диапазоне для прохода.

*последний*<br/>
Входной итератор, указывающий позицию, следующую за последним элементом в диапазоне для прохода.

*Val*<br/>
Значение элементов для подсчета.

### <a name="return-value"></a>Возвращаемое значение

Тип различия `InputIterator` , подсчитывает количество элементов в диапазоне [ *первый*, *последнего* ), имеющий значение *val*.

### <a name="remarks"></a>Примечания

`operator==`, используемый для определения совпадения между элементом и указанным значением, должен применять отношение эквивалентности между своими операндами.

Этот алгоритм обобщается для подсчета элементов, которые соответствуют любому предикату, с помощью функции шаблона [count_if](../standard-library/algorithm-functions.md#count_if).

### <a name="example"></a>Пример

```cpp
// alg_count.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <iostream>

int main()
{
    using namespace std;
    vector<int> v1;
    vector<int>::iterator Iter;

    v1.push_back(10);
    v1.push_back(20);
    v1.push_back(10);
    v1.push_back(40);
    v1.push_back(10);

    cout << "v1 = ( " ;
    for (Iter = v1.begin(); Iter != v1.end(); Iter++)
        cout << *Iter << " ";
    cout << ")" << endl;

    vector<int>::iterator::difference_type result;
    result = count(v1.begin(), v1.end(), 10);
    cout << "The number of 10s in v2 is: " << result << "." << endl;
}
```

```Output
v1 = ( 10 20 10 40 10 )
The number of 10s in v2 is: 3.
```

## <a name="count_if"></a>  count_if

Возвращает количество элементов в диапазоне, значения которых соответствуют заданному условию.

```cpp
template<class InputIterator, class Predicate>
typename iterator_traits<InputIterator>::difference_type count_if(
    InputIterator first,
    InputIterator last,
    Predicate pred);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Входной итератор, адресующий положение первого элемента в диапазоне для поиска.

*последний*<br/>
Входной итератор, адресующий положение на единицу после последнего элемента в диапазоне для поиска.

*_Pred*<br/>
Определенный пользователем объект функции предиката, задающий условие, которое должно удовлетворяться, чтобы элемент был подсчитан. Предикат принимает один аргумент и возвращает значение **true** или **false**.

### <a name="return-value"></a>Возвращаемое значение

Количество элементов, которые удовлетворяют условию, заданному предикатом.

### <a name="remarks"></a>Примечания

Эта функция шаблона представляет собой обобщение алгоритма [count](../standard-library/algorithm-functions.md#count) с заменой предиката "равно определенному значению" на любой предикат.

### <a name="example"></a>Пример

```cpp
// alg_count_if.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <iostream>

bool greater10(int value)
{
    return value > 10;
}

int main()
{
    using namespace std;
    vector<int> v1;
    vector<int>::iterator Iter;

    v1.push_back(10);
    v1.push_back(20);
    v1.push_back(10);
    v1.push_back(40);
    v1.push_back(10);

    cout << "v1 = ( ";
    for (Iter = v1.begin(); Iter != v1.end(); Iter++)
        cout << *Iter << " ";
    cout << ")" << endl;

    vector<int>::iterator::difference_type result1;
    result1 = count_if(v1.begin(), v1.end(), greater10);
    cout << "The number of elements in v1 greater than 10 is: "
         << result1 << "." << endl;
}
```

```Output
v1 = ( 10 20 10 40 10 )
The number of elements in v1 greater than 10 is: 2.
```

## <a name="equal"></a>  equal

Сравнивает два диапазона поэлементно на признак равенства или равноценности в смысле, заданном бинарным предикатом.

Используйте функцию `std::equal` при сравнении элементов в контейнерах разного типа (например, в `vector` и `list`), или при сравнении элементов разного типа, или когда необходимо сравнить поддиапазоны контейнеров. При сравнении элементов одного типа в контейнерах одного типа используйте оператор `operator==`, предоставляемый для каждого контейнера.

Используйте двух-диапазонные перегрузки в коде C++ 14. Перегрузки, использующие только один итератор для второго диапазона, не обнаруживают различия в тех случаях, когда второй диапазон длиннее, чем первый, и их поведение может быть непредсказуемо, если второй диапазон короче, чем первый.

```cpp
template<class InputIterator1, class InputIterator2>
bool equal(
    InputIterator1  First1,
    InputIterator1  Last1,
    InputIterator2  First2);

template<class InputIterator1, class InputIterator2, class BinaryPredicate>
bool equal(
    InputIterator1  First1,
    InputIterator1  Last1,
    InputIterator2  First2,
    BinaryPredicate Comp); // C++14

template<class InputIterator1, class InputIterator2>
bool equal(
    InputIterator1  First1,
    InputIterator1  Last1,
    InputIterator2  First2,
    InputIterator2  Last2);

template<class InputIterator1, class InputIterator2, class BinaryPredicate>
bool equal(
    InputIterator1  First1,
    InputIterator1  Last1,
    InputIterator2  First2,
    InputIterator2  Last2,
    BinaryPredicate Comp);
```

### <a name="parameters"></a>Параметры

*first1*<br/>
Входной итератор, указывающий на положение первого элемента в первом диапазоне для тестирования.

*last1*<br/>
Входной итератор, указывающий на положение, следующее за последним элементом, в первом диапазоне для тестирования.

*first2*<br/>
Входной итератор, указывающий на положение первого элемента во втором диапазоне для тестирования.

*first2*<br/>
Входной итератор, указывающий на положение, следующее за последним элементом, во втором диапазоне для тестирования.

*Зап.*<br/>
Заданный пользователем объект функции предиката, определяющий условие, которое должно выполняться, чтобы два элемента считались эквивалентными друг другу. Двоичный предикат принимает два аргумента и возвращает **true** , если условие удовлетворено, или **false** , если условие не удовлетворено.

### <a name="return-value"></a>Возвращаемое значение

Значение **true** в том и только в том случае, когда диапазоны идентичны или эквивалентны в смысле, заданном бинарным предикатом, при поэлементном сравнении. В противном случае — значение **false**.

### <a name="remarks"></a>Примечания

Диапазон, по которому ведется поиск, должен быть допустимым. Все итераторы должны поддерживать сброс ссылок и должна быть возможность достижения последнего положения, начиная от первого, путем приращения.

Если два диапазона имеют одинаковую длину, то временная сложность алгоритма линейно зависит от числа элементов в диапазоне. В противном случае функция немедленно возвращает **false**.

Ни `operator==`, ни определяемый пользователем предикат не требуется применять для наложения отношения эквивалентности (симметричной, рефлексивной и транзитивной) между операндами.

### <a name="example"></a>Пример

```cpp
#include <iostream>
#include <vector>
#include <algorithm>

using namespace std;

int main()
{
    vector<int> v1 { 0, 5, 10, 15, 20, 25 };
    vector<int> v2 { 0, 5, 10, 15, 20, 25 };
    vector<int> v3 { 0, 5, 10, 15, 20, 25, 30, 35, 40, 45, 50 };

    // Using range-and-a-half equal:
    bool b = equal(v1.begin(), v1.end(), v2.begin());
    cout << "v1 and v2 are equal: "
       << b << endl; // true, as expected

    b = equal(v1.begin(), v1.end(), v3.begin());
    cout << "v1 and v3 are equal: "
       << b << endl; // true, surprisingly

    // Using dual-range equal:
    b = equal(v1.begin(), v1.end(), v3.begin(), v3.end());
    cout << "v1 and v3 are equal with dual-range overload: "
       << b << endl; // false

    return 0;
}

```

## <a name="equal_range"></a>  equal_range

Принимая во внимание упорядоченный диапазон, находит поддиапазон, в котором все элементы эквивалентны заданному значению.

```cpp
template<class ForwardIterator, class Type>
pair<ForwardIterator, ForwardIterator> equal_range(
    ForwardIterator first,
    ForwardIterator last,
    const Type& val);

template<class ForwardIterator, class Type, class Predicate>
pair<ForwardIterator, ForwardIterator> equal_range(
    ForwardIterator first,
    ForwardIterator last,
    const Type& val,
    Predicate comp);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Прямой итератор, адресующий положение первого элемента в диапазоне для поиска.

*последний*<br/>
Прямой итератор, адресующий положение на единицу после последнего элемента в диапазоне для поиска.

*Val*<br/>
Значение для поиска в упорядоченном диапазоне.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, задающий условие, когда один элемент меньше другого.

### <a name="return-value"></a>Возвращаемое значение

Пара прямых итераторов, задающих поддиапазон в искомом диапазоне, в которых все элементы эквивалентны *val* в смысле, заданном используемым двоичным предикатом (либо *comp* или значение по умолчанию, менее-чем).

Если ни один элемент в диапазоне эквивалентны *val*, возвращенной паре прямых итератора равны и указывают точку, где *val* удалось вставить не нарушая порядок диапазона.

### <a name="remarks"></a>Примечания

Первый итератор из пары, возвращаемой алгоритмом, — это [lower_bound](../standard-library/algorithm-functions.md#lower_bound), а второй итератор — [upper_bound](../standard-library/algorithm-functions.md#upper_bound).

Диапазон должен быть упорядочен согласно предикату, предоставленному в `equal_range`. Например, если вы собираетесь использовать предикат "больше чем", диапазон должен быть отсортирован в порядке убывания.

Элементы в возможно пустой поддиапазон, определяется парой итераторов, возвращенных `equal_range` считается эквивалентным *val* в смысле, заданном используемым предикатом.

Сложность алгоритма является логарифмической для итераторов произвольного доступа и линейной в противном случае с числом шагов, пропорциональным значению (*последнего* - *первый*).

### <a name="example"></a>Пример

```cpp
// alg_equal_range.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <functional>      // greater<int>()
#include <iostream>
#include <string>
using namespace std;

template<class T> void dump_vector( const vector<T>& v, pair<typename vector<T>::iterator, typename vector<T>::iterator> range )
{
    // prints vector v with range delimited by [ and ]

    for ( typename vector<T>::const_iterator i = v.begin(); i != v.end(); ++i )
    {
        if ( i == range.first )
        {
            cout << "[ ";
        }
        if ( i == range.second )
        {
            cout << "] ";
        }

        cout << *i << " ";
    }
    cout << endl;
}

template<class T> void equal_range_demo( const vector<T>& original_vector, T val )
{
    vector<T> v(original_vector);

    sort( v.begin(), v.end() );
    cout << "Vector sorted by the default binary predicate <:" << endl << '\t';
    for ( vector<T>::const_iterator i = v.begin(); i != v.end(); ++i )
    {
        cout << *i << " ";
    }
    cout << endl << endl;

    pair<vector<T>::iterator, vector<T>::iterator> result
        = equal_range( v.begin(), v.end(), val );

    cout << "Result of equal_range with val = " << val << ":" << endl << '\t';
    dump_vector( v, result );
    cout << endl;
}

template<class T, class F> void equal_range_demo( const vector<T>& original_vector, T val, F pred, string predname )
{
    vector<T> v(original_vector);

    sort( v.begin(), v.end(), pred );
    cout << "Vector sorted by the binary predicate " << predname << ":" << endl << '\t';
    for ( typename vector<T>::const_iterator i = v.begin(); i != v.end(); ++i )
    {
        cout << *i << " ";
    }
    cout << endl << endl;

    pair<typename vector<T>::iterator, typename vector<T>::iterator> result
        = equal_range( v.begin(), v.end(), val, pred );

    cout << "Result of equal_range with val = " << val << ":" << endl << '\t';
    dump_vector( v, result );
    cout << endl;
}

// Return whether absolute value of elem1 is less than absolute value of elem2
bool abs_lesser( int elem1, int elem2 )
{
    return abs(elem1) < abs(elem2);
}

// Return whether string l is shorter than string r
bool shorter_than(const string& l, const string& r)
{
    return l.size() < r.size();
}

int main()
{
    vector<int> v1;

    // Constructing vector v1 with default less than ordering
    for ( int i = -1; i <= 4; ++i )
    {
        v1.push_back(i);
    }

    for ( int i =-3; i <= 0; ++i )
    {
        v1.push_back( i );
    }

    equal_range_demo( v1, 3 );
    equal_range_demo( v1, 3, greater<int>(), "greater" );
    equal_range_demo( v1, 3, abs_lesser, "abs_lesser" );

    vector<string> v2;

    v2.push_back("cute");
    v2.push_back("fluffy");
    v2.push_back("kittens");
    v2.push_back("fun");
    v2.push_back("meowmeowmeow");
    v2.push_back("blah");

    equal_range_demo<string>( v2, "fred" );
    equal_range_demo<string>( v2, "fred", shorter_than, "shorter_than" );
}

```

## <a name="fill"></a>  fill

Присваивает одно и то же новое значение каждому элементу в заданном диапазоне.

```cpp
template<class ForwardIterator, class Type>
void fill(
    ForwardIterator first,
    ForwardIterator last,
    const Type& val);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Прямой итератор, указывающий на позицию первого элемента в диапазоне для прохода.

*последний*<br/>
Прямой итератор, указывающий на позицию, следующую за последним элементом в диапазоне для прохода.

*Val*<br/>
Значение, которое назначается элементам в диапазоне [ *первый*, *последнего*).

### <a name="remarks"></a>Примечания

Целевой диапазон должен быть допустимым; все указатели должны поддерживать сброс ссылок; должна быть возможность достижения последнего положения с первого путем приращения. Сложность линейная по отношению к размеру диапазона.

### <a name="example"></a>Пример

```cpp
// alg_fill.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <iostream>

int main()
{
   using namespace std;
   vector <int> v1;
   vector <int>::iterator Iter1;

   int i;
   for ( i = 0 ; i <= 9 ; i++ )
   {
      v1.push_back( 5 * i );
   }

   cout << "Vector v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;

   // Fill the last 5 positions with a value of 2
   fill( v1.begin( ) + 5, v1.end( ), 2 );

   cout << "Modified v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;
}
```

```Output
Vector v1 = ( 0 5 10 15 20 25 30 35 40 45 )
Modified v1 = ( 0 5 10 15 20 2 2 2 2 2 )
```

## <a name="fill_n"></a>  fill_n

Назначает новое значение указанному количеству элементов в диапазоне, начиная с определенного элемента.

```cpp
template<class OutputIterator, class Size, class Type>
OutputIterator fill_n(
    OutputIterator First,
    Size Count,
    const Type& Val);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Выходной итератор, указывающий позицию первого элемента в диапазоне присваиваемое значение *Val*.

*Количество*<br/>
Целое число со знаком или без знака, указывающее количество элементов, которым следует назначить значение.

*Val*<br/>
Значение, которое назначается элементам в диапазоне [ *первый*, *First + Count*).

### <a name="return-value"></a>Возвращаемое значение

Заполнить итератор, указывающий на элемент, следующий за последним элементом в случае, если *число* > ноль, в противном случае первый элемент.

### <a name="remarks"></a>Примечания

Целевой диапазон должен быть допустимым; все указатели должны поддерживать сброс ссылок; должна быть возможность достижения последнего положения с первого путем приращения. Сложность линейная по отношению к размеру диапазона.

### <a name="example"></a>Пример

```cpp
// alg_fill_n.cpp
// compile using /EHsc
#include <vector>
#include <algorithm>
#include <iostream>

int main()
{
    using namespace std;
    vector <int> v;

    for ( auto i = 0 ; i < 9 ; ++i )
        v.push_back( 0 );

    cout << "  vector v = ( " ;
    for ( const auto &w : v )
        cout << w << " ";
    cout << ")" << endl;

    // Fill the first 3 positions with a value of 1, saving position.
    auto pos = fill_n( v.begin(), 3, 1 );

    cout << "modified v = ( " ;
    for ( const auto &w : v )
        cout << w << " ";
    cout << ")" << endl;

    // Fill the next 3 positions with a value of 2, using last position.
    fill_n( pos, 3, 2 );

    cout << "modified v = ( " ;
    for ( const auto &w : v )
        cout << w << " ";
    cout << ")" << endl;

    // Fill the last 3 positions with a value of 3, using relative math.
    fill_n( v.end()-3, 3, 3 );

    cout << "modified v = ( " ;
    for ( const auto &w : v )
        cout << w << " ";
    cout << ")" << endl;
}

```

## <a name="find"></a>  find

Находит позицию первого вхождения элемента с заданным значением в диапазон.

```cpp
template<class InputIterator, class T>
InputIterator find(
    InputIterator first,
    InputIterator last,
    const T& val);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Входной итератор, адресующий положение первого элемента в диапазоне для поиска заданного значения.

*последний*<br/>
Входной итератор, адресующий положение после последнего элемента в диапазоне для поиска заданного значения.

*Val*<br/>
Значение, которое нужно найти.

### <a name="return-value"></a>Возвращаемое значение

Входной итератор, адресующий первое вхождение заданного значения в диапазоне, в котором выполняется поиск. Если элемент не найден с эквивалентным значением, возвращает *последнего*.

### <a name="remarks"></a>Примечания

`operator==`, используемый для определения совпадения между элементом и указанным значением, должен применять отношение эквивалентности между своими операндами.

Пример кода с использованием `find()` см. в разделе [find_if](../standard-library/algorithm-functions.md#find_if).

## <a name="find_end"></a>  find_end

Ищет в диапазоне последнюю подпоследовательность, совпадающую с заданной последовательностью, или эквивалентной согласно условию, заданному двоичным предикатом.

```cpp
template<class ForwardIterator1, class ForwardIterator2>
ForwardIterator1 find_end(
    ForwardIterator1 First1,
    ForwardIterator1 Last1,
    ForwardIterator2 First2,
    ForwardIterator2 Last2);

template<class ForwardIterator1, class ForwardIterator2, class Pred>
ForwardIterator1 find_end(
    ForwardIterator1 First1,
    ForwardIterator1 Last1,
    ForwardIterator2 First2,
    ForwardIterator2 Last2,
    Pred Comp);
```

### <a name="parameters"></a>Параметры

*first1*<br/>
Прямой итератор, адресующий положение первого элемента в диапазоне для поиска.

*last1*<br/>
Прямой итератор, указывающий на положение, следующее за последним элементом в диапазоне для поиска.

*first2*<br/>
Прямой итератор, указывающий на положение первого элемента в диапазоне для поиска.

*last2*<br/>
Прямой итератор, указывающий на положение, следующее за последним элементом в диапазоне для поиска.

*Зап.*<br/>
Заданный пользователем объект функции предиката, определяющий условие, которое должно выполняться, чтобы два элемента считались эквивалентными друг другу. Двоичный предикат принимает два аргумента и возвращает **true** , если условие удовлетворено, или **false** , если условие не удовлетворено.

### <a name="return-value"></a>Возвращаемое значение

Прямой итератор, указывающий на положение первого элемента последней подпоследовательности в интервале [First1, Last1), совпадающей с указанной последовательностью [First2, Last2).

### <a name="remarks"></a>Примечания

`operator==`, используемый для определения совпадения между элементом и указанным значением, должен применять отношение эквивалентности между своими операндами.

Диапазоны, на которые указывают ссылки, должны быть допустимыми; все указатели должны поддерживать сброс ссылок; в каждой последовательности должна быть возможность достижения последнего положения с первого путем приращения.

### <a name="example"></a>Пример

```cpp
// alg_find_end.cpp
// compile with: /EHsc
#include <vector>
#include <list>
#include <algorithm>
#include <iostream>

// Return whether second element is twice the first
bool twice ( int elem1, int elem2 )
{
   return 2 * elem1 == elem2;
}

int main()
{
   using namespace std;
   vector <int> v1, v2;
   list <int> L1;
   vector <int>::iterator Iter1, Iter2;
   list <int>::iterator L1_Iter, L1_inIter;

   int i;
   for ( i = 0 ; i <= 5 ; i++ )
   {
      v1.push_back( 5 * i );
   }
   for ( i = 0 ; i <= 5 ; i++ )
   {
      v1.push_back( 5 * i );
   }

   int ii;
   for ( ii = 1 ; ii <= 4 ; ii++ )
   {
      L1.push_back( 5 * ii );
   }

   int iii;
   for ( iii = 2 ; iii <= 4 ; iii++ )
   {
      v2.push_back( 10 * iii );
   }

   cout << "Vector v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;

   cout << "List L1 = ( " ;
   for ( L1_Iter = L1.begin( ) ; L1_Iter!= L1.end( ) ; L1_Iter++ )
      cout << *L1_Iter << " ";
   cout << ")" << endl;

   cout << "Vector v2 = ( " ;
   for ( Iter2 = v2.begin( ) ; Iter2 != v2.end( ) ; Iter2++ )
      cout << *Iter2 << " ";
      cout << ")" << endl;

   // Searching v1 for a match to L1 under identity
   vector <int>::iterator result1;
   result1 = find_end ( v1.begin( ), v1.end( ), L1.begin( ), L1.end( ) );

   if ( result1 == v1.end( ) )
      cout << "There is no match of L1 in v1."
           << endl;
   else
      cout << "There is a match of L1 in v1 that begins at "
           << "position "<< result1 - v1.begin( ) << "." << endl;

   // Searching v1 for a match to L1 under the binary predicate twice
   vector <int>::iterator result2;
   result2 = find_end ( v1.begin( ), v1.end( ), v2.begin( ), v2.end( ), twice );

   if ( result2 == v1.end( ) )
      cout << "There is no match of L1 in v1."
           << endl;
   else
      cout << "There is a sequence of elements in v1 that "
           << "are equivalent to those\n in v2 under the binary "
           << "predicate twice and that begins at position "
           << result2 - v1.begin( ) << "." << endl;
}
```

```Output
Vector v1 = ( 0 5 10 15 20 25 0 5 10 15 20 25 )
List L1 = ( 5 10 15 20 )
Vector v2 = ( 20 30 40 )
There is a match of L1 in v1 that begins at position 7.
There is a sequence of elements in v1 that are equivalent to those
in v2 under the binary predicate twice and that begins at position 8.
```

## <a name="find_first_of"></a>  find_first_of

Выполняет поиск первого вхождения любого из нескольких значений в заданный диапазон или первого вхождения любого из нескольких элементов, равноценных в смысле, заданном бинарным предикатом, в указанный набор элементов.

```cpp
template<class ForwardIterator1, class ForwardIterator2>
ForwardIterator1 find_first_of(
    ForwardIterator1  first1,
    ForwardIterator1 Last1,
    ForwardIterator2  first2,
    ForwardIterator2 Last2);

template<class ForwardIterator1, class ForwardIterator2, class BinaryPredicate>
ForwardIterator1 find_first_of(
    ForwardIterator1  first1,
    ForwardIterator1 Last1,
    ForwardIterator2  first2,
    ForwardIterator2 Last2,
    BinaryPredicate  comp);
```

### <a name="parameters"></a>Параметры

*first1*<br/>
Прямой итератор, адресующий положение первого элемента в диапазоне для поиска.

*last1*<br/>
Прямой итератор, адресующий положение на единицу после последнего элемента в диапазоне для поиска.

*first2*<br/>
Прямой итератор, адресующий положение первого элемента в диапазоне для сравнения.

*last2*<br/>
Прямой итератор, адресующий положение на единицу после последнего элемента в диапазоне для сравнения.

*Зап.*<br/>
Заданный пользователем объект функции предиката, определяющий условие, которое должно выполняться, чтобы два элемента считались эквивалентными друг другу. Двоичный предикат принимает два аргумента и возвращает **true** , если условие удовлетворено, или **false** , если условие не удовлетворено.

### <a name="return-value"></a>Возвращаемое значение

Прямой итератор, адресующий положение первого элемента первой последовательности, совпадающей с определенной последовательностью или эквивалентной согласно условию, заданному двоичным предикатом.

### <a name="remarks"></a>Примечания

`operator==`, используемый для определения совпадения между элементом и указанным значением, должен применять отношение эквивалентности между своими операндами.

Диапазоны, на которые указывают ссылки, должны быть допустимыми; все указатели должны поддерживать сброс ссылок; в каждой последовательности должна быть возможность достижения последнего положения с первого путем приращения.

### <a name="example"></a>Пример

```cpp
// alg_find_first_of.cpp
// compile with: /EHsc
#include <vector>
#include <list>
#include <algorithm>
#include <iostream>

// Return whether second element is twice the first
bool twice ( int elem1, int elem2 )
{
   return 2 * elem1 == elem2;
}

int main()
{
   using namespace std;
   vector <int> v1, v2;
   list <int> L1;
   vector <int>::iterator Iter1, Iter2;
   list <int>::iterator L1_Iter, L1_inIter;

   int i;
   for ( i = 0 ; i <= 5 ; i++ )
   {
      v1.push_back( 5 * i );
   }
   for ( i = 0 ; i <= 5 ; i++ )
   {
      v1.push_back( 5 * i );
   }

   int ii;
   for ( ii = 3 ; ii <= 4 ; ii++ )
   {
      L1.push_back( 5 * ii );
   }

   int iii;
   for ( iii = 2 ; iii <= 4 ; iii++ )
   {
      v2.push_back( 10 * iii );
   }

   cout << "Vector v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;

   cout << "List L1 = ( " ;
   for ( L1_Iter = L1.begin( ) ; L1_Iter!= L1.end( ) ; L1_Iter++ )
      cout << *L1_Iter << " ";
   cout << ")" << endl;

   cout << "Vector v2 = ( " ;
   for ( Iter2 = v2.begin( ) ; Iter2 != v2.end( ) ; Iter2++ )
      cout << *Iter2 << " ";
      cout << ")" << endl;

   // Searching v1 for first match to L1 under identity
   vector <int>::iterator result1;
   result1 = find_first_of ( v1.begin( ), v1.end( ), L1.begin( ), L1.end( ) );

   if ( result1 == v1.end( ) )
      cout << "There is no match of L1 in v1."
           << endl;
   else
      cout << "There is at least one match of L1 in v1"
           << "\n and the first one begins at "
           << "position "<< result1 - v1.begin( ) << "." << endl;

   // Searching v1 for a match to L1 under the binary predicate twice
   vector <int>::iterator result2;
   result2 = find_first_of ( v1.begin( ), v1.end( ), v2.begin( ), v2.end( ), twice );

   if ( result2 == v1.end( ) )
      cout << "There is no match of L1 in v1."
           << endl;
   else
      cout << "There is a sequence of elements in v1 that "
           << "are equivalent\n to those in v2 under the binary "
           << "predicate twice\n and the first one begins at position "
           << result2 - v1.begin( ) << "." << endl;
}
```

```Output
Vector v1 = ( 0 5 10 15 20 25 0 5 10 15 20 25 )
List L1 = ( 15 20 )
Vector v2 = ( 20 30 40 )
There is at least one match of L1 in v1
and the first one begins at position 3.
There is a sequence of elements in v1 that are equivalent
to those in v2 under the binary predicate twice
and the first one begins at position 2.
```

## <a name="find_if"></a>  find_if

Находит позицию первого вхождения элемента, удовлетворяющего определенному условию, в диапазон.

```cpp
template<class InputIterator, class Predicate>
InputIterator find_if(
    InputIterator first,
    InputIterator last,
    Predicate pred);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Входной итератор, адресующий положение первого элемента в диапазоне для поиска.

*последний*<br/>
Входной итератор, адресующий положение на единицу после последнего элемента в диапазоне для поиска.

*Пред*<br/>
Определенный пользователем объект функции предиката или [лямбда-выражение](../cpp/lambda-expressions-in-cpp.md), определяющее условие, которому должен соответствовать искомый элемент. Предикат принимает один аргумент и возвращает **true** (выполняется) или **false** (не выполнено). Подпись *pred* должна быть `bool pred(const T& arg);`, где `T` — это тип, к которому `InputIterator` может быть неявно преобразован при разыменовании. **Const** ключевое слово, отображается только для демонстрации того, что объект функции или лямбда не должен изменять аргумент.

### <a name="return-value"></a>Возвращаемое значение

Входной итератор, ссылающийся на первый элемент в диапазоне, удовлетворяющий условию, заданному предикатом (результат предиката **true**). Если элемент не найден для удовлетворяют предикату, возвращает *последнего*.

### <a name="remarks"></a>Примечания

Эта функция шаблона представляет собой обобщение алгоритма [find](../standard-library/algorithm-functions.md#find) с заменой предиката "равно определенному значению" на любой предикат. Сведения о противоположной по назначению функции (которая находит первый элемент, не удовлетворяющий условию предиката), см. в разделе [find_if_not](../standard-library/algorithm-functions.md#find_if_not).

### <a name="example"></a>Пример

```cpp
// cl.exe /W4 /nologo /EHsc /MTd
#include <vector>
#include <algorithm>
#include <iostream>
#include <string>

using namespace std;

template <typename S> void print(const S& s) {
for (const auto& p : s) {
        cout << "(" << p << ") ";
    }
    cout << endl;
}

// Test std::find()
template <class InputIterator, class T>
void find_print_result(InputIterator first, InputIterator last, const T& value) {

    // call <algorithm> std::find()
    auto p = find(first, last, value);

    cout << "value " << value;
    if (p == last) {
        cout << " not found." << endl;
    } else {
        cout << " found." << endl;
    }
}

// Test std::find_if()
template <class InputIterator, class Predicate>
void find_if_print_result(InputIterator first, InputIterator last,
    Predicate Pred, const string& Str) {

    // call <algorithm> std::find_if()
    auto p = find_if(first, last, Pred);

    if (p == last) {
        cout << Str << " not found." << endl;
    } else {
        cout << "first " << Str << " found: " << *p << endl;
    }
}

// Function to use as the UnaryPredicate argument to find_if() in this example
bool is_odd_int(int i) {
    return ((i % 2) != 0);
}

int main()
{
    // Test using a plain old array.
    const int x[] = { 1, 2, 3, 4, 5, 6, 7, 8, 9, 10 };
    cout << "array x[] contents: ";
    print(x);
    // Using non-member std::begin()/std::end() to get input iterators for the plain old array.
    cout << "Test std::find() with array..." << endl;
    find_print_result(begin(x), end(x), 10);
    find_print_result(begin(x), end(x), 42);
    cout << "Test std::find_if() with array..." << endl;
    find_if_print_result(begin(x), end(x), is_odd_int, "odd integer"); // function name
    find_if_print_result(begin(x), end(x), // lambda
        [](int i){ return ((i % 2) == 0); }, "even integer");

    // Test using a vector.
    vector<int> v;
    for (int i = 0; i < 10; ++i) {
        v.push_back((i + 1) * 10);
    }
    cout << endl << "vector v contents: ";
    print(v);
    cout << "Test std::find() with vector..." << endl;
    find_print_result(v.begin(), v.end(), 20);
    find_print_result(v.begin(), v.end(), 12);
    cout << "Test std::find_if() with vector..." << endl;
    find_if_print_result(v.begin(), v.end(), is_odd_int, "odd integer");
    find_if_print_result(v.begin(), v.end(), // lambda
        [](int i){ return ((i % 2) == 0); }, "even integer");
}

```

## <a name="find_if_not"></a>  find_if_not

Возвращает первый элемент, который не удовлетворяет условию, в указанном диапазоне.

```cpp
template<class InputIterator, class Predicate>
InputIterator find_if_not(
    InputIterator first,
    InputIterator last,
    Predicate pred);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Входной итератор, адресующий положение первого элемента в диапазоне для поиска.

*последний*<br/>
Входной итератор, адресующий положение на единицу после последнего элемента в диапазоне для поиска.

*Пред*<br/>
Определенный пользователем объект функции предиката или [лямбда-выражение](../cpp/lambda-expressions-in-cpp.md), определяющее условие, которому не должен соответствовать искомый элемент. Предикат принимает один аргумент и возвращает **true** (выполняется) или **false** (не выполнено). Подпись *pred* должна быть `bool pred(const T& arg);`, где `T` — это тип, к которому `InputIterator` может быть неявно преобразован при разыменовании. **Const** ключевое слово, отображается только для демонстрации того, что объект функции или лямбда не должен изменять аргумент.

### <a name="return-value"></a>Возвращаемое значение

Входной итератор, ссылающийся на первый элемент в диапазоне, который не удовлетворяет условию, заданному предикатом (результат предиката **false**). Если все элементы удовлетворяют предикату (результат предиката **true** для каждого элемента), возвращает *последнего*.

### <a name="remarks"></a>Примечания

Эта функция шаблона представляет собой обобщение алгоритма [find](../standard-library/algorithm-functions.md#find) с заменой предиката "равно определенному значению" на любой предикат. Сведения о противоположной по назначению функции (которая находит первый элемент, удовлетворяющий условию предиката), см. в разделе [find_if](../standard-library/algorithm-functions.md#find_if).

Пример кода, готовый для адаптации к `find_if_not()`, см. в разделе [find_if](../standard-library/algorithm-functions.md#find_if).

## <a name="for_each"></a>  for_each

Применяет заданный объект функции к каждому элементу в прямом порядке в пределах диапазона и возвращает объект функции.

```cpp
template<class InputIterator, class Function>
Function for_each(
    InputIterator first,
    InputIterator last,
    Function func);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Итератор ввода содержит позицию первого элемента из нужного диапазона.

*последний*<br/>
Итератор ввода содержит положение элемента, стоящего за последним рассматриваемым элементом в нужном диапазоне.

*_Func*<br/>
Определенный пользователем объект функции, который применяется к каждому элементу в диапазоне.

### <a name="return-value"></a>Возвращаемое значение

Копия объекта функции после того, как он будет применён ко всем элементам в диапазоне.

### <a name="remarks"></a>Примечания

Алгоритм `for_each` весьма гибок, что позволяет изменять каждый элемент в пределах диапазона разными способами, определенными пользователем. Шаблонизируемые функции могут использоваться многократно в измененной форме путем передачи разных параметров. Определяемые пользователем функции могут накапливать сведения во внутреннем состоянии, которое может возвращать алгоритм после обработки всех элементов в диапазоне.

Указанный диапазон должен быть допустимым. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Отношение сложности линейное с не более ( *последнего* -  *первый*) сравнений.

### <a name="example"></a>Пример

```cpp
// alg_for_each.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <iostream>

// The function object multiplies an element by a Factor
template <class Type>
class MultValue
{
private:
   Type Factor;   // The value to multiply by
public:
   // Constructor initializes the value to multiply by
   MultValue ( const Type& val ) : Factor ( val ) {
   }

   // The function call for the element to be multiplied
   void operator( ) ( Type& elem ) const
   {
      elem *= Factor;
   }
};

// The function object to determine the average
class Average
{
private:
   long num;      // The number of elements
   long sum;      // The sum of the elements
public:
   // Constructor initializes the value to multiply by
   Average( ) : num ( 0 ) , sum ( 0 )
   {
   }

   // The function call to process the next elment
   void operator( ) ( int elem ) \
   {
      num++;      // Increment the element count
      sum += elem;   // Add the value to the partial sum
   }

   // return Average
   operator double( )
   {
      return  static_cast <double> (sum) /
      static_cast <double> (num);
   }
};

int main()
{
   using namespace std;
   vector <int> v1;
   vector <int>::iterator Iter1;

   // Constructing vector v1
   int i;
   for ( i = -4 ; i <= 2 ; i++ )
   {
      v1.push_back(  i );
   }

   cout << "Original vector  v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Using for_each to multiply each element by a Factor
   for_each ( v1.begin( ), v1.end( ), MultValue<int> ( -2 ) );

   cout << "Multiplying the elements of the vector v1\n "
        <<  "by the factor -2 gives:\n v1mod1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // The function object is templatized and so can be
   // used again on the elements with a different Factor
   for_each (v1.begin( ), v1.end( ), MultValue<int> (5 ) );

   cout << "Multiplying the elements of the vector v1mod\n "
        <<  "by the factor 5 gives:\n v1mod2 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // The local state of a function object can accumulate
   // information about a sequence of actions that the
   // return value can make available, here the Average
   double avemod2 = for_each ( v1.begin( ), v1.end( ),
      Average( ) );
   cout << "The average of the elements of v1 is:\n Average ( v1mod2 ) = "
        << avemod2 << "." << endl;
}
```

```Output
Original vector  v1 = ( -4 -3 -2 -1 0 1 2 ).
Multiplying the elements of the vector v1
by the factor -2 gives:
v1mod1 = ( 8 6 4 2 0 -2 -4 ).
Multiplying the elements of the vector v1mod
by the factor 5 gives:
v1mod2 = ( 40 30 20 10 0 -10 -20 ).
The average of the elements of v1 is:
Average ( v1mod2 ) = 10.
```

## <a name="generate"></a>  generate

Присваивает значения, создаваемые объектом функции, каждому элементу в диапазоне.

```cpp
template<class ForwardIterator, class Generator>
void generate(
    ForwardIterator first,
    ForwardIterator last,
    Generator _Gen);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Прямой итератор, указывающий позицию первого элемента в диапазоне, которому назначаются значения.

*последний*<br/>
Прямой итератор, указывающий позицию, следующую за последним элементом в диапазоне, которому назначаются значения.

*_Gen*<br/>
Объект функции, который вызывается без аргументов и используется для формирования значений, которые необходимо назначить каждому из элементов в диапазоне.

### <a name="remarks"></a>Примечания

Этот объект функции вызывается для всех элементов в диапазоне; он необязательно должен возвращать одинаковое значение при вызове. Например, он может читать данные из файла или ссылаться на локальное состояние и изменять его. Тип результата должен поддерживать преобразование в тип значения прямых итераторов диапазона.

Указанный диапазон должен быть допустимым. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Отношение сложности линейное, точно ( `last`  -   `first`) вызовов генератора является обязательным.

### <a name="example"></a>Пример

```cpp
// alg_generate.cpp
// compile with: /EHsc
#include <vector>
#include <deque>
#include <algorithm>
#include <iostream>
#include <ostream>

int main()
{
   using namespace std;

   // Assigning random values to vector integer elements
   vector <int> v1 ( 5 );
   vector <int>::iterator Iter1;
   deque <int> deq1 ( 5 );
   deque <int>::iterator d1_Iter;

   generate ( v1.begin( ), v1.end( ), rand );

   cout << "Vector v1 is ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Assigning random values to deque integer elements
   generate ( deq1.begin( ), deq1.end( ), rand );

   cout << "Deque deq1 is ( " ;
   for ( d1_Iter = deq1.begin( ) ; d1_Iter != deq1.end( ) ; d1_Iter++ )
      cout << *d1_Iter << " ";
   cout << ")." << endl;
}
```

```Output
Vector v1 is ( 41 18467 6334 26500 19169 ).
Deque deq1 is ( 15724 11478 29358 26962 24464 ).
```

## <a name="generate_n"></a>  generate_n

Присваивает значения, создаваемые объектом функции, указанному количеству элементов в диапазоне и возвращается на позицию, следующую за последним присвоенным значением.

```cpp
template<class OutputIterator, class Diff, class Generator>
void generate_n(
    OutputIterator First,
    Diff Count,
    Generator Gen);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Выходной итератор, обращающийся к позиции первого элемента в диапазоне, которому назначаются значения.

*Количество*<br/>
Целочисленный тип со знаком или без знака, указывающий количество элементов, которым функция генератора назначит значение.

*Gen*<br/>
Объект функции, который вызывается без аргументов и используется для формирования значений, которые необходимо назначить каждому из элементов в диапазоне.

### <a name="remarks"></a>Примечания

Этот объект функции вызывается для всех элементов в диапазоне; он необязательно должен возвращать одинаковое значение при вызове. Например, он может читать данные из файла или ссылаться на локальное состояние и изменять его. Тип результата должен поддерживать преобразование в тип значения прямых итераторов диапазона.

Указанный диапазон должен быть допустимым. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Отношение сложности линейное, требуется ровно `Count` вызовов генератора.

### <a name="example"></a>Пример

```cpp
// cl.exe /EHsc /nologo /W4 /MTd
#include <vector>
#include <deque>
#include <iostream>
#include <string>
#include <algorithm>
#include <random>

using namespace std;

template <typename C> void print(const string& s, const C& c) {
    cout << s;

    for (const auto& e : c) {
        cout << e << " ";
    }

    cout << endl;
}

int main()
{
    const int elemcount = 5;
    vector<int> v(elemcount);
    deque<int> dq(elemcount);

    // Set up random number distribution
    random_device rd;
    mt19937 engine(rd());
    uniform_int_distribution<int> dist(-9, 9);

    // Call generate_n, using a lambda for the third parameter
    generate_n(v.begin(), elemcount, [&](){ return dist(engine); });
    print("vector v is: ", v);

    generate_n(dq.begin(), elemcount, [&](){ return dist(engine); });
    print("deque dq is: ", dq);
}

```

## <a name="includes"></a>  includes

Проверяет, содержит ли один отсортированный диапазон все элементы, содержащиеся во втором отсортированном диапазоне, где порядок сортировки или критерий эквивалентности элементов можно задать бинарным предикатом.

```cpp
template<class InputIterator1, class InputIterator2>
bool includes(
    InputIterator1 first1,
    InputIterator1 last1,
    InputIterator2 first2,
    InputIterator2 last2);

template<class InputIterator1, class InputIterator2, class BinaryPredicate>
bool includes(
    InputIterator1 first1,
    InputIterator1 last1,
    InputIterator2 first2,
    InputIterator2 last2,
    BinaryPredicate comp );
```

### <a name="parameters"></a>Параметры

*first1*<br/>
Входной итератор, указывающий позицию первого элемента в первом из двух упорядоченных исходных диапазонов, которые должны проверяться на наличие в первом диапазоне всех элементов из второго диапазона.

*last1*<br/>
Входной итератор, указывающий позицию, следующую за последним элементом в первом из двух упорядоченных исходных диапазонов, которые должны проверяться на наличие в первом диапазоне всех элементов из второго диапазона.

*first2*<br/>
Входной итератор, указывающий позицию первого элемента во втором из двух последовательных упорядоченных исходных диапазонов, которые должны проверяться на наличие в первом диапазоне всех элементов из второго диапазона.

*last2*<br/>
Входной итератор, указывающий позицию, следующую за последним элементом во втором из двух последовательных упорядоченных исходных диапазонов, которые должны проверяться на наличие в первом диапазоне всех элементов из второго диапазона.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, задающий условие, когда один элемент меньше другого. Двоичный предикат принимает два аргумента и возвращает **true** , если условие удовлетворено, или **false** , если условие не удовлетворено.

### <a name="return-value"></a>Возвращаемое значение

Значение **true**, если первый упорядоченный диапазон содержит все элементы из второго упорядоченного диапазона; в противном случае — значение **false**.

### <a name="remarks"></a>Примечания

Можно также представить себе этот тест как проверку, является ли второй исходный диапазон подмножеством первого исходного диапазона.

Упорядоченные исходные диапазоны, на которые указывают ссылки, должны быть допустимыми. Все указатели должны поддерживать отмену ссылок. В каждой последовательности должна быть возможность достижения последней позиции с первой путем приращения.

Предварительное условие для применения алгоритма includes состоит в том, что каждый упорядоченный диапазон должен быть упорядочен в соответствии с теми же правилами, которые будут использоваться этим алгоритмом для сортировки объединенных диапазонов.

Алгоритм не изменяет исходные диапазоны `merge`.

В целях упорядочения типы значений входных итераторов должны подлежать сравнению "меньше чем" для установления такого порядка, чтобы, имея два элемента, можно было определить, что они равны (ни один не меньше другого) или что один меньше другого. Это приводит к упорядочению неравнозначных элементов. Точнее, алгоритм проверяет, все ли элементы в первом упорядоченном диапазоне под указанным двоичным предикатом имеют порядок, эквивалентный порядку элементов во втором упорядоченном диапазоне.

Отношение сложности алгоритма линейное более 2 \* (( *last1 - first1*)-(* last2 - first2 *)) – 1 сравнений для непустых исходных диапазонов.

### <a name="example"></a>Пример

```cpp
// alg_includes.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <functional>      // For greater<int>( )
#include <iostream>

// Return whether modulus of elem1 is less than modulus of elem2
bool mod_lesser (int elem1, int elem2 )
{
   if ( elem1 < 0 )
      elem1 = - elem1;
   if ( elem2 < 0 )
      elem2 = - elem2;
   return elem1 < elem2;
}

int main()
{
   using namespace std;
   vector <int> v1a, v1b;
   vector <int>::iterator Iter1a,  Iter1b;

   // Constructing vectors v1a & v1b with default less-than ordering
   int i;
   for ( i = -2 ; i <= 4 ; i++ )
   {
      v1a.push_back(  i );
   }

   int ii;
   for ( ii =-2 ; ii <= 3 ; ii++ )
   {
      v1b.push_back(  ii  );
   }

   cout << "Original vector v1a with range sorted by the\n "
        << "binary predicate less than is v1a = ( " ;
   for ( Iter1a = v1a.begin( ) ; Iter1a != v1a.end( ) ; Iter1a++ )
      cout << *Iter1a << " ";
   cout << ")." << endl;

   cout << "Original vector v1b with range sorted by the\n "
        <<  "binary predicate less than is v1b = ( " ;
   for ( Iter1b = v1b.begin( ) ; Iter1b != v1b.end( ) ; Iter1b++ )
      cout << *Iter1b << " ";
   cout << ")." << endl;

   // Constructing vectors v2a & v2b with ranges sorted by greater
   vector <int> v2a ( v1a ) , v2b ( v1b );
   vector <int>::iterator Iter2a,  Iter2b;
   sort ( v2a.begin( ), v2a.end( ), greater<int>( ) );
   sort ( v2b.begin( ), v2b.end( ), greater<int>( ) );
   v2a.pop_back( );

   cout << "Original vector v2a with range sorted by the\n "
        <<  "binary predicate greater is v2a = ( " ;
   for ( Iter2a = v2a.begin( ) ; Iter2a != v2a.end( ) ; Iter2a++ )
      cout << *Iter2a << " ";
   cout << ")." << endl;

   cout << "Original vector v2b with range sorted by the\n "
        <<  "binary predicate greater is v2b = ( " ;
   for ( Iter2b = v2b.begin( ) ; Iter2b != v2b.end( ) ; Iter2b++ )
      cout << *Iter2b << " ";
   cout << ")." << endl;

   // Constructing vectors v3a & v3b with ranges sorted by mod_lesser
   vector <int> v3a ( v1a ), v3b ( v1b ) ;
   vector <int>::iterator Iter3a, Iter3b;
   reverse (v3a.begin( ), v3a.end( ) );
   v3a.pop_back( );
   v3a.pop_back( );
   sort ( v3a.begin( ), v3a.end( ), mod_lesser );
   sort ( v3b.begin( ), v3b.end( ), mod_lesser );

   cout << "Original vector v3a with range sorted by the\n "
        <<  "binary predicate mod_lesser is v3a = ( " ;
   for ( Iter3a = v3a.begin( ) ; Iter3a != v3a.end( ) ; Iter3a++ )
      cout << *Iter3a << " ";
   cout << ")." << endl;

   cout << "Original vector v3b with range sorted by the\n "
        <<  "binary predicate mod_lesser is v3b = ( " ;
   for ( Iter3b = v3b.begin( ) ; Iter3b != v3b.end( ) ; Iter3b++ )
      cout << *Iter3b << " ";
   cout << ")." << endl;

   // To test for inclusion under an asscending order
   // with the default binary predicate less <int>( )
   bool Result1;
   Result1 = includes ( v1a.begin( ), v1a.end( ),
      v1b.begin( ), v1b.end( ) );
   if ( Result1 )
      cout << "All the elements in vector v1b are "
           << "contained in vector v1a." << endl;
   else
      cout << "At least one of the elements in vector v1b "
           << "is not contained in vector v1a." << endl;

   // To test for inclusion under descending
   // order specify binary predicate greater<int>( )
   bool Result2;
   Result2 = includes ( v2a.begin( ), v2a.end( ),
      v2b.begin( ), v2b.end( ), greater <int>( ) );
   if ( Result2 )
      cout << "All the elements in vector v2b are "
           << "contained in vector v2a." << endl;
   else
      cout << "At least one of the elements in vector v2b "
           << "is not contained in vector v2a." << endl;

   // To test for inclusion under a user
   // defined binary predicate mod_lesser
   bool Result3;
   Result3 = includes ( v3a.begin( ), v3a.end( ),
      v3b.begin( ), v3b.end( ), mod_lesser );
   if ( Result3 )
      cout << "All the elements in vector v3b are "
           << "contained under mod_lesser in vector v3a."
           << endl;
   else
      cout << "At least one of the elements in vector v3b is "
           << " not contained under mod_lesser in vector v3a."
           << endl;
}
```

```Output
Original vector v1a with range sorted by the
binary predicate less than is v1a = ( -2 -1 0 1 2 3 4 ).
Original vector v1b with range sorted by the
binary predicate less than is v1b = ( -2 -1 0 1 2 3 ).
Original vector v2a with range sorted by the
binary predicate greater is v2a = ( 4 3 2 1 0 -1 ).
Original vector v2b with range sorted by the
binary predicate greater is v2b = ( 3 2 1 0 -1 -2 ).
Original vector v3a with range sorted by the
binary predicate mod_lesser is v3a = ( 0 1 2 3 4 ).
Original vector v3b with range sorted by the
binary predicate mod_lesser is v3b = ( 0 -1 1 -2 2 3 ).
All the elements in vector v1b are contained in vector v1a.
At least one of the elements in vector v2b is not contained in vector v2a.
At least one of the elements in vector v3b is  not contained under mod_lesser in vector v3a.
```

## <a name="inplace_merge"></a>  inplace_merge

Объединяет элементы из двух последовательных упорядоченных диапазонов в один упорядоченный диапазон, где критерий порядка сортировки может быть указан бинарным предикатом.

```cpp
template<class BidirectionalIterator>
void inplace_merge(
    BidirectionalIterator first,
    BidirectionalIterator middle,
    BidirectionalIterator last);

template<class BidirectionalIterator, class Predicate>
void inplace_merge(
    BidirectionalIterator first,
    BidirectionalIterator middle,
    BidirectionalIterator last,
    Predicate comp);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Двунаправленный итератор, указывающий позицию первого элемента в первом из двух последовательных упорядоченных диапазонов, которые следует объединить и упорядочить в один диапазон.

*среднего*<br/>
Двунаправленный итератор, указывающий позицию первого элемента во втором из двух последовательных упорядоченных диапазонов, которые следует объединить и упорядочить в один диапазон.

*последний*<br/>
Двунаправленный итератор, указывающий позицию, следующую за последним элементом во втором из двух последовательных упорядоченных диапазонов, которые следует объединить и упорядочить в один диапазон.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, определяющий условие, когда один элемент больше другого. Бинарный предикат принимает два аргумента и должен возвращать значение **true** , когда первый элемент меньше второго элемента, и значение **false** в противном случае.

### <a name="remarks"></a>Примечания

Упорядоченные последовательные диапазоны, на которые указывают ссылки, должны быть допустимыми. Все указатели должны поддерживать отмену ссылок. В каждой последовательности должна быть возможность достижения последней позиции с первой путем приращения.

Предварительное условие для применения алгоритма `inplace_merge` состоит в том, что каждый упорядоченный последовательный диапазон должен быть упорядочен в соответствии с теми же правилами, которые будут использоваться этим алгоритмом для сортировки объединенных диапазонов. Операция стабильна, так как сохраняется относительный порядок элементов в каждом диапазоне. Если эквивалентные элементы имеются в обоих исходных диапазонах, в объединенном диапазоне элемент из первого диапазона будет предшествовать элементу из второго диапазона.

Сложность зависит от объема доступной памяти, так как алгоритм выделяет память для временного буфера. При наличии достаточного объема памяти лучшим вариантом является Линейный с (* фамилия - имя *) – 1 сравнений; Если нет дополнительная память недоступна, худшим вариантом является *N* журнала *(N)*, где  *N* = (* фамилия - имя*).

### <a name="example"></a>Пример

```cpp
// alg_inplace_merge.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <functional>      //For greater<int>( )
#include <iostream>

// Return whether modulus of elem1 is less than modulus of elem2
bool mod_lesser ( int elem1, int elem2 )
{
   if ( elem1 < 0 )
      elem1 = - elem1;
   if ( elem2 < 0 )
      elem2 = - elem2;
   return elem1 < elem2;
}

int main()
{
   using namespace std;
   vector <int> v1;
   vector <int>::iterator Iter1, Iter2, Iter3;

   // Constructing vector v1 with default less-than ordering
   int i;
   for ( i = 0 ; i <= 5 ; i++ )
   {
      v1.push_back( i );
   }

   int ii;
   for ( ii =-5 ; ii <= 0 ; ii++ )
   {
      v1.push_back(  ii  );
   }

   cout << "Original vector v1 with subranges sorted by the\n "
        <<  "binary predicate less than is  v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;

   // Constructing vector v2 with ranges sorted by greater
   vector <int> v2 ( v1 );
   vector <int>::iterator break2;
   break2 = find ( v2.begin( ), v2.end( ), -5 );
   sort ( v2.begin( ), break2 , greater<int>( ) );
   sort ( break2 , v2.end( ), greater<int>( ) );
   cout << "Original vector v2 with subranges sorted by the\n "
        << "binary predicate greater is v2 = ( " ;
   for ( Iter2 = v2.begin( ) ; Iter2 != v2.end( ) ; Iter2++ )
      cout << *Iter2 << " ";
   cout << ")" << endl;

   // Constructing vector v3 with ranges sorted by mod_lesser
   vector <int> v3 ( v1 );
   vector <int>::iterator break3;
   break3 = find ( v3.begin( ), v3.end( ), -5 );
   sort ( v3.begin( ), break3 , mod_lesser );
   sort ( break3 , v3.end( ), mod_lesser );
   cout << "Original vector v3 with subranges sorted by the\n "
        << "binary predicate mod_lesser is v3 = ( " ;
   for ( Iter3 = v3.begin( ) ; Iter3 != v3.end( ) ; Iter3++ )
      cout << *Iter3 << " ";
   cout << ")" << endl;

   vector <int>::iterator break1;
   break1 = find (v1.begin( ), v1.end( ), -5 );
   inplace_merge ( v1.begin( ), break1, v1.end( ) );
   cout << "Merged inplace with default order,\n vector v1mod = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;

   // To merge inplace in descending order, specify binary
   // predicate greater<int>( )
   inplace_merge ( v2.begin( ), break2 , v2.end( ) , greater<int>( ) );
   cout << "Merged inplace with binary predicate greater specified,\n "
        << "vector v2mod = ( " ;
   for ( Iter2 = v2.begin( ) ; Iter2 != v2.end( ) ; Iter2++ )
      cout << *Iter2 << " ";
   cout << ")" << endl;

   // Applying a user defined (UD) binary predicate mod_lesser
   inplace_merge ( v3.begin( ), break3, v3.end( ), mod_lesser );
   cout << "Merged inplace with binary predicate mod_lesser specified,\n "
        << "vector v3mod = ( " ; ;
   for ( Iter3 = v3.begin( ) ; Iter3 != v3.end( ) ; Iter3++ )
      cout << *Iter3 << " ";
   cout << ")" << endl;
}
```

```Output
Original vector v1 with subranges sorted by the
binary predicate less than is  v1 = ( 0 1 2 3 4 5 -5 -4 -3 -2 -1 0 )
Original vector v2 with subranges sorted by the
binary predicate greater is v2 = ( 5 4 3 2 1 0 0 -1 -2 -3 -4 -5 )
Original vector v3 with subranges sorted by the
binary predicate mod_lesser is v3 = ( 0 1 2 3 4 5 0 -1 -2 -3 -4 -5 )
Merged inplace with default order,
vector v1mod = ( -5 -4 -3 -2 -1 0 0 1 2 3 4 5 )
Merged inplace with binary predicate greater specified,
vector v2mod = ( 5 4 3 2 1 0 0 -1 -2 -3 -4 -5 )
Merged inplace with binary predicate mod_lesser specified,
vector v3mod = ( 0 0 1 -1 2 -2 3 -3 4 -4 5 -5 )
```

## <a name="is_heap"></a>  is_heap

Возвращает **true** Если элементы в указанном диапазоне образуют кучу.

```cpp
template<class RandomAccessIterator>
bool is_heap(
    RandomAccessIterator first,
    RandomAccessIterator last);

template<class RandomAccessIterator, class BinaryPredicate>
bool is_heap(
    RandomAccessIterator first,
    RandomAccessIterator last,
    BinaryPredicate comp);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Итератор произвольного доступа, указывающий начало диапазона для проверки кучи.

*последний*<br/>
Итератор произвольного доступа, указывающий конец диапазона.

*Зап.*<br/>
Условие для проверки порядка элементов. Двоичный предикат принимает один аргумент и возвращает **true** или **false**.

### <a name="return-value"></a>Возвращаемое значение

Возвращает **true** Если элементы в указанном диапазоне образуют кучу, **false** при их отсутствии.

### <a name="remarks"></a>Примечания

Первая функция-шаблон возвращает [is_heap_until](../standard-library/algorithm-functions.md#is_heap_until)`(first , last) == last`.

Вторая функция шаблона возвращает

`is_heap_until(first, last, comp) == last`.

## <a name="is_heap_until"></a>  is_heap_until

Возвращает итератор, расположенный на первый элемент в диапазоне [ `begin`, `end`), не удовлетворяет условию упорядочения кучи, или *окончания* Если диапазон образует кучу.

```cpp
template<class RandomAccessIterator>
RandomAccessIterator is_heap_until(
    RandomAccessIterator begin,
    RandomAccessIterator end);

template<class RandomAccessIterator, class BinaryPredicate>
RandomAccessIterator is_heap_until(
    RandomAccessIterator begin,
    RandomAccessIterator end,
    BinaryPredicate compare);
```

### <a name="parameters"></a>Параметры

*begin*<br/>
Итератор произвольного доступа, который задает первый элемент диапазона для проверки кучи.

*end*<br/>
Итератор произвольного доступа, который задает конец диапазона для проверки кучи.

*compare*<br/>
Двухместный предикат, который задает условие строгого слабого упорядочения, определяющее кучу. Предикат по умолчанию, когда *сравнения* не указан — `std::less<>`.

### <a name="return-value"></a>Возвращаемое значение

Возвращает *окончания* Если указанный диапазон образует кучу или содержит один элемент либо менее. В противном случае возвращает итератор для первого найденного элемента, который не удовлетворяет условию кучи.

### <a name="remarks"></a>Примечания

Первая функция-шаблон возвращает последний итератор `next` в `[ begin , end ]` где `[ begin , next)` — это куча, упорядоченная по объекту функции `std::less<>`. Если расстояние `end - begin < 2`, функция возвращает *окончания*.

Вторая функция-шаблон работает так же, как первая, но использует в качестве условия упорядочения кучи предикат `compare` вместо `std::less<>`.

## <a name="is_partitioned"></a>  is_partitioned

Возвращает **true** Если все элементы в заданном диапазоне, возвращающие **true** для условие располагаются перед всеми элементами, возвращающими **false**.

```cpp
template<class InputIterator, class BinaryPredicate>
bool is_partitioned(
    InputIterator first,
    InputIterator last,
    BinaryPredicate comp);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Входной итератор, указывающий, где начинается диапазон для проверки условия.

*последний*<br/>
Входной итератор, указывающий конец диапазона.

*Зап.*<br/>
Условие для проверки. Оно предоставляется определенным пользователем объектом функции, задающим условие, которому должен соответствовать искомый элемент. Предикат принимает один аргумент и возвращает значение **true** или **false**.

### <a name="return-value"></a>Возвращаемое значение

Возвращает значение true, если все элементы в заданном диапазоне, которые проверяют **true** для условие располагаются перед всеми элементами, возвращающими **false**и в противном случае возвращает **false**.

### <a name="remarks"></a>Примечания

Функция шаблона возвращает **true** только если все элементы в `[` `first ,` `last )` разделяются по *comp*; то есть все элементы `X` в `[` `first ,` `last )` для которого `comp (X)` имеет значение true, находятся перед всеми элементами `Y` для которого `comp (Y)` — **false**.

## <a name="is_permutation"></a>  is_permutation

Возвращает значение true, если оба диапазона содержат одинаковые элементы и не важно, располагаются ли элементы в одном и том же порядке. Используйте двух-диапазонные перегрузки в коде C++ 14. Перегрузки, использующие только один итератор для второго диапазона, не обнаруживают различия в тех случаях, когда второй диапазон длиннее, чем первый, и их поведение может быть непредсказуемо, если второй диапазон короче, чем первый.

```cpp
template<class ForwardIterator1, class ForwardIterator2>
bool is_permutation(
    ForwardIterator1 First1,
    ForwardIterator1 Last1,
    ForwardIterator2 First2);

template<class ForwardIterator1, class ForwardIterator2, class Predicate>
bool is_permutation(
    ForwardIterator1 First1,
    ForwardIterator1 Last1,
    ForwardIterator2 First2,
    Predicate Pred);

// C++14
template<class ForwardIterator1, class ForwardIterator2>
bool is_permutation(
    ForwardIterator1 First1,
    ForwardIterator1 Last1,
    ForwardIterator2 First2,
    ForwardIterator2 Last2);

template<class ForwardIterator1, class ForwardIterator2, class Predicate>
bool is_permutation(
    ForwardIterator1 First1,
    ForwardIterator1 Last1,
    ForwardIterator2 First2,
    ForwardIterator2 Last2,
    Predicate Pred);
```

### <a name="parameters"></a>Параметры

*first1*<br/>
Прямой итератор, указывающий на первый элемент диапазона.

*last1*<br/>
Прямой итератор, указывающий на место, следующее за последним элементом диапазона.

*first2*<br/>
Прямой итератор, указывающий на первый элемент второго диапазона, используемый для сравнения.

*last2*<br/>
Прямой итератор, указывающий на место, следующее за последним элементом второго диапазона, используемым для сравнения.

*Пред*<br/>
Предикат, который проверяет равенство и возвращает **bool**.

### <a name="return-value"></a>Возвращаемое значение

**значение true,** при диапазоны, которые можно переупорядочить таким образом, чтобы быть идентичны в соответствии с предикатом сравнения; в противном случае — значение **false**.

### <a name="remarks"></a>Примечания

`is_permutation` в худшем случае имеет квадратичную сложность.

Первая функция-шаблон предполагает, что существуют столько же элементов в диапазоне, начинающемся *First2* в диапазоне, указанном аргументами [ `First1`, `Last1`). Если во втором диапазоне элементов больше, они игнорируются. Если элементов меньше — результат будет непредсказуемым. Третья функция шаблона (C++ 14 и более поздние версии) не использует это допущение.  Обе функции возвращают **true** только если для каждого элемента X в диапазоне, указанном аргументами [ `First1`, `Last1`) существует столько же элементов Y в тот же диапазон, для которых X == Y, сколько в диапазоне, начинающемся *First2* или [ `First2, Last2).` здесь `operator==` должен выполнять парные сравнения между операндами.

Вторая и четвертая функции шаблона действуют одинаково, за исключением того, что они заменяют `operator==(X, Y)` на `Pred(X, Y)`. Чтобы действия были правильными, предикат должен быть симметричным, рефлексивным и транзитивным.

### <a name="example"></a>Пример

В следующем примере показано использование `is_permutation`.

```cpp
#include <vector>
#include <iostream>
#include <algorithm>
#include <string>

using namespace std;

int main()
{
    vector<int> vec_1{ 2, 3, 0, 1, 4, 5 };
    vector<int> vec_2{ 5, 4, 0, 3, 1, 2 };

    vector<int> vec_3{ 4, 9, 13, 3, 6, 5 };
    vector<int> vec_4{ 7, 4, 11, 9, 2, 1 };

    cout << "(1) Compare using built-in == operator: ";
    cout << boolalpha << is_permutation(vec_1.begin(), vec_1.end(),
        vec_2.begin(), vec_2.end()) << endl; // true

    cout << "(2) Compare after modifying vec_2: ";
    vec_2[0] = 6;
    cout << is_permutation(vec_1.begin(), vec_1.end(),
        vec_2.begin(), vec_2.end()) << endl; // false

    // Define equivalence as "both are odd or both are even"
    cout << "(3) vec_3 is a permutation of vec_4: ";
    cout << is_permutation(vec_3.begin(), vec_3.end(),
        vec_4.begin(), vec_4.end(),
        [](int lhs, int rhs) { return lhs % 2 == rhs % 2; }) << endl; // true

    // Initialize a vector using the 's' string literal to specify a std::string
    vector<string> animals_1{ "dog"s, "cat"s, "bird"s, "monkey"s };
    vector<string> animals_2{ "donkey"s, "bird"s, "meerkat"s, "cat"s };

    // Define equivalence as "first letters are equal":
    bool is_perm = is_permutation(animals_1.begin(), animals_1.end(), animals_2.begin(), animals_2.end(),
        [](const string& lhs, const string& rhs)
    {
        return lhs[0] == rhs[0]; //std::string guaranteed to have at least a null terminator
    });

    cout << "animals_2 is a permutation of animals_1: " << is_perm << endl; // true

    cout << "Press a letter" << endl;
    char c;
    cin >> c;

    return 0;
}

```

## <a name="is_sorted"></a>  is_sorted

Возвращает **true** Если элементы в указанном диапазоне расположены в порядке сортировки.

```cpp
template<class ForwardIterator>
bool is_sorted(
    ForwardIterator first,
    ForwardIterator last);

template<class ForwardIterator, class BinaryPredicate>
bool is_sorted(
    ForwardIterator first,
    ForwardIterator last,
    BinaryPredicate comp);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Прямой итератор, указывающий, где начинается диапазон для проверки.

*последний*<br/>
Прямой итератор, указывающий конец диапазона.

*Зап.*<br/>
Условие теста для определения порядка между двумя элементами. Предикат принимает один аргумент и возвращает значение **true** или **false**. Он выполняет ту же задачу, что и `operator<`.

### <a name="remarks"></a>Примечания

Первая функция-шаблон возвращает [is_sorted_until](#is_sorted_until)`( first, last ) == last`. `operator<` Функция выполняет сравнение порядка.

Вторая функция-шаблон возвращает `is_sorted_until( first, last , comp ) == last`. *Comp* функции предиката выполняет сравнение порядка.

## <a name="is_sorted_until"></a>  is_sorted_until

Возвращает `ForwardIterator`, установленный в последний элемент в порядке сортировки из указанного диапазона.

Вторая версия позволяет предоставить `BinaryPredicate` функция, возвращающая **true** при два конкретных элемента расположены в отсортированном порядке и **false** в противном случае.

```cpp
template<class ForwardIterator>
ForwardIterator is_sorted_until(
    ForwardIterator first,
    ForwardIterator last);
template<class ForwardIterator, class BinaryPredicate>
ForwardIterator is_sorted_until(
    ForwardIterator first,
    ForwardIterator last,
    BinaryPredicate comp);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Прямой итератор, указывающий, где начинается диапазон для проверки.

*последний*<br/>
Прямой итератор, указывающий конец диапазона.

*Зап.*<br/>
Условие теста для определения порядка между двумя элементами. Предикат принимает один аргумент и возвращает значение **true** или **false**.

### <a name="return-value"></a>Возвращаемое значение

Возвращает `ForwardIterator`, установленный в последний элемент в порядке сортировки. Отсортированная последовательность начинается с *первый*.

### <a name="remarks"></a>Примечания

Первая функция-шаблон возвращает последний итератор `next` в `[` `first ,` `last ]`, так что `[` `first , next)` — это последовательность, упорядоченная по `operator<`. Если `distance()` `< 2` функция возвращает *последнего*.

Вторая функция шаблона работает так же, за исключением того, что она заменяет `operator<(X, Y)` на `comp (X, Y)`.

## <a name="iter_swap"></a>  iter_swap

Меняет местами два значения, указанные парой определенных итераторов.

```cpp
template<class ForwardIterator1, class ForwardIterator2>
void iter_swap( ForwardIterator1 left, ForwardIterator2 right );

```

### <a name="parameters"></a>Параметры

*left*<br/>
Один из прямых итераторов, значение которого должно быть изменено.

*right*<br/>
Второй из прямых итераторов, значение которого должно быть изменено.

### <a name="remarks"></a>Примечания

Рекомендуется использовать функцию `swap` вместо i **ter_swap**, которая включена в стандарт C++ для обеспечения обратной совместимости. Если `Fit1` и `Fit2` являются прямыми итераторами, затем `iter_swap` ( `Fit1`, `Fit2` ), эквивалентно `swap` ( \* `Fit1`, \* `Fit2` ).

Типы значений входных прямых итераторов должны иметь одно и то же значение.

### <a name="example"></a>Пример

```cpp
// alg_iter_swap.cpp
// compile with: /EHsc
#include <vector>
#include <deque>
#include <algorithm>
#include <iostream>
#include <ostream>

using namespace std;
class CInt;
ostream& operator<<( ostream& osIn, const CInt& rhs );

class CInt
{
public:
   CInt( int n = 0 ) : m_nVal( n ){}
   CInt( const CInt& rhs ) : m_nVal( rhs.m_nVal ){}
   CInt&   operator=( const CInt& rhs ) { m_nVal =
   rhs.m_nVal; return *this; }
   bool operator<( const CInt& rhs ) const
      { return ( m_nVal < rhs.m_nVal );}
   friend ostream& operator<<( ostream& osIn, const CInt& rhs );

private:
   int m_nVal;
};

inline ostream& operator<<( ostream& osIn, const CInt& rhs )
{
   osIn << "CInt(" << rhs.m_nVal << ")";
   return osIn;
}

// Return whether modulus of elem1 is less than modulus of elem2
bool mod_lesser ( int elem1, int elem2 )
{
   if ( elem1 < 0 )
      elem1 = - elem1;
   if ( elem2 < 0 )
      elem2 = - elem2;
   return elem1 < elem2;
};

int main()
{
   CInt c1 = 5, c2 = 1, c3 = 10;
   deque<CInt> deq1;
   deque<CInt>::iterator d1_Iter;

   deq1.push_back ( c1 );
   deq1.push_back ( c2 );
   deq1.push_back ( c3 );

   cout << "The original deque of CInts is deq1 = (";
   for ( d1_Iter = deq1.begin( ); d1_Iter != --deq1.end( ); d1_Iter++ )
      cout << " " << *d1_Iter << ",";
   d1_Iter = --deq1.end( );
   cout << " " << *d1_Iter << " )." << endl;

   // Exchanging first and last elements with iter_swap
   iter_swap ( deq1.begin( ), --deq1.end( ) );

   cout << "The deque of CInts with first & last elements swapped is:\n deq1 = (";
   for ( d1_Iter = deq1.begin( ); d1_Iter != --deq1.end( ); d1_Iter++ )
      cout << " " << *d1_Iter << ",";
   d1_Iter = --deq1.end( );
   cout << " " << *d1_Iter << " )." << endl;

   // Swapping back first and last elements with swap
   swap ( *deq1.begin( ), *(deq1.end( ) -1 ) );

   cout << "The deque of CInts with first & last elements swapped back is:\n deq1 = (";
   for ( d1_Iter = deq1.begin( ); d1_Iter != --deq1.end( ); d1_Iter++ )
      cout << " " << *d1_Iter << ",";
   d1_Iter = --deq1.end( );
   cout << " " << *d1_Iter << " )." << endl;

   // Swapping a vector element with a deque element
   vector <int> v1;
   vector <int>::iterator Iter1;
   deque <int> deq2;
   deque <int>::iterator d2_Iter;

   int i;
   for ( i = 0 ; i <= 3 ; i++ )
   {
      v1.push_back( i );
   }

   int ii;
   for ( ii = 4 ; ii <= 5 ; ii++ )
   {
      deq2.push_back( ii );
   }

   cout << "Vector v1 is ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   cout << "Deque deq2 is ( " ;
   for ( d2_Iter = deq2.begin( ) ; d2_Iter != deq2.end( ) ; d2_Iter++ )
      cout << *d2_Iter << " ";
   cout << ")." << endl;

   iter_swap ( v1.begin( ), deq2.begin( ) );

   cout << "After exchanging first elements,\n vector v1 is: v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl << " & deque deq2 is: deq2 = ( ";
   for ( d2_Iter = deq2.begin( ) ; d2_Iter != deq2.end( ) ; d2_Iter++ )
      cout << *d2_Iter << " ";
   cout << ")." << endl;
}
```

```Output
The original deque of CInts is deq1 = ( CInt(5), CInt(1), CInt(10) ).
The deque of CInts with first & last elements swapped is:
deq1 = ( CInt(10), CInt(1), CInt(5) ).
The deque of CInts with first & last elements swapped back is:
deq1 = ( CInt(5), CInt(1), CInt(10) ).
Vector v1 is ( 0 1 2 3 ).
Deque deq2 is ( 4 5 ).
After exchanging first elements,
vector v1 is: v1 = ( 4 1 2 3 ).
& deque deq2 is: deq2 = ( 0 5 ).
```

## <a name="lexicographical_compare"></a>  lexicographical_compare

Сравнивает две последовательности поэлементно для определения того, какой элемент из двух меньше.

```cpp
template<class InputIterator1, class InputIterator2>
bool lexicographical_compare(
    InputIterator1  first1,
    InputIterator1 Last1,
    InputIterator2  first2,
    InputIterator2 Last2  );

template<class InputIterator1, class InputIterator2, class BinaryPredicate>
bool lexicographical_compare(
    InputIterator1  first1,
    InputIterator1 Last1,
    InputIterator2  first2,
    InputIterator2 Last2,
    BinaryPredicate  comp  );

```

### <a name="parameters"></a>Параметры

*first1*<br/>
Входной итератор, указывающий на положение первого элемента в первом диапазоне для сравнения.

*last1*<br/>
Входной итератор, указывающий на положение, следующее за последним элементом в первом диапазоне для сравнения.

*first2*<br/>
Входной итератор, указывающий на положение первого элемента во втором диапазоне для сравнения.

*last2*<br/>
Входной итератор, указывающий на положение, следующее за последним элементом во втором диапазоне для сравнения.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, задающий условие, когда один элемент меньше другого. Двоичный предикат принимает два аргумента и возвращает **true** , если условие удовлетворено, или **false** , если условие не удовлетворено.

### <a name="return-value"></a>Возвращаемое значение

Значение **true**, если первый диапазон лексикографически меньше второго диапазона; в противном случае — значение **false**.

### <a name="remarks"></a>Примечания

При лексикографическом сравнении двух последовательностей они сравниваются поэлементно до тех пор, пока не произойдет следующее.

- Находит 2 неравных соответствующих элемента и результат их сравнения считается результатом сравнения между двумя последовательностями.

- Неравенства не найдены, но одна последовательность имеет больше элементов, чем другая, и более короткая последовательность считается меньше, чем более длинная последовательность.

- Неравенства не найдены и последовательности имеют одинаковое количество элементов, поэтому последовательности равны и результат сравнения ложен.

### <a name="example"></a>Пример

```cpp
// alg_lex_comp.cpp
// compile with: /EHsc
#include <vector>
#include <list>
#include <algorithm>
#include <iostream>

// Return whether second element is twice the first
bool twice ( int elem1, int elem2 )
{
   return 2 * elem1 < elem2;
}

int main()
{
   using namespace std;
   vector <int> v1, v2;
   list <int> L1;
   vector <int>::iterator Iter1, Iter2;
   list <int>::iterator L1_Iter, L1_inIter;

   int i;
   for ( i = 0 ; i <= 5 ; i++ )
   {
      v1.push_back( 5 * i );
   }
   int ii;
   for ( ii = 0 ; ii <= 6 ; ii++ )
   {
      L1.push_back( 5 * ii );
   }

   int iii;
   for ( iii = 0 ; iii <= 5 ; iii++ )
   {
      v2.push_back( 10 * iii );
   }

   cout << "Vector v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;

   cout << "List L1 = ( " ;
   for ( L1_Iter = L1.begin( ) ; L1_Iter!= L1.end( ) ; L1_Iter++ )
      cout << *L1_Iter << " ";
   cout << ")" << endl;

   cout << "Vector v2 = ( " ;
   for ( Iter2 = v2.begin( ) ; Iter2 != v2.end( ) ; Iter2++ )
      cout << *Iter2 << " ";
      cout << ")" << endl;

   // Self lexicographical_comparison of v1 under identity
   bool result1;
   result1 = lexicographical_compare (v1.begin( ), v1.end( ),
                  v1.begin( ), v1.end( ) );
   if ( result1 )
      cout << "Vector v1 is lexicographically_less than v1." << endl;
   else
      cout << "Vector v1 is not lexicographically_less than v1." << endl;

   // lexicographical_comparison of v1 and L2 under identity
   bool result2;
   result2 = lexicographical_compare (v1.begin( ), v1.end( ),
                  L1.begin( ), L1.end( ) );
   if ( result2 )
      cout << "Vector v1 is lexicographically_less than L1." << endl;
   else
      cout << "Vector v1 is lexicographically_less than L1." << endl;

   bool result3;
   result3 = lexicographical_compare (v1.begin( ), v1.end( ),
                  v2.begin( ), v2.end( ), twice );
   if ( result3 )
      cout << "Vector v1 is lexicographically_less than v2 "
           << "under twice." << endl;
   else
      cout << "Vector v1 is not lexicographically_less than v2 "
           << "under twice." << endl;
}
```

```Output
Vector v1 = ( 0 5 10 15 20 25 )
List L1 = ( 0 5 10 15 20 25 30 )
Vector v2 = ( 0 10 20 30 40 50 )
Vector v1 is not lexicographically_less than v1.
Vector v1 is lexicographically_less than L1.
Vector v1 is not lexicographically_less than v2 under twice.
```

## <a name="lower_bound"></a>  lower_bound

Находит позицию первого элемента в упорядоченном диапазоне, значение которого больше или равно указанному значению, где критерий упорядочивания может быть задан бинарным предикатом.

```cpp
template<class ForwardIterator, class Type>
ForwardIterator lower_bound(
    ForwardIterator first,
    ForwardIterator last,
    const Type& value );

template<class ForwardIterator, class Type, class BinaryPredicate>
ForwardIterator lower_bound(
    ForwardIterator first,
    ForwardIterator last,
    const Type& value,
    BinaryPredicate comp );

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Прямой итератор, адресующий положение первого элемента в диапазоне для поиска.

*последний*<br/>
Прямой итератор, адресующий положение на единицу после последнего элемента в диапазоне для поиска.

*значение*<br/>
Значение, чья первая позиция или возможная первая позиция ищется в упорядоченном диапазоне.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, задающий условие, когда один элемент меньше другого. Двоичный предикат принимает два аргумента и возвращает **true** , если условие удовлетворено, или **false** , если условие не удовлетворено.

### <a name="return-value"></a>Возвращаемое значение

Однонаправленный итератор в позиции первого элемента в упорядоченном диапазоне, который имеет значение большее или эквивалентное указанному значению, где эквивалентность задана двоичным предикатом.

### <a name="remarks"></a>Примечания

Упорядоченный исходный диапазон, на который указывает ссылка, должен быть допустим. Все итераторы должны поддерживать отмену ссылок. В последовательности должна быть возможность достижения последней позиции с первой путем приращения.

Предварительным условием для использования `lower_bound` является упорядоченный диапазон, порядок в котором тот же, что и заданный двоичным предикатом.

Диапазон не изменяется алгоритмом `lower_bound`.

В целях упорядочения типы значений прямых итераторов должны подлежать сравнению "меньше чем", чтобы при наличии двух элементов можно было определить, что они равны (т. е. ни один не меньше другого) или что один меньше другого. Это приводит к упорядочению неравнозначных элементов.

Сложность алгоритма является логарифмической для итераторов произвольного доступа и линейной в противном случае с числом шагов, пропорциональным значению (`last - first`).

### <a name="example"></a>Пример

```cpp
// alg_lower_bound.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <functional>      // greater<int>( )
#include <iostream>

// Return whether modulus of elem1 is less than modulus of elem2
bool mod_lesser( int elem1, int elem2 )
{
    if ( elem1 < 0 )
        elem1 = - elem1;
    if ( elem2 < 0 )
        elem2 = - elem2;
    return elem1 < elem2;
}

int main()
{
    using namespace std;

    vector<int> v1;
    // Constructing vector v1 with default less-than ordering
    for ( auto i = -1 ; i <= 4 ; ++i )
    {
        v1.push_back(  i );
    }

    for ( auto ii =-3 ; ii <= 0 ; ++ii )
    {
        v1.push_back(  ii  );
    }

    cout << "Starting vector v1 = ( " ;
    for (const auto &Iter : v1)
        cout << Iter << " ";
    cout << ")." << endl;

    sort(v1.begin(), v1.end());
    cout << "Original vector v1 with range sorted by the\n "
        << "binary predicate less than is v1 = ( " ;
    for (const auto &Iter : v1)
        cout << Iter << " ";
    cout << ")." << endl;

    // Constructing vector v2 with range sorted by greater
    vector<int> v2(v1);

    sort(v2.begin(), v2.end(), greater<int>());

    cout << "Original vector v2 with range sorted by the\n "
        << "binary predicate greater is v2 = ( " ;
    for (const auto &Iter : v2)
        cout << Iter << " ";
    cout << ")." << endl;

    // Constructing vectors v3 with range sorted by mod_lesser
    vector<int> v3(v1);
    sort(v3.begin(), v3.end(), mod_lesser);

    cout << "Original vector v3 with range sorted by the\n "
        <<  "binary predicate mod_lesser is v3 = ( " ;
    for (const auto &Iter : v3)
        cout << Iter << " ";
    cout << ")." << endl;

    // Demonstrate lower_bound

    vector<int>::iterator Result;

    // lower_bound of 3 in v1 with default binary predicate less<int>()
    Result = lower_bound(v1.begin(), v1.end(), 3);
    cout << "The lower_bound in v1 for the element with a value of 3 is: "
        << *Result << "." << endl;

    // lower_bound of 3 in v2 with the binary predicate greater<int>( )
    Result = lower_bound(v2.begin(), v2.end(), 3, greater<int>());
    cout << "The lower_bound in v2 for the element with a value of 3 is: "
        << *Result << "." << endl;

    // lower_bound of 3 in v3 with the binary predicate  mod_lesser
    Result = lower_bound(v3.begin(), v3.end(), 3,  mod_lesser);
    cout << "The lower_bound in v3 for the element with a value of 3 is: "
        << *Result << "." << endl;
}

```

## <a name="make_heap"></a>  make_heap

Преобразует элементы из указанного диапазона в кучу, в которой первый элемент является наибольшим и для которой критерий сортировки может быть определен бинарным предикатом.

```cpp
template<class RandomAccessIterator>
void make_heap(
    RandomAccessIterator first,
    RandomAccessIterator last );

template<class RandomAccessIterator, class BinaryPredicate>
void make_heap(
    RandomAccessIterator first,
    RandomAccessIterator last,
    BinaryPredicate comp );

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Итератор произвольного доступа, обращающийся к позиции первого элемента в диапазоне, подлежащем преобразованию в кучу.

*последний*<br/>
Итератор произвольного доступа, обращающийся к позиции, следующей за последним элементом в диапазоне, подлежащем преобразованию в кучу.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, задающий условие, когда один элемент меньше другого. Двоичный предикат принимает два аргумента и возвращает **true** , если условие удовлетворено, или **false** , если условие не удовлетворено.

### <a name="remarks"></a>Примечания

Кучи имеют два следующих свойства.

- Первый элемент — всегда наибольший.

- Элементы могут добавляться и удаляться в логарифмическое время.

Кучи — идеальный способ реализации очередей с приоритетами, и они используются в [классе priority_queue](../standard-library/priority-queue-class.md) адаптеров контейнеров библиотеки стандартных программ C++.

Отношение сложности линейное; требуется 3 \* (* фамилия - имя *) сравнений.

### <a name="example"></a>Пример

```cpp
// alg_make_heap.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <functional>
#include <iostream>

int main() {
   using namespace std;
   vector <int> v1, v2;
   vector <int>::iterator Iter1, Iter2;

   int i;
   for ( i = 0 ; i <= 9 ; i++ )
      v1.push_back( i );

   random_shuffle( v1.begin( ), v1.end( ) );

   cout << "Vector v1 is ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Make v1 a heap with default less than ordering
   make_heap ( v1.begin( ), v1.end( ) );
   cout << "The heaped version of vector v1 is ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Make v1 a heap with greater than ordering
   make_heap ( v1.begin( ), v1.end( ), greater<int>( ) );
   cout << "The greater-than heaped version of v1 is ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;
}
```

## <a name="max"></a>  max

Сравнивает два объекта и возвращает больший из них, где критерий упорядочивания может быть указан бинарным предикатом.

```cpp
template<class Type>
constexpr Type& max(
    const Type& left,
    const Type& right);
template<class Type, class Pr>
constexpr Type& max(
    const Type& left,
    const Type& right,
    BinaryPredicate comp);
template<class Type>
constexpr Type& max (
    initializer_list<Type> );
template<class Type, class Pr>
constexpr Type& max(
    initializer_list<Type> ,
    BinaryPredicate comp);
```

### <a name="parameters"></a>Параметры

*left*<br/>
Первый из сравниваемых объектов.

*right*<br/>
Второй из сравниваемых объектов.

*Зап.*<br/>
Двоичный предикат, используемый для сравнения двух объектов.

*_IList*<br/>
Список initializer с объектами, которые необходимо сравнить.

### <a name="return-value"></a>Возвращаемое значение

Больший из двух объектов, если ни один из них не больше — в этом случае возвращается первый из двух объектов. В случае с initializer_list возвращается самый большой из объектов в списке.

### <a name="remarks"></a>Примечания

При использовании алгоритма `max` очень редко объекты передаются как параметры. Большинство алгоритмов библиотеки стандартных программ C++ работают в диапазоне элементов, позиция которых задается итераторами, передаваемыми в качестве параметров. Если требуется функция, которая работает в диапазоне элементов, рекомендуется использовать [max_element](../standard-library/algorithm-functions.md#max_element). Visual Studio 2017 позволяет **constexpr** на перегрузки, принимающие объект initializer_list.

### <a name="example"></a>Пример

```cpp
// alg_max.cpp
// compile with: /EHsc
#include <vector>
#include <set>
#include <algorithm>
#include <iostream>
#include <ostream>

using namespace std;
class CInt;
ostream& operator<<( ostream& osIn, const CInt& rhs );

class CInt
{
public:
   CInt( int n = 0 ) : m_nVal( n ){}
   CInt( const CInt& rhs ) : m_nVal( rhs.m_nVal ){}
   CInt&   operator=( const CInt& rhs ) {m_nVal =
   rhs.m_nVal; return *this;}
   bool operator<( const CInt& rhs ) const
      {return ( m_nVal < rhs.m_nVal );}
   friend ostream& operator<<( ostream& osIn, const CInt& rhs );

private:
   int m_nVal;
};

inline ostream& operator<<( ostream& osIn, const CInt& rhs )
{
   osIn << "CInt( " << rhs.m_nVal << " )";
   return osIn;
}

// Return whether absolute value of elem1 is greater than
// absolute value of elem2
bool abs_greater ( int elem1, int elem2 )
{
   if ( elem1 < 0 )
      elem1 = -elem1;
   if ( elem2 < 0 )
      elem2 = -elem2;
   return elem1 < elem2;
};

int main()
{
   int a = 6, b = -7;
   // Return the integer with the larger absolute value
   const int& result1 = max(a, b, abs_greater);
   // Return the larger integer
   const int& result2 = max(a, b);

   cout << "Using integers 6 and -7..." << endl;
   cout << "The integer with the greater absolute value is: "
        << result1 << "." << endl;
   cout << "The integer with the greater value is: "
        << result2 << "." << endl;
   cout << endl;

// Comparing the members of an initializer_list
const int& result3 = max({ a, b });
const int& result4 = max({ a, b }, abs_greater);

cout << "Comparing the members of an initializer_list..." << endl;
cout << "The member with the greater value is: " << result3 << endl;
cout << "The integer with the greater absolute value is: " << result4 << endl;

   // Comparing set containers with elements of type CInt
   // using the max algorithm
   CInt c1 = 1, c2 = 2, c3 = 3;
   set<CInt> s1, s2, s3;
   set<CInt>::iterator s1_Iter, s2_Iter, s3_Iter;

   s1.insert ( c1 );
   s1.insert ( c2 );
   s2.insert ( c2 );
   s2.insert ( c3 );

   cout << "s1 = (";
   for ( s1_Iter = s1.begin( ); s1_Iter != --s1.end( ); s1_Iter++ )
      cout << " " << *s1_Iter << ",";
   s1_Iter = --s1.end( );
   cout << " " << *s1_Iter << " )." << endl;

   cout << "s2 = (";
   for ( s2_Iter = s2.begin( ); s2_Iter != --s2.end( ); s2_Iter++ )
      cout << " " << *s2_Iter << ",";
   s2_Iter = --s2.end( );
   cout << " " << *s2_Iter << " )." << endl;

   s3 = max ( s1, s2 );
   cout << "s3 = max ( s1, s2 ) = (";
   for ( s3_Iter = s3.begin( ); s3_Iter != --s3.end( ); s3_Iter++ )
      cout << " " << *s3_Iter << ",";
   s3_Iter = --s3.end( );
   cout << " " << *s3_Iter << " )." << endl << endl;

   // Comparing vectors with integer elements using the max algorithm
   vector <int> v1, v2, v3, v4, v5;
   vector <int>::iterator Iter1, Iter2, Iter3, Iter4, Iter5;

   int i;
   for ( i = 0 ; i <= 2 ; i++ )
   {
      v1.push_back( i );
   }

   int ii;
   for ( ii = 0 ; ii <= 2 ; ii++ )
   {
      v2.push_back( ii );
   }

   int iii;
   for ( iii = 0 ; iii <= 2 ; iii++ )
   {
      v3.push_back( 2 * iii );
   }

   cout << "Vector v1 is ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   cout << "Vector v2 is ( " ;
   for ( Iter2 = v2.begin( ) ; Iter2 != v2.end( ) ; Iter2++ )
      cout << *Iter2 << " ";
   cout << ")." << endl;

   cout << "Vector v3 is ( " ;
   for ( Iter3 = v3.begin( ) ; Iter3 != v3.end( ) ; Iter3++ )
      cout << *Iter3 << " ";
   cout << ")." << endl;

   v4 = max ( v1, v2 );
   v5 = max ( v1, v3 );

   cout << "Vector v4 = max (v1,v2) is ( " ;
   for ( Iter4 = v4.begin( ) ; Iter4 != v4.end( ) ; Iter4++ )
      cout << *Iter4 << " ";
   cout << ")." << endl;

   cout << "Vector v5 = max (v1,v3) is ( " ;
   for ( Iter5 = v5.begin( ) ; Iter5 != v5.end( ) ; Iter5++ )
      cout << *Iter5 << " ";
   cout << ")." << endl;
}
```

```Output
Using integers 6 and -7...
The integer with the greater absolute value is: -7
The integer with the greater value is: 6.
Comparing the members of an initializer_list...The member with the greater value is: 6The integer wiht the greater absolute value is: -7
s1 = ( CInt( 1 ), CInt( 2 ) ).
s2 = ( CInt( 2 ), CInt( 3 ) ).
s3 = max ( s1, s2 ) = ( CInt( 2 ), CInt( 3 ) ).

Vector v1 is ( 0 1 2 ).
Vector v2 is ( 0 1 2 ).
Vector v3 is ( 0 2 4 ).
Vector v4 = max (v1,v2) is ( 0 1 2 ).
Vector v5 = max (v1,v3) is ( 0 2 4 ).
```

## <a name="max_element"></a>  max_element

Находит первое вхождение наибольшего элемента в указанном диапазоне, где критерий упорядочивания может быть указан бинарным предикатом.

```cpp
template<class ForwardIterator>
constexpr ForwardIterator max_element(ForwardIterator first, ForwardIterator last );

template<class ForwardIterator, class BinaryPredicate>
constexpr ForwardIterator max_element(ForwardIterator first, ForwardIterator last, BinaryPredicate comp );

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Прямой итератор, указывающий положение первого элемента в диапазоне для поиска наибольшего элемента.

*последний*<br/>
Прямой итератор, указывающий положение, следующее за последним элементом в диапазоне для поиска наибольшего элемента.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, определяющий условие, когда один элемент больше другого. Бинарный предикат принимает два аргумента и должен возвращать значение **true** , когда первый элемент меньше второго элемента, и значение **false** в противном случае.

### <a name="return-value"></a>Возвращаемое значение

Прямой итератор, указывающий положение первого вхождения наибольшего элемента в диапазоне для поиска.

### <a name="remarks"></a>Примечания

Диапазоны, на которые указывают ссылки, должны быть допустимыми; все указатели должны поддерживать сброс ссылок; в каждой последовательности должна быть возможность достижения последнего положения с первого путем приращения.

Отношение сложности линейное: (`last` - `first`) – 1 сравнений для непустого диапазона требуется.

### <a name="example"></a>Пример

```cpp
// alg_max_element.cpp
// compile with: /EHsc
#include <vector>
#include <set>
#include <algorithm>
#include <iostream>
#include <ostream>

using namespace std;
class CInt;
ostream& operator<<( ostream& osIn, const CInt& rhs );

class CInt
{
public:
   CInt( int n = 0 ) : m_nVal( n ){}
   CInt( const CInt& rhs ) : m_nVal( rhs.m_nVal ){}
   CInt& operator=( const CInt& rhs ) {m_nVal =
   rhs.m_nVal; return *this;}
   bool operator<( const CInt& rhs ) const
      {return ( m_nVal < rhs.m_nVal );}
   friend ostream& operator<<( ostream& osIn, const CInt& rhs );

private:
   int m_nVal;
};

inline ostream& operator<<(ostream& osIn, const CInt& rhs)
{
   osIn << "CInt( " << rhs.m_nVal << " )";
   return osIn;
}

// Return whether modulus of elem1 is greater than modulus of elem2
bool mod_lesser ( int elem1, int elem2 )
{
   if ( elem1 < 0 )
      elem1 = - elem1;
   if ( elem2 < 0 )
      elem2 = - elem2;
   return elem1 < elem2;
};

int main()
{
   // Searching a set container with elements of type CInt
   // for the maximum element
   CInt c1 = 1, c2 = 2, c3 = -3;
   set<CInt> s1;
   set<CInt>::iterator s1_Iter, s1_R1_Iter, s1_R2_Iter;

   s1.insert ( c1 );
   s1.insert ( c2 );
   s1.insert ( c3 );

   cout << "s1 = (";
   for ( s1_Iter = s1.begin( ); s1_Iter != --s1.end( ); s1_Iter++ )
      cout << " " << *s1_Iter << ",";
   s1_Iter = --s1.end( );
   cout << " " << *s1_Iter << " )." << endl;

   s1_R1_Iter = max_element ( s1.begin( ), s1.end( ) );

   cout << "The largest element in s1 is: " << *s1_R1_Iter << endl;
   cout << endl;

   // Searching a vector with elements of type int for the maximum
   // element under default less than & mod_lesser binary predicates
   vector <int> v1;
   vector <int>::iterator v1_Iter, v1_R1_Iter, v1_R2_Iter;

   int i;
   for ( i = 0 ; i <= 3 ; i++ )
   {
      v1.push_back( i );
   }

   int ii;
   for ( ii = 1 ; ii <= 4 ; ii++ )
   {
      v1.push_back( - 2 * ii );
   }

   cout << "Vector v1 is ( " ;
   for ( v1_Iter = v1.begin( ) ; v1_Iter != v1.end( ) ; v1_Iter++ )
      cout << *v1_Iter << " ";
   cout << ")." << endl;

   v1_R1_Iter = max_element ( v1.begin( ), v1.end( ) );
   v1_R2_Iter = max_element ( v1.begin( ), v1.end( ), mod_lesser);

   cout << "The largest element in v1 is: " << *v1_R1_Iter << endl;
   cout << "The largest element in v1 under the mod_lesser"
        << "\n binary predicate is: " << *v1_R2_Iter << endl;
}
```

## <a name="merge"></a>  merge

Объединяет все элементы из двух исходных упорядоченных диапазонов в один упорядоченный диапазон назначения, где критерий порядка сортировки может быть указан бинарным предикатом.

```cpp
template<class InputIterator1, class InputIterator2, class OutputIterator>
OutputIterator merge(
    InputIterator1 first1,
    InputIterator1 last1,
    InputIterator2 first2,
    InputIterator2 last2,
    OutputIterator result );

template<class InputIterator1, class InputIterator2, class OutputIterator, class BinaryPredicate>
OutputIterator merge(
    InputIterator1 first1,
    InputIterator1 last1,
    InputIterator2 first2,
    InputIterator2 last2,
    OutputIterator result,
    BinaryPredicate comp );

```

### <a name="parameters"></a>Параметры

*first1*<br/>
Входной итератор, обращающийся к позиции первого элемента в первом из двух упорядоченных исходных диапазонов, которые следует объединить и упорядочить в один диапазон.

*last1*<br/>
Входной итератор, обращающийся к позиции, следующей за последним элементом в первом из двух упорядоченных исходных диапазонов, которые следует объединить и упорядочить в один диапазон.

*first2*<br/>
Входной итератор, обращающийся к позиции первого элемента во втором из двух последовательных упорядоченных исходных диапазонов, которые следует объединить и упорядочить в один диапазон.

*last2*<br/>
Входной итератор, обращающийся к позиции, следующей за последним элементом во втором из двух последовательных упорядоченных исходных диапазонов, которые следует объединить и упорядочить в один диапазон.

*результат*<br/>
Выходной итератор, обращающийся к позиции первого элемента в диапазоне назначения, где два исходных диапазона следует объединить в один диапазон.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, определяющий условие, когда один элемент больше другого. Бинарный предикат принимает два аргумента и должен возвращать значение **true** , когда первый элемент меньше второго элемента, и значение **false** в противном случае.

### <a name="return-value"></a>Возвращаемое значение

Выходной итератор, указывающий на позицию, следующую за последним элементом, в упорядоченном диапазоне назначения.

### <a name="remarks"></a>Примечания

Упорядоченные исходные диапазоны, на которые указывают ссылки, должны быть допустимыми. Все указатели должны поддерживать отмену ссылок. В каждой последовательности должна быть возможность достижения последней позиции с первой путем приращения.

Диапазон назначения не должен перекрывать исходные диапазоны и должен быть достаточно большим, чтобы содержать диапазон назначения.

Каждый упорядоченный исходный диапазон должны быть упорядочен в качестве предусловия для применения алгоритма `merge` в соответствии с теми же правилами, чтобы использоваться алгоритмом для упорядочения объединенных диапазонов.

Операция стабильна, так как в диапазоне назначения сохраняется относительный порядок элементов в каждом диапазоне. Алгоритм не изменяет исходные диапазоны `merge`.

В целях упорядочения типы значений входных итераторов должны подлежать сравнению "меньше чем" для установления такого порядка, чтобы, имея два элемента, можно было определить, что они равны (ни один не меньше другого) или что один меньше другого. Это приводит к упорядочению неравнозначных элементов. Если эквивалентные элементы имеются в обоих исходных диапазонах, в диапазоне назначения элементы из первого диапазона будут предшествовать элементам из второго исходного диапазона.

Отношение сложности алгоритма линейное с не более (* last1 - first1 *)-(* last2 - first2*) – 1 сравнений.

Класс [list](../standard-library/list-class.md) предоставляет функцию-член merge для слияния элементов двух списков.

### <a name="example"></a>Пример

```cpp
// alg_merge.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <functional>   // For greater<int>( )
#include <iostream>

// Return whether modulus of elem1 is less than modulus of elem2
bool mod_lesser ( int elem1, int elem2 ) {
   if (elem1 < 0)
      elem1 = - elem1;
   if (elem2 < 0)
      elem2 = - elem2;
   return elem1 < elem2;
}

int main() {
   using namespace std;
   vector <int> v1a, v1b, v1 ( 12 );
   vector <int>::iterator Iter1a,  Iter1b, Iter1;

   // Constructing vector v1a and v1b with default less than ordering
   int i;
   for ( i = 0 ; i <= 5 ; i++ )
      v1a.push_back(  i );

   int ii;
   for ( ii =-5 ; ii <= 0 ; ii++ )
      v1b.push_back(  ii  );

   cout << "Original vector v1a with range sorted by the\n "
        << "binary predicate less than is  v1a = ( " ;
   for ( Iter1a = v1a.begin( ) ; Iter1a != v1a.end( ) ; Iter1a++ )
      cout << *Iter1a << " ";
   cout << ")." << endl;

   cout << "Original vector v1b with range sorted by the\n "
        << "binary predicate less than is  v1b = ( " ;
   for ( Iter1b = v1b.begin( ) ; Iter1b != v1b.end( ) ; Iter1b++ )
      cout << *Iter1b << " ";
   cout << ")." << endl;

   // Constructing vector v2 with ranges sorted by greater
   vector <int> v2a ( v1a ) , v2b ( v1b ) ,  v2 ( v1 );
   vector <int>::iterator Iter2a,  Iter2b, Iter2;
   sort ( v2a.begin( ), v2a.end( ), greater<int>( ) );
   sort ( v2b.begin( ), v2b.end( ), greater<int>( ) );

   cout << "Original vector v2a with range sorted by the\n "
        <<  "binary predicate greater is   v2a =  ( " ;
   for ( Iter2a = v2a.begin( ) ; Iter2a != v2a.end( ) ; Iter2a++ )
      cout << *Iter2a << " ";
   cout << ")." << endl;

   cout << "Original vector v2b with range sorted by the\n "
        <<  "binary predicate greater is   v2b =  ( " ;
   for ( Iter2b = v2b.begin( ) ; Iter2b != v2b.end( ) ; Iter2b++ )
      cout << *Iter2b << " ";
   cout << ")." << endl;

   // Constructing vector v3 with ranges sorted by mod_lesser
   vector <int> v3a ( v1a ), v3b ( v1b ) ,  v3 ( v1 );
   vector <int>::iterator Iter3a,  Iter3b, Iter3;
   sort ( v3a.begin( ), v3a.end( ), mod_lesser );
   sort ( v3b.begin( ), v3b.end( ), mod_lesser );

   cout << "Original vector v3a with range sorted by the\n "
        << "binary predicate mod_lesser is   v3a =  ( " ;
   for ( Iter3a = v3a.begin( ) ; Iter3a != v3a.end( ) ; Iter3a++ )
      cout << *Iter3a << " ";
   cout << ")." << endl;

   cout << "Original vector v3b with range sorted by the\n "
        << "binary predicate mod_lesser is   v3b =  ( " ;
   for ( Iter3b = v3b.begin( ) ; Iter3b != v3b.end( ) ; Iter3b++ )
      cout << *Iter3b << " ";
   cout << ")." << endl;

   // To merge inplace in ascending order with default binary
   // predicate less <int>( )
   merge ( v1a.begin( ), v1a.end( ), v1b.begin( ), v1b.end( ), v1.begin( ) );
   cout << "Merged inplace with default order,\n vector v1mod =  ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // To merge inplace in descending order, specify binary
   // predicate greater<int>( )
   merge ( v2a.begin( ), v2a.end( ), v2b.begin( ), v2b.end( ),
       v2.begin( ),  greater <int>( ) );
   cout << "Merged inplace with binary predicate greater specified,\n "
        << "vector v2mod  = ( " ;
   for ( Iter2 = v2.begin( ) ; Iter2 != v2.end( ) ; Iter2++ )
      cout << *Iter2 << " ";
   cout << ")." << endl;

   // Applying A user-defined (UD) binary predicate mod_lesser
   merge ( v3a.begin( ), v3a.end( ), v3b.begin( ), v3b.end( ),
       v3.begin( ),  mod_lesser );
   cout << "Merged inplace with binary predicate mod_lesser specified,\n "
        << "vector v3mod  = ( " ; ;
   for ( Iter3 = v3.begin( ) ; Iter3 != v3.end( ) ; Iter3++ )
      cout << *Iter3 << " ";
   cout << ")." << endl;
}
```

## <a name="min"></a>  min

Сравнивает два объекта и возвращает меньший из них, где критерий упорядочивания может быть указан бинарным предикатом.

```cpp
template<class Type>
constexpr const Type& min(
    const Type& left,
    const Type& right);
template<class Type, class Pr>
constexpr const Type& min(
    const Type& left,
    const Type& right,
    BinaryPredicate comp);
template<class Type>
constexpr Type min(
    initializer_list<Type> );
template<class Type, class Pr>
constexpr Type min(
    initializer_list<Type>,
    BinaryPredicate comp);

```

### <a name="parameters"></a>Параметры

*left*<br/>
Первый из сравниваемых объектов.

*right*<br/>
Второй из сравниваемых объектов.

*Зап.*<br/>
Двоичный предикат, используемый для сравнения двух объектов.

*_IList*<br/>
Списокinitializer_list с объектами для сравнения.

### <a name="return-value"></a>Возвращаемое значение

Меньший из двух объектов; если ни один из них не меньше, то возвращается первый из двух объектов. В случае с initializer_list возвращается наименьший из объектов в списке.

### <a name="remarks"></a>Примечания

При использовании алгоритма `min` очень редко объекты передаются как параметры. Большинство алгоритмов библиотеки стандартных программ C++ работают в диапазоне элементов, позиция которых задается итераторами, передаваемыми в качестве параметров. Если требуется функция, которая работает в диапазоне элементов, используйте [min_element](../standard-library/algorithm-functions.md#min_element). [constexpr](../cpp/constexpr-cpp.md) была включена на `initializer_list` перегрузки в Visual Studio 2017.

### <a name="example"></a>Пример

```cpp
// alg_min.cpp
// compile with: /EHsc
#include <vector>
#include <set>
#include <algorithm>
#include <iostream>
#include <ostream>

using namespace std;
class CInt;
ostream& operator<<( ostream& osIn, const CInt& rhs );

class CInt
{
public:
    CInt( int n = 0 ) : m_nVal( n ){}
    CInt( const CInt& rhs ) : m_nVal( rhs.m_nVal ){}
    CInt& operator=( const CInt& rhs ) {m_nVal =
    rhs.m_nVal; return *this;}
    bool operator<( const CInt& rhs ) const
        {return ( m_nVal < rhs.m_nVal );}
    friend ostream& operator<<(ostream& osIn, const CInt& rhs);

private:
    int m_nVal;
};

inline ostream& operator<<( ostream& osIn, const CInt& rhs )
{
    osIn << "CInt( " << rhs.m_nVal << " )";
       return osIn;
}

// Return whether modulus of elem1 is less than modulus of elem2
bool mod_lesser ( int elem1, int elem2 )
{
    if ( elem1 < 0 )
        elem1 = - elem1;
    if ( elem2 < 0 )
        elem2 = - elem2;
    return elem1 < elem2;
};

int main()
{
    // Comparing integers directly using the min algorithm with
    // binary predicate mod_lesser & with default less than
    int a = 6, b = -7, c = 7 ;
    const int& result1 = min ( a, b, mod_lesser );
    const int& result2 = min ( b, c );

    cout << "The mod_lesser of the integers 6 & -7 is: "
        << result1 << "." << endl;
    cout << "The lesser of the integers -7 & 7 is: "
        << result2 << "." << endl;
    cout << endl;

// Comparing the members of an initializer_list
    const int& result3 = min({ a, c });
    const int& result4 = min({ a, b }, mod_lesser);

    cout << "The lesser of the integers 6 & 7 is: "
        << result3 << "." << endl;
    cout << "The mod_lesser of the integers 6 & -7 is: "
        << result4 << "." << endl;
    cout << endl;

    // Comparing set containers with elements of type CInt
       // using the min algorithm
    CInt c1 = 1, c2 = 2, c3 = 3;
    set<CInt> s1, s2, s3;
    set<CInt>::iterator s1_Iter, s2_Iter, s3_Iter;

    s1.insert ( c1 );
    s1.insert ( c2 );
    s2.insert ( c2 );
    s2.insert ( c3 );

    cout << "s1 = (";
    for ( s1_Iter = s1.begin( ); s1_Iter != --s1.end( ); s1_Iter++ )
        cout << " " << *s1_Iter << ",";
    s1_Iter = --s1.end( );
        cout << " " << *s1_Iter << " )." << endl;

    cout << "s2 = (";
    for ( s2_Iter = s2.begin( ); s2_Iter != --s2.end( ); s2_Iter++ )
        cout << " " << *s2_Iter << ",";
    s2_Iter = --s2.end( );
    cout << " " << *s2_Iter << " )." << endl;

    s3 = min ( s1, s2 );
    cout << "s3 = min ( s1, s2 ) = (";
    for ( s3_Iter = s3.begin( ); s3_Iter != --s3.end( ); s3_Iter++ )
        cout << " " << *s3_Iter << ",";
    s3_Iter = --s3.end( );
    cout << " " << *s3_Iter << " )." << endl << endl;

    // Comparing vectors with integer elements using min algorithm
    vector <int> v1, v2, v3, v4, v5;
    vector <int>::iterator Iter1, Iter2, Iter3, Iter4, Iter5;

    int i;
    for ( i = 0 ; i <= 2 ; i++ )
    {
        v1.push_back( i );
    }

    int ii;
    for ( ii = 0 ; ii <= 2 ; ii++ )
    {
        v2.push_back( ii );
    }

    int iii;
    for ( iii = 0 ; iii <= 2 ; iii++ )
    {
        v3.push_back( 2 * iii );
    }

    cout << "Vector v1 is ( " ;
    for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
        cout << *Iter1 << " ";
    cout << ")." << endl;

    cout << "Vector v2 is ( " ;
    for ( Iter2 = v2.begin( ) ; Iter2 != v2.end( ) ; Iter2++ )
        cout << *Iter2 << " ";
    cout << ")." << endl;

    cout << "Vector v3 is ( " ;
    for ( Iter3 = v3.begin( ) ; Iter3 != v3.end( ) ; Iter3++ )
        cout << *Iter3 << " ";
    cout << ")." << endl;

    v4 = min ( v1, v2 );
    v5 = min ( v1, v3 );

    cout << "Vector v4 = min ( v1,v2 ) is ( " ;
    for ( Iter4 = v4.begin( ) ; Iter4 != v4.end( ) ; Iter4++ )
        cout << *Iter4 << " ";
    cout << ")." << endl;

    cout << "Vector v5 = min ( v1,v3 ) is ( " ;
    for ( Iter5 = v5.begin( ) ; Iter5 != v5.end( ) ; Iter5++ )
        cout << *Iter5 << " ";
    cout << ")." << endl;
}
```

```Output
The mod_lesser of the integers 6 & -7 is: 6.
The lesser of the integers -7 & 7 is: -7.
The lesser of the integers 6 & 7 is: 6.The mod_lesser of the integers 6 & -7 is: 6.
s1 = ( CInt( 1 ), CInt( 2 ) ).
s2 = ( CInt( 2 ), CInt( 3 ) ).
s3 = min ( s1, s2 ) = ( CInt( 1 ), CInt( 2 ) ).

Vector v1 is ( 0 1 2 ).
Vector v2 is ( 0 1 2 ).
Vector v3 is ( 0 2 4 ).
Vector v4 = min ( v1,v2 ) is ( 0 1 2 ).
Vector v5 = min ( v1,v3 ) is ( 0 1 2 ).
```

## <a name="min_element"></a>  min_element

Находит первое вхождение наименьшего элемента в указанном диапазоне, где критерий упорядочивания может быть указан бинарным предикатом.

```cpp
template<class ForwardIterator>
constexpr ForwardIterator min_element(ForwardIterator first, ForwardIterator last );

template<class ForwardIterator, class BinaryPredicate>
constexpr ForwardIterator min_element(
    ForwardIterator first,
    ForwardIterator last,
    BinaryPredicate comp);

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Прямой итератор, указывающий положение первого элемента в диапазоне для поиска наименьшего элемента.

*последний*<br/>
Прямой итератор, указывающий положение, следующее за последним элементом в диапазоне для поиска наименьшего элемента.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, определяющий условие, когда один элемент больше другого. Бинарный предикат принимает два аргумента и должен возвращать значение **true** , когда первый элемент меньше второго элемента, и значение **false** в противном случае.

### <a name="return-value"></a>Возвращаемое значение

Прямой итератор, указывающий положение первого вхождения наименьшего элемента в диапазоне для поиска.

### <a name="remarks"></a>Примечания

Диапазоны, на которые указывают ссылки, должны быть допустимыми; все указатели должны поддерживать сброс ссылок; в каждой последовательности должна быть возможность достижения последнего положения с первого путем приращения.

Отношение сложности линейное: (`last` - `first`) – 1 сравнений для непустого диапазона требуется.

### <a name="example"></a>Пример

```cpp
// alg_min_element.cpp
// compile with: /EHsc
#include <vector>
#include <set>
#include <algorithm>
#include <iostream>
#include <ostream>

using namespace std;
class CInt;
ostream& operator<<( ostream& osIn, const CInt& rhs );

class CInt
{
public:
   CInt( int n = 0 ) : m_nVal( n ){}
   CInt( const CInt& rhs ) : m_nVal( rhs.m_nVal ){}
   CInt& operator=( const CInt& rhs ) {m_nVal =
   rhs.m_nVal; return *this;}
   bool operator<( const CInt& rhs ) const
      {return ( m_nVal < rhs.m_nVal );}
   friend ostream& operator<<( ostream& osIn, const CInt& rhs );

private:
   int m_nVal;
};

inline ostream& operator<<( ostream& osIn, const CInt& rhs )
{
   osIn << "CInt( " << rhs.m_nVal << " )";
   return osIn;
}

// Return whether modulus of elem1 is less than modulus of elem2
bool mod_lesser ( int elem1, int elem2 )
{
   if ( elem1 < 0 )
      elem1 = - elem1;
   if ( elem2 < 0 )
      elem2 = - elem2;
   return elem1 < elem2;
};

int main()
{
   // Searching a set container with elements of type CInt
   // for the minimum element
   CInt c1 = 1, c2 = 2, c3 = -3;
   set<CInt> s1;
   set<CInt>::iterator s1_Iter, s1_R1_Iter, s1_R2_Iter;

   s1.insert ( c1 );
   s1.insert ( c2 );
   s1.insert ( c3 );

   cout << "s1 = (";
   for ( s1_Iter = s1.begin( ); s1_Iter != --s1.end( ); s1_Iter++ )
      cout << " " << *s1_Iter << ",";
   s1_Iter = --s1.end( );
   cout << " " << *s1_Iter << " )." << endl;

   s1_R1_Iter = min_element ( s1.begin( ), s1.end( ) );

   cout << "The smallest element in s1 is: " << *s1_R1_Iter << endl;
   cout << endl;

   // Searching a vector with elements of type int for the maximum
   // element under default less than & mod_lesser binary predicates
   vector <int> v1;
   vector <int>::iterator v1_Iter, v1_R1_Iter, v1_R2_Iter;

   int i;
   for ( i = 0 ; i <= 3 ; i++ )
   {
      v1.push_back( i );
   }

   int ii;
   for ( ii = 1 ; ii <= 4 ; ii++ )
   {
      v1.push_back( - 2 * ii );
   }

   cout << "Vector v1 is ( " ;
   for ( v1_Iter = v1.begin( ) ; v1_Iter != v1.end( ) ; v1_Iter++ )
      cout << *v1_Iter << " ";
   cout << ")." << endl;

   v1_R1_Iter = min_element ( v1.begin( ), v1.end( ) );
   v1_R2_Iter = min_element ( v1.begin( ), v1.end( ), mod_lesser);

   cout << "The smallest element in v1 is: " << *v1_R1_Iter << endl;
   cout << "The smallest element in v1 under the mod_lesser"
        << "\n binary predicate is: " << *v1_R2_Iter << endl;
}
```

```Output
s1 = ( CInt( -3 ), CInt( 1 ), CInt( 2 ) ).
The smallest element in s1 is: CInt( -3 )

Vector v1 is ( 0 1 2 3 -2 -4 -6 -8 ).
The smallest element in v1 is: -8
The smallest element in v1 under the mod_lesser
binary predicate is: 0
```

## <a name="minmax_element"></a>  minmax_element

Выполняет работу, которую делают `min_element` и `max_element`, в одном вызове.

```cpp
template<class ForwardIterator>
constexpr pair<ForwardIterator, ForwardIterator> minmax_element(
    ForwardIterator first,
    ForwardIterator Last);
template<class ForwardIterator, class BinaryPredicate>
constexpr pair<ForwardIterator, ForwardIterator> minmax_element(
    ForwardIterator  first,
    ForwardIterator Last,
    BinaryPredicate  comp);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Прямой итератор, указывающий начало диапазона.

*последний*<br/>
Прямой итератор, указывающий конец диапазона.

*Зап.*<br/>
Дополнительный тест, используемый для упорядочивания элементов.

### <a name="return-value"></a>Возвращаемое значение

Returns

`pair<ForwardIterator, ForwardIterator>`

`(` [min_element](../standard-library/algorithm-functions.md#min_element)`(first, last), `[max_element](../standard-library/algorithm-functions.md#max_element)`(first, last))`.

### <a name="remarks"></a>Примечания

Первая функция шаблона возвращает

`pair<ForwardIterator,ForwardIterator>`

`(min_element(_First,Last), max_element(_First,Last))`.

Вторая функция шаблона работает так же, за исключением того, что она заменяет `operator<(X, Y)` на `comp (X, Y)`.

Если последовательность является пустым, функция выполняет не более `3 * (last - first - 1) / 2` сравнения.

## <a name="minmax"></a>  minmax

Сравнивает два входных параметра и возвращает их в виде пары, в порядке от меньшего к большему.

```cpp
template<class Type>
constexpr pair<const Type&, const Type&> minmax(
    const Type& left,
    const Type& right);
template<class Type, class BinaryPredicate>
constexpr pair<const Type&, const Type&> minmax(
    const Type& left,
    const Type& right,
    BinaryPredicate comp);
template<class Type>
constexpr pair<Type&, Type&> minmax(
    initializer_list<Type> );
template<class Type, class BinaryPredicate>
constexpr pair<Type&, Type&> minmax(
    initializer_list<Type>,
    BinaryPredicate comp);

```

### <a name="parameters"></a>Параметры

*left*<br/>
Первый из сравниваемых объектов.

*right*<br/>
Второй из сравниваемых объектов.

*Зап.*<br/>
Двоичный предикат, используемый для сравнения двух объектов.

*_IList*<br/>
Списокinitializer_list с объектами для сравнения.

### <a name="remarks"></a>Примечания

Первая функция-шаблон возвращает `pair<const Type&, const Type&>( right , left )` Если *правой* — меньше, чем *левой*. В противном случае возвращает значение `pair<const Type&, const Type&>( left , right )`.

Вторая функция-член возвращает пару, где первый элемент меньше, а второй — больше при сравнении по предикату *comp*.

Остальные функции шаблона действуют одинаково, за исключением того, что они заменяют *левой* и *правой* параметров с *_IList*.

Функция выполняет точно одно сравнение.

## <a name="mismatch"></a>  mismatch

Сравнивает поэлементно два диапазона и находит первую позицию, где элементы отличаются.

Используйте двух-диапазонные перегрузки в коде C++ 14. Перегрузки, использующие только один итератор для второго диапазона, не обнаруживают различия в тех случаях, когда второй диапазон длиннее, чем первый, и их поведение может быть непредсказуемо, если второй диапазон короче, чем первый.

```cpp
template<class InputIterator1, class InputIterator2>
pair<InputIterator1, InputIterator2>>
mismatch(
    InputIterator1 First1,
    InputIterator1 Last1,
    InputIterator2 First2 );

template<class InputIterator1, class InputIterator2, class BinaryPredicate> pair<InputIterator1, InputIterator2>>
mismatch(
    InputIterator1 First1,
    InputIterator1 Last1,
    InputIterator2 First2,
    BinaryPredicate Comp );

//C++14
template<class InputIterator1, class InputIterator2>
pair<InputIterator1, InputIterator2>>
mismatch(
    InputIterator1 First1,
    InputIterator1 Last1,
    InputIterator2 First2,
    InputIterator2 Last2 );

template<class InputIterator1, class InputIterator2, class BinaryPredicate> pair<InputIterator1, InputIterator2>>
mismatch(
    InputIterator1 First1,
    InputIterator1 Last1,
    InputIterator2 First2,
    InputIterator2 Last2,
    BinaryPredicate Comp);
```

### <a name="parameters"></a>Параметры

*first1*<br/>
Входной итератор, указывающий на положение первого элемента в первом диапазоне для тестирования.

*last1*<br/>
Входной итератор, указывающий на положение, следующее за последним элементом, в первом диапазоне для тестирования.

*first2*<br/>
Входной итератор, указывающий на положение первого элемента во втором диапазоне для тестирования.

*last2*<br/>
Входной итератор, указывающий на положение, следующее за последним элементом, во втором диапазоне для тестирования.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, который сравнивает текущие элементы в каждом диапазоне и определяет, являются ли они равными. Он возвращает значение **true** при выполнении условия и значение **false** — в противном случае.

### <a name="return-value"></a>Возвращаемое значение

Пара итераторов, указывающих на положения несовпадений в двух диапазонах: первый компонентный итератор — на положение в первом диапазоне, второй итератор — на положение во втором диапазоне. Если между элементами сравниваемых диапазонов нет разницы или если бинарный предикат во второй версии показывает соответствие для всех пар элементов из двух диапазонов, то первый компонентный итератор указывает на положение, следующее за последним проверенным элементом в первом диапазоне, а второй итератор — на положение, следующее за последним проверенным элементом во втором диапазоне.

### <a name="remarks"></a>Примечания

При выполнении первой функции шаблона предполагается, что в диапазоне, начинающемся с first2, имеется столько же элементов, сколько в диапазоне, указанном аргументами [first1, last1). Если во втором диапазоне элементов больше, они игнорируются. Если элементов меньше — результат будет непредсказуемым.

Диапазон, по которому ведется поиск, должен быть допустимым. Все итераторы должны поддерживать сброс ссылок и должна быть возможность достижения последнего положения, начиная от первого, путем приращения.

Временная сложность алгоритма линейно зависит от количества элементов в более коротком диапазоне.

Применение определяемого пользователем предиката не требуется для наложения отношения эквивалентности (симметричной, рефлексивной и транзитивной) между операндами.

### <a name="example"></a>Пример

В следующем примере демонстрируется использование несовпадения. Перегрузка C++ 03 показана только с целью демонстрации того, как она может привести к непредвиденному результату.

```cpp
#include <vector>
#include <list>
#include <algorithm>
#include <iostream>
#include <string>
#include <utility>

using namespace std;

// Return whether first element is twice the second
// Note that this is not a symmetric, reflexive and transitive equivalence.
// mismatch and equal accept such predicates, but is_permutation does not.
bool twice(int elem1, int elem2)
{
    return elem1 == elem2 * 2;
}

void PrintResult(const string& msg, const pair<vector<int>::iterator, vector<int>::iterator>& result,
    const vector<int>& left, const vector<int>& right)
{
    // If either iterator stops before reaching the end of its container,
    // it means a mismatch was detected.
    if (result.first != left.end() || result.second != right.end())
    {
        string leftpos(result.first == left.end() ? "end" : to_string(*result.first));
        string rightpos(result.second == right.end() ? "end" : to_string(*result.second));
        cout << msg << "mismatch. Left iterator at " << leftpos
            << " right iterator at " << rightpos << endl;
    }
    else
    {
        cout << msg << " match." << endl;
    }
}

int main()
{

    vector<int> vec_1{ 0, 5, 10, 15, 20, 25 };
    vector<int> vec_2{ 0, 5, 10, 15, 20, 25, 30 };

    // Testing different length vectors for mismatch (C++03)
    auto match_vecs = mismatch(vec_1.begin(), vec_1.end(), vec_2.begin());
    bool is_mismatch = match_vecs.first != vec_1.end();
    cout << "C++03: vec_1 and vec_2 are a mismatch: " << boolalpha << is_mismatch << endl;

    // Using dual-range overloads:

    // Testing different length vectors for mismatch (C++14)
    match_vecs = mismatch(vec_1.begin(), vec_1.end(), vec_2.begin(), vec_2.end());
    PrintResult("C++14: vec_1 and vec_2: ", match_vecs, vec_1, vec_2);

    // Identify point of mismatch between vec_1 and modified vec_2.
    vec_2[3] = 42;
    match_vecs = mismatch(vec_1.begin(), vec_1.end(), vec_2.begin(), vec_2.end());
    PrintResult("C++14 vec_1 v. vec_2 modified: ", match_vecs, vec_1, vec_2);

    // Test vec_3 and vec_4 for mismatch under the binary predicate twice (C++14)
    vector<int> vec_3{ 10, 20, 30, 40, 50, 60 };
    vector<int> vec_4{ 5, 10, 15, 20, 25, 30 };
    match_vecs = mismatch(vec_3.begin(), vec_3.end(), vec_4.begin(), vec_4.end(), twice);
    PrintResult("vec_3 v. vec_4 with pred: ", match_vecs, vec_3, vec_4);

    vec_4[5] = 31;
    match_vecs = mismatch(vec_3.begin(), vec_3.end(), vec_4.begin(), vec_4.end(), twice);
    PrintResult("vec_3 v. modified vec_4 with pred: ", match_vecs, vec_3, vec_4);

    // Compare a vector<int> to a list<int>
    list<int> list_1{ 0, 5, 10, 15, 20, 25 };
    auto match_vec_list = mismatch(vec_1.begin(), vec_1.end(), list_1.begin(), list_1.end());
    is_mismatch = match_vec_list.first != vec_1.end() || match_vec_list.second != list_1.end();
    cout << "vec_1 and list_1 are a mismatch: " << boolalpha << is_mismatch << endl;

    char c;
    cout << "Press a key" << endl;
    cin >> c;

}

/*
Output:
C++03: vec_1 and vec_2 are a mismatch: false
C++14: vec_1 and vec_2: mismatch. Left iterator at end right iterator at 30
C++14 vec_1 v. vec_2 modified: mismatch. Left iterator at 15 right iterator at 42
C++14 vec_3 v. vec_4 with pred:  match.
C++14 vec_3 v. modified vec_4 with pred: mismatch. Left iterator at 60 right iterator at 31
C++14: vec_1 and list_1 are a mismatch: false
Press a key
*/

```

## <a name="alg_move"></a>  &lt;alg&gt; move

Перемещает элементы, связанные с заданным диапазоном.

```cpp
template<class InputIterator, class OutputIterator>
OutputIterator move(
    InputIterator first,
    InputIterator last,
    OutputIterator dest);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Входной итератор, указывающий, откуда начинается диапазон элементов для перемещения.

*последний*<br/>
Входной итератор, указывающий конец диапазона элементов для перемещения.

*dest*<br/>
Выходной итератор, который должен содержать перемещенные элементы.

### <a name="remarks"></a>Примечания

Функция шаблона проверяет `*(dest + N) = move(*(first + N))` один раз для каждого `N` в диапазоне `[0, last - first)`, строго на увеличение значений `N` начиная с наименьшего значения. Затем оно возвращает значение `dest + N`. Если `dest` и *первый* обозначают области хранилища, *dest* не должны находиться в диапазоне `[first, last)`.

## <a name="move_backward"></a>  move_backward

Перемещает элементы одного итератора в другой. Перемещение начинается с последнего элементом в указанном диапазоне и завершается первым элементом в этом диапазоне.

```cpp
template<class BidirectionalIterator1, class BidirectionalIterator2>
   BidirectionalIterator2 move_backward(
       BidirectionalIterator1 first,
       BidirectionalIterator1 last,
       BidirectionalIterator2 destEnd);

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Итератор, указывающий начало диапазона, из которого должны перемещаться элементы.

*последний*<br/>
Итератор, указывающий конец диапазона, из которого должны перемещаться элементы. Этот элемент не перемещается.

*destEnd*<br/>
Двунаправленный итератор, обращающийся к позиции, которая на единицу превышает позицию завершающего элемента в диапазоне назначения.

### <a name="remarks"></a>Примечания

Функция шаблона проверяет `*(destEnd - N - 1) = move(*(last - N - 1))` один раз для каждого `N` в диапазоне `[0, last - first)`, строго на увеличение значений `N` начиная с наименьшего значения. Затем оно возвращает значение `destEnd - (last - first)`. Если *destEnd* и *первый* обозначают области хранилища, *destEnd* не должны находиться в диапазоне `[first, last)`.

`move` и `move_backward` — функциональный эквивалент использованию `copy` и `copy_backward` с итератором перемещения.

## <a name="next_permutation"></a>  next_permutation

Изменяет порядок элементов в диапазоне, чтобы исходный порядок был заменен перестановкой "лексикографически следующий больший", если такая существует, где смысл термина "следующий" может быть задан бинарным предикатом.

```cpp
template<class BidirectionalIterator>
bool next_permutation(BidirectionalIterator first, BidirectionalIterator last);

template<class BidirectionalIterator, class BinaryPredicate>
bool next_permutation(BidirectionalIterator first, BidirectionalIterator last, BinaryPredicate comp);

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Двунаправленный итератор, указывающий позицию первого элемента в диапазоне, в котором переставляются элементы.

*последний*<br/>
Двунаправленный итератор, указывающий позицию, следующую за последним элементом в диапазоне, в котором переставляются элементы.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, задающий критерий сравнения, который должен соблюдаться идущими подряд элементами при упорядочении. Двоичный предикат принимает два аргумента и возвращает **true** , если условие удовлетворено, или **false** , если условие не удовлетворено.

### <a name="return-value"></a>Возвращаемое значение

Значение **true**, если лексикографически следующая перестановка существует и заменила исходный порядок в диапазоне; в противном случае — значение **false**, указывающее, что порядок преобразуется в лексикографически наименьшую перестановку.

### <a name="remarks"></a>Примечания

Указанный диапазон должен быть допустимым. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Двоичный предикат по умолчанию — "меньше чем", и элементы в диапазоне должны быть сравнимы на "меньше чем", чтобы следующая перестановка была задана правильно.

Отношение сложности линейное с не более (* фамилия - имя *) / 2 перестановок.

### <a name="example"></a>Пример

```cpp
// alg_next_perm.cpp
// compile with: /EHsc
#include <vector>
#include <deque>
#include <algorithm>
#include <iostream>
#include <ostream>

using namespace std;
class CInt;
ostream& operator<<( ostream& osIn, const CInt& rhs );

class CInt
{
public:
   CInt( int n = 0 ) : m_nVal( n ){}
   CInt( const CInt& rhs ) : m_nVal( rhs.m_nVal ){}
   CInt&   operator=( const CInt& rhs ) {m_nVal =
   rhs.m_nVal; return *this;}
   bool operator<( const CInt& rhs ) const
      { return ( m_nVal < rhs.m_nVal );}
   friend   ostream& operator<<( ostream& osIn, const CInt& rhs );

private:
   int m_nVal;
};

inline ostream& operator<<( ostream& osIn, const CInt& rhs )
{
   osIn << "CInt( " << rhs.m_nVal << " )";
   return osIn;
}

// Return whether modulus of elem1 is less than modulus of elem2
bool mod_lesser ( int elem1, int elem2 )
{
   if ( elem1 < 0 )
      elem1 = - elem1;
   if ( elem2 < 0 )
      elem2 = - elem2;
   return elem1 < elem2;
};

int main()
{
   // Reordering the elements of type CInt in a deque
   // using the prev_permutation algorithm
   CInt c1 = 5, c2 = 1, c3 = 10;
   bool deq1Result;
   deque<CInt> deq1, deq2, deq3;
   deque<CInt>::iterator d1_Iter;

   deq1.push_back ( c1 );
   deq1.push_back ( c2 );
   deq1.push_back ( c3 );

   cout << "The original deque of CInts is deq1 = (";
   for ( d1_Iter = deq1.begin( ); d1_Iter != --deq1.end( ); d1_Iter++ )
      cout << " " << *d1_Iter << ",";
   d1_Iter = --deq1.end( );
   cout << " " << *d1_Iter << " )." << endl;

   deq1Result = next_permutation ( deq1.begin( ), deq1.end( ) );

   if ( deq1Result )
      cout << "The lexicographically next permutation "
           << "exists and has\nreplaced the original "
           << "ordering of the sequence in deq1." << endl;
   else
      cout << "The lexicographically next permutation doesn't "
           << "exist\n and the lexicographically "
           << "smallest permutation\n has replaced the "
           << "original ordering of the sequence in deq1." << endl;

   cout << "After one application of next_permutation,\n deq1 = (";
   for ( d1_Iter = deq1.begin( ); d1_Iter != --deq1.end( ); d1_Iter++ )
      cout << " " << *d1_Iter << ",";
   d1_Iter = --deq1.end( );
   cout << " " << *d1_Iter << " )." << endl << endl;

   // Permuting vector elements with binary function mod_lesser
   vector <int> v1;
   vector <int>::iterator Iter1;

   int i;
   for ( i = -3 ; i <= 3 ; i++ )
   {
      v1.push_back( i );
   }

   cout << "Vector v1 is ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   next_permutation ( v1.begin( ), v1.end( ), mod_lesser );

   cout << "After the first next_permutation, vector v1 is:\n v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   int iii = 1;
   while ( iii <= 5 ) {
      next_permutation ( v1.begin( ), v1.end( ), mod_lesser );
      cout << "After another next_permutation of vector v1,\n v1 =   ( " ;
      for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ;Iter1 ++ )
         cout << *Iter1  << " ";
      cout << ")." << endl;
      iii++;
   }
}
```

```Output
The original deque of CInts is deq1 = ( CInt( 5 ), CInt( 1 ), CInt( 10 ) ).
The lexicographically next permutation exists and has
replaced the original ordering of the sequence in deq1.
After one application of next_permutation,
deq1 = ( CInt( 5 ), CInt( 10 ), CInt( 1 ) ).

Vector v1 is ( -3 -2 -1 0 1 2 3 ).
After the first next_permutation, vector v1 is:
v1 = ( -3 -2 -1 0 1 3 2 ).
After another next_permutation of vector v1,
v1 =   ( -3 -2 -1 0 2 1 3 ).
After another next_permutation of vector v1,
v1 =   ( -3 -2 -1 0 2 3 1 ).
After another next_permutation of vector v1,
v1 =   ( -3 -2 -1 0 3 1 2 ).
After another next_permutation of vector v1,
v1 =   ( -3 -2 -1 0 3 2 1 ).
After another next_permutation of vector v1,
v1 =   ( -3 -2 -1 1 0 2 3 ).
```

## <a name="nth_element"></a>  nth_element

Разделяет диапазон элементов, правильно находя *n*-й элемент последовательности в диапазоне, чтобы все элементы перед ним были меньше или равны ему, а все элементы в последовательности после него — больше либо равны ему.

```cpp
template<class RandomAccessIterator>
void nth_element( RandomAccessIterator first, RandomAccessIterator _Nth, RandomAccessIterator last);

template<class RandomAccessIterator, class BinaryPredicate>
void nth_element( RandomAccessIterator first, RandomAccessIterator _Nth, RandomAccessIterator last, BinaryPredicate comp);

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Итератор произвольного доступа, указывающий позицию первого элемента в разделяемом диапазоне.

*_Nth*<br/>
Итератор произвольного доступа, указывающий позицию элемента для правильного упорядочивания на границе раздела.

*последний*<br/>
Итератор произвольного доступа, обращающийся к позиции, следующей за последним элементом в разделяемом диапазоне.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, задающий критерий сравнения, который должен соблюдаться идущими подряд элементами при упорядочении. Двоичный предикат принимает два аргумента и возвращает **true** , если условие удовлетворено, или **false** , если условие не удовлетворено.

### <a name="remarks"></a>Примечания

Указанный диапазон должен быть допустимым. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Алгоритм `nth_element` не гарантирует упорядочивание элементов в поддиапазонах с каждой стороны *n*-го элемента. Таким образом, он дает меньшие гарантии, чем `partial_sort`, который упорядочивает элементы в диапазоне ниже некоторого выбранного элемента, и может использоваться в качестве более быстрой альтернативы `partial_sort`, когда упорядочивание нижнего диапазона не требуется.

Если ни один из элементов не меньше другого, то эти элементы эквивалентны, но не обязательно равны.

Средняя сложность сортировки линейная по отношению к * фамилия - имя *.

### <a name="example"></a>Пример

```cpp
// alg_nth_elem.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <functional>      // For greater<int>( )
#include <iostream>

// Return whether first element is greater than the second
bool UDgreater ( int elem1, int elem2 ) {
   return elem1 > elem2;
}

int main() {
   using namespace std;
   vector <int> v1;
   vector <int>::iterator Iter1;

   int i;
   for ( i = 0 ; i <= 5 ; i++ )
      v1.push_back( 3 * i );

   int ii;
   for ( ii = 0 ; ii <= 5 ; ii++ )
      v1.push_back( 3 * ii + 1 );

   int iii;
   for ( iii = 0 ; iii <= 5 ; iii++ )
      v1.push_back( 3 * iii +2 );

   cout << "Original vector:\n v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;

   nth_element(v1.begin( ), v1.begin( ) + 3, v1.end( ) );
   cout << "Position 3 partitioned vector:\n v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;

   // To sort in descending order, specify binary predicate
   nth_element( v1.begin( ), v1.begin( ) + 4, v1.end( ),
          greater<int>( ) );
   cout << "Position 4 partitioned (greater) vector:\n v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;

   random_shuffle( v1.begin( ), v1.end( ) );
   cout << "Shuffled vector:\n v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;

   // A user-defined (UD) binary predicate can also be used
   nth_element( v1.begin( ), v1.begin( ) + 5, v1.end( ), UDgreater );
   cout << "Position 5 partitioned (UDgreater) vector:\n v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;
}
```

## <a name="none_of"></a>  none_of

Возвращает **true** Если условие не выполняется ни одним элементом заданного диапазона.

```cpp
template<class InputIterator, class BinaryPredicate>
bool none_of(InputIterator first, InputIterator last, BinaryPredicate comp);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Входной итератор, указывающий, откуда должна начинаться проверка диапазона элементов на соответствие условию.

*последний*<br/>
Входной итератор, указывающий конец диапазона элементов.

*Зап.*<br/>
Условие для проверки. Это условие предоставляется определенным пользователем объектом функции предиката, который задает условие. Предикат принимает один аргумент и возвращает значение **true** или **false**.

### <a name="return-value"></a>Возвращаемое значение

Возвращает **true** Если условие не будет обнаружен по крайней мере один раз в указанном диапазоне соответствует условию, и **false** при обнаружении этого условия.

### <a name="remarks"></a>Примечания

Функция шаблона возвращает **true** только если для некоторых `N` в диапазоне `[0, last - first)`, предикат `comp(*(first + N))` всегда **false**.

## <a name="partial_sort"></a>  partial_sort

Упорядочивает указанное число меньших элементов в диапазоне в не нисходящий порядок или согласно критерию упорядочивания, заданному бинарным предикатом.

```cpp
template<class RandomAccessIterator>
void partial_sort(
    RandomAccessIterator first,
    RandomAccessIterator sortEnd,
    RandomAccessIterator last);

template<class RandomAccessIterator, class BinaryPredicate>
void partial_sort(
    RandomAccessIterator first,
    RandomAccessIterator sortEnd,
    RandomAccessIterator last
    BinaryPredicate comp);

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Итератор произвольного доступа, обращающийся к позиции первого элемента в сортируемом диапазоне.

*sortEnd*<br/>
Итератор произвольного доступа, обращающийся к позиции, следующей за последним элементом в сортируемом поддиапазоне.

*последний*<br/>
Итератор произвольного доступа, обращающийся к позиции, следующей за последним элементом в диапазоне для частичной сортировки.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, задающий критерий сравнения, который должен соблюдаться идущими подряд элементами при упорядочении. Двоичный предикат принимает два аргумента и возвращает **true** , если условие удовлетворено, или **false** , если условие не удовлетворено.

### <a name="remarks"></a>Примечания

Указанный диапазон должен быть допустимым. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Если ни один из элементов не меньше другого, то эти элементы эквивалентны, но не обязательно равны. `sort` Алгоритм нестабилен и не гарантирует, что относительный порядок эквивалентных элементов будет сохранен. Алгоритм `stable_sort` сохраняет этот исходный порядок.

Средняя сложность частичной сортировки — *O*((`last`- `first`) log (`sortEnd`- `first`)).

### <a name="example"></a>Пример

```cpp
// alg_partial_sort.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <functional>      // For greater<int>( )
#include <iostream>

// Return whether first element is greater than the second
bool UDgreater ( int elem1, int elem2 )
{
   return elem1 > elem2;
}

int main()
{
   using namespace std;
   vector <int> v1;
   vector <int>::iterator Iter1;

   int i;
   for ( i = 0 ; i <= 5 ; i++ )
   {
      v1.push_back( 2 * i );
   }

   int ii;
   for ( ii = 0 ; ii <= 5 ; ii++ )
   {
      v1.push_back( 2 * ii +1 );
   }

   cout << "Original vector:\n v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;

   partial_sort(v1.begin( ), v1.begin( ) + 6, v1.end( ) );
   cout << "Partially sorted vector:\n v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;

   // To partially sort in descending order, specify binary predicate
   partial_sort(v1.begin( ), v1.begin( ) + 4, v1.end( ), greater<int>( ) );
   cout << "Partially resorted (greater) vector:\n v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;

   // A user-defined (UD) binary predicate can also be used
   partial_sort(v1.begin( ), v1.begin( ) + 8, v1.end( ),
UDgreater );
   cout << "Partially resorted (UDgreater) vector:\n v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;
}
```

```Output
Original vector:
v1 = ( 0 2 4 6 8 10 1 3 5 7 9 11 )
Partially sorted vector:
v1 = ( 0 1 2 3 4 5 10 8 6 7 9 11 )
Partially resorted (greater) vector:
v1 = ( 11 10 9 8 0 1 2 3 4 5 6 7 )
Partially resorted (UDgreater) vector:
v1 = ( 11 10 9 8 7 6 5 4 0 1 2 3 )
```

## <a name="partial_sort_copy"></a>  partial_sort_copy

Копирует элементы из исходного диапазона в диапазон назначения, где исходные элементы упорядочены по критерию "меньше либо равно" или согласно другому заданному бинарному предикату.

```cpp
template<class InputIterator, class RandomAccessIterator>
RandomAccessIterator partial_sort_copy(
    InputIterator first1,
    InputIterator last1,
    RandomAccessIterator first2,
    RandomAccessIterator last2 );

template<class InputIterator, class RandomAccessIterator, class BinaryPredicate>
RandomAccessIterator partial_sort_copy(
    InputIterator first1,
    InputIterator last1,
    RandomAccessIterator first2,
    RandomAccessIterator last2,
    BinaryPredicate comp);
```

### <a name="parameters"></a>Параметры

*first1*<br/>
Итератор ввода, обращающийся к позиции первого элемента в исходном диапазоне.

*last1*<br/>
Входной итератор, указывающий позицию, следующую за последним элементом в исходном диапазоне.

*first2*<br/>
Итератор произвольного доступа, указывающий позицию первого элемента в сортируемом диапазоне назначения.

*last2*<br/>
Итератор произвольного доступа, указывающий позицию, следующую за последним элементом в сортируемом диапазоне назначения.

*Зап.*<br/>
Заданный пользователем объект функции предиката, определяющий условие, которое должно выполняться, чтобы два элемента считались эквивалентными друг другу. Двоичный предикат принимает два аргумента и возвращает **true** , если условие удовлетворено, или **false** , если условие не удовлетворено.

### <a name="return-value"></a>Возвращаемое значение

Итератор произвольного доступа, указывающий элемент в диапазоне назначения, находящийся на позиции, следующей за последним элементом, вставленным из исходного диапазона.

### <a name="remarks"></a>Примечания

Исходный диапазон и диапазон назначения не должны перекрываться и должны быть допустимыми. Все указатели должны поддерживать удаление ссылок, а последняя позиция в каждой последовательности должна быть доступна из первой позиции путем приращения.

Бинарный предикат должен предоставлять строгую квазиупорядоченность, чтобы элементы, которые не являются эквивалентными, упорядочивались, а эквивалентные элементы — нет. Два элемента эквивалентны в рамках условия "меньше чем", но они не обязательно равны, если ни один из элементов не меньше другого.

### <a name="example"></a>Пример

```cpp
// alg_partial_sort_copy.cpp
// compile with: /EHsc
#include <vector>
#include <list>
#include <algorithm>
#include <functional>
#include <iostream>

int main() {
    using namespace std;
    vector<int> v1, v2;
    list<int> list1;
    vector<int>::iterator iter1, iter2;
    list<int>::iterator list1_Iter, list1_inIter;

    int i;
    for (i = 0; i <= 9; i++)
        v1.push_back(i);

    random_shuffle(v1.begin(), v1.end());

    list1.push_back(60);
    list1.push_back(50);
    list1.push_back(20);
    list1.push_back(30);
    list1.push_back(40);
    list1.push_back(10);

    cout << "Vector v1 = ( " ;
    for (iter1 = v1.begin(); iter1 != v1.end(); iter1++)
        cout << *iter1 << " ";
    cout << ")" << endl;

    cout << "List list1 = ( " ;
    for (list1_Iter = list1.begin();
         list1_Iter!= list1.end();
         list1_Iter++)
        cout << *list1_Iter << " ";
    cout << ")" << endl;

    // Copying a partially sorted copy of list1 into v1
    vector<int>::iterator result1;
    result1 = partial_sort_copy(list1.begin(), list1.end(),
             v1.begin(), v1.begin() + 3);

    cout << "List list1 Vector v1 = ( " ;
    for (iter1 = v1.begin() ; iter1 != v1.end() ; iter1++)
        cout << *iter1 << " ";
    cout << ")" << endl;
    cout << "The first v1 element one position beyond"
         << "\n the last L 1 element inserted was " << *result1
         << "." << endl;

    // Copying a partially sorted copy of list1 into v2
    int ii;
    for (ii = 0; ii <= 9; ii++)
        v2.push_back(ii);

    random_shuffle(v2.begin(), v2.end());
    vector<int>::iterator result2;
    result2 = partial_sort_copy(list1.begin(), list1.end(),
             v2.begin(), v2.begin() + 6);

    cout << "List list1 into Vector v2 = ( " ;
    for (iter2 = v2.begin() ; iter2 != v2.end(); iter2++)
        cout << *iter2 << " ";
    cout << ")" << endl;
    cout << "The first v2 element one position beyond"
         << "\n the last L 1 element inserted was " << *result2
         << "." << endl;
}
```

## <a name="partition"></a>  partition

Разделяет элементы диапазона на два непересекающихся множества, при этом элементы, удовлетворяющие унарному предикату, расположены перед теми, которые ему не удовлетворяют.

```cpp
template<class BidirectionalIterator, class Predicate>
BidirectionalIterator partition(
    BidirectionalIterator first,
    BidirectionalIterator last,
    Predicate comp);

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Двунаправленный итератор адресует позицию первого элемента в разделяемом диапазоне.

*последний*<br/>
Двунаправленный итератор, указывающий позицию, следующую за последним элементом в разделяемом диапазоне.

*Зап.*<br/>
Определенный пользователем объект функции предиката, задающий условие, которое должно удовлетворяться, чтобы элемент был классифицирован. Предикат принимает один аргумент и возвращает значение **true** или **false**.

### <a name="return-value"></a>Возвращаемое значение

Двунаправленный итератор указывает позицию первого элемента в диапазоне, не соответствующего условию предиката.

### <a name="remarks"></a>Примечания

Указанный диапазон должен быть допустимым. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Элементы *a* и *b* эквивалентны, но не обязательно равны, если и *Pr* (*a*, *b*) имеет значение false, и *Pr* (*b*, *a*) имеет значение false, где *Pr* — это предикат, заданный в параметре. `partition` Алгоритм нестабилен и не гарантирует, что относительный порядок эквивалентных элементов будет сохранен. Алгоритм `stable_ partition` сохраняет этот исходный порядок.

Отношение сложности линейное: существует (`last` - `first`) приложений *comp* и не более (`last` - `first`) / 2 перестановок.

### <a name="example"></a>Пример

```cpp
// alg_partition.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <iostream>

bool greater5 ( int value ) {
   return value > 5;
}

int main() {
   using namespace std;
   vector <int> v1, v2;
   vector <int>::iterator Iter1, Iter2;

   int i;
   for ( i = 0 ; i <= 10 ; i++ )
   {
      v1.push_back( i );
   }
   random_shuffle( v1.begin( ), v1.end( ) );

   cout << "Vector v1 is ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Partition the range with predicate greater10
   partition ( v1.begin( ), v1.end( ), greater5 );
   cout << "The partitioned set of elements in v1 is: ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;
}
```

## <a name="partition_copy"></a>  partition_copy

Копирует элементы, для которых является условие **true** в одно место назначения, и для которого задано условие **false** в другой. Эти элементы должны поступать из указанного диапазона.

```cpp
template<class InputIterator, class OutputIterator1, class OutputIterator2, class Predicate>
pair<OutputIterator1, OutputIterator2>
    partition_copy(
    InputIterator first,
    InputIterator last,
    OutputIterator1 dest1,
    OutputIterator2 dest2,
    Predicate pred);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Входной итератор, указывающий начало диапазона для проверки условия.

*последний*<br/>
Входной итератор, указывающий конец диапазона.

*dest1*<br/>
Выходной итератор, используемый для копирования элементов, возвращающих значение true, если условие, проверены с использованием *_Pred*.

*dest2*<br/>
Выходной итератор, используемый для копирования элементов, которые возвращают значение false, если условие, проверены с использованием *_Pred*.

*_Pred*<br/>
Условие для проверки. Это условие предоставляется определенным пользователем объектом функции предиката, который задает условие для проверки. Предикат принимает один аргумент и возвращает значение **true** или **false**.

### <a name="remarks"></a>Примечания

Функция шаблона копирует каждый элемент `X` в `[first,last)` для `*dest1++` Если `_Pred(X)` имеет значение true, или к `*dest2++` в противном случае. Он возвращает `pair<OutputIterator1, OutputIterator2>(dest1, dest2)`.

## <a name="partition_point"></a>  partition_point

Возвращает первый элемент, который не удовлетворяет условию, в данном диапазоне. Элементы сортируются так, чтобы те, которые соответствуют условию, располагались перед теми, что не соответствуют.

```cpp
template<class ForwardIterator, class Predicate>
ForwardIterator partition_point(
    ForwardIterator first,
    ForwardIterator last,
    Predicate comp);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
`ForwardIterator`, указывающий начало диапазона для проверки условия.

*последний*<br/>
`ForwardIterator`, указывающий конец диапазона.

*Зап.*<br/>
Условие для проверки. Оно предоставляется определенным пользователем объектом функции, задающим условие, которому должен соответствовать искомый элемент. Предикат принимает один аргумент и возвращает значение **true** или **false**.

### <a name="return-value"></a>Возвращаемое значение

Возвращает `ForwardIterator` , ссылающийся на первый элемент, который не удовлетворяет условию, проверенному с *comp*, или возвращает *последнего* если таковой не найден.

### <a name="remarks"></a>Примечания

Функция шаблона находит первый итератор `it` в `[first, last)` для которого `comp(*it)` — **false**. Последовательности должны быть упорядочены по *comp*.

## <a name="pop_heap"></a>  pop_heap

Удаляет наибольший элемент из начала кучи до позиции, следующей за последней, в диапазоне, а затем формирует новую кучу из оставшихся элементов.

```cpp
template<class RandomAccessIterator>
void pop_heap( RandomAccessIterator first, RandomAccessIterator last);

template<class RandomAccessIterator, class BinaryPredicate>
void pop_heap(RandomAccessIterator first, RandomAccessIterator last, BinaryPredicate comp);

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Итератор произвольного доступа, обращающийся к позиции первого элемента в куче.

*последний*<br/>
Итератор произвольного доступа, обращающийся к позиции, следующей за последним элементом в куче.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, задающий условие, когда один элемент меньше другого. Двоичный предикат принимает два аргумента и возвращает **true** , если условие удовлетворено, или **false** , если условие не удовлетворено.

### <a name="remarks"></a>Примечания

Алгоритм `pop_heap` представляет операцию, противоположную выполняемой алгоритмом push_heap, в которой элемент в позиции, следующей за последним элементом в диапазоне, добавляется в кучу, состоящую из предыдущих элементов в диапазоне, в том случае, когда элемент, добавляемый в кучу, больше, чем любые элементы, уже находящиеся в куче.

Кучи имеют два следующих свойства.

- Первый элемент — всегда наибольший.

- Элементы могут добавляться и удаляться в логарифмическое время.

Кучи — идеальный способ реализации очередей с приоритетами, и они используются в [классе priority_queue](../standard-library/priority-queue-class.md) адаптеров контейнеров библиотеки стандартных программ C++.

Указанный диапазон должен быть допустимым. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Диапазон, исключая только что добавленный в конце элемент, должен быть кучей.

Отношение сложности логарифмическое; требуется не более журнала (* фамилия - имя *) сравнений.

### <a name="example"></a>Пример

```cpp
// alg_pop_heap.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <functional>
#include <iostream>

int main()  {
   using namespace std;
   vector <int> v1;
   vector <int>::iterator Iter1, Iter2;

   int i;
   for ( i = 1 ; i <= 9 ; i++ )
      v1.push_back( i );

   // Make v1 a heap with default less than ordering
   random_shuffle( v1.begin( ), v1.end( ) );
   make_heap ( v1.begin( ), v1.end( ) );
   cout << "The heaped version of vector v1 is ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Add an element to the back of the heap
   v1.push_back( 10 );
   push_heap( v1.begin( ), v1.end( ) );
   cout << "The reheaped v1 with 10 added is ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Remove the largest element from the heap
   pop_heap( v1.begin( ), v1.end( ) );
   cout << "The heap v1 with 10 removed is ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl << endl;

   // Make v1 a heap with greater-than ordering with a 0 element
   make_heap ( v1.begin( ), v1.end( ), greater<int>( ) );
   v1.push_back( 0 );
   push_heap( v1.begin( ), v1.end( ), greater<int>( ) );
   cout << "The 'greater than' reheaped v1 puts the smallest "
        << "element first:\n ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Application of pop_heap to remove the smallest element
   pop_heap( v1.begin( ), v1.end( ), greater<int>( ) );
   cout << "The 'greater than' heaped v1 with the smallest element\n "
        << "removed from the heap is: ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;
}
```

## <a name="prev_permutation"></a>  prev_permutation

Изменяет порядок элементов в диапазоне, чтобы исходный порядок был заменен перестановкой "лексикографически предыдущий больший", если такая существует, где смысл термина "предыдущий" может быть задан бинарным предикатом.

```cpp
template<class BidirectionalIterator>
bool prev_permutation(
    BidirectionalIterator first,
    BidirectionalIterator last);

template<class BidirectionalIterator, class BinaryPredicate>
bool prev_permutation(
    BidirectionalIterator first,
    BidirectionalIterator last,
    BinaryPredicate comp);

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Двунаправленный итератор, указывающий позицию первого элемента в диапазоне, в котором переставляются элементы.

*последний*<br/>
Двунаправленный итератор, указывающий позицию, следующую за последним элементом в диапазоне, в котором переставляются элементы.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, задающий критерий сравнения, который должен соблюдаться идущими подряд элементами при упорядочении. Двоичный предикат принимает два аргумента и возвращает **true** , если условие удовлетворено, или **false** , если условие не удовлетворено.

### <a name="return-value"></a>Возвращаемое значение

**значение true,** Если лексикографически предыдущая перестановка существует и заменила исходный порядок в диапазоне; в противном случае **false**, в этом случае порядок преобразуется в лексикографически наибольшую перестановки.

### <a name="remarks"></a>Примечания

Указанный диапазон должен быть допустимым. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Двоичный предикат по умолчанию — "меньше чем", и элементы в диапазоне должны быть сравнимы на "меньше чем", чтобы предыдущая перестановка была задана правильно.

Отношение сложности линейное, не более (`last` -  `first`) / 2 перестановок.

### <a name="example"></a>Пример

```cpp
// alg_prev_perm.cpp
// compile with: /EHsc
#include <vector>
#include <deque>
#include <algorithm>
#include <iostream>
#include <ostream>

using namespace std;
class CInt;
ostream& operator<<( ostream& osIn, const CInt& rhs );

class CInt {
public:
   CInt( int n = 0 ) : m_nVal( n ){}
   CInt( const CInt& rhs ) : m_nVal( rhs.m_nVal ){}
   CInt&   operator=( const CInt& rhs ) {m_nVal =
   rhs.m_nVal; return *this;}
   bool operator<( const CInt& rhs ) const
      {return ( m_nVal < rhs.m_nVal );}
   friend ostream& operator<<( ostream& osIn, const CInt& rhs );

private:
   int m_nVal;
};

inline ostream& operator<<( ostream& osIn, const CInt& rhs ) {
   osIn << "CInt( " << rhs.m_nVal << " )";
   return osIn;
}

// Return whether modulus of elem1 is less than modulus of elem2
bool mod_lesser (int elem1, int elem2 ) {
   if ( elem1 < 0 )
      elem1 = - elem1;
   if ( elem2 < 0 )
      elem2 = - elem2;
   return elem1 < elem2;
};

int main() {
   // Reordering the elements of type CInt in a deque
   // using the prev_permutation algorithm
   CInt c1 = 1, c2 = 5, c3 = 10;
   bool deq1Result;
   deque<CInt> deq1, deq2, deq3;
   deque<CInt>::iterator d1_Iter;

   deq1.push_back ( c1 );
   deq1.push_back ( c2 );
   deq1.push_back ( c3 );

   cout << "The original deque of CInts is deq1 = (";
   for ( d1_Iter = deq1.begin( ); d1_Iter != --deq1.end( ); d1_Iter++ )
      cout << " " << *d1_Iter << ",";
   d1_Iter = --deq1.end( );
   cout << " " << *d1_Iter << " )." << endl;

   deq1Result = prev_permutation ( deq1.begin( ), deq1.end( ) );

   if ( deq1Result )
      cout << "The lexicographically previous permutation "
           << "exists and has \nreplaced the original "
           << "ordering of the sequence in deq1." << endl;
   else
      cout << "The lexicographically previous permutation doesn't "
           << "exist\n and the lexicographically "
           << "smallest permutation\n has replaced the "
           << "original ordering of the sequence in deq1." << endl;

   cout << "After one application of prev_permutation,\n deq1 = (";
   for ( d1_Iter = deq1.begin( ); d1_Iter != --deq1.end( ); d1_Iter++ )
      cout << " " << *d1_Iter << ",";
   d1_Iter = --deq1.end( );
   cout << " " << *d1_Iter << " )." << endl << endl;

   // Permutating vector elements with binary function mod_lesser
   vector <int> v1;
   vector <int>::iterator Iter1;

   int i;
   for ( i = -3 ; i <= 3 ; i++ )
      v1.push_back( i );

   cout << "Vector v1 is ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   prev_permutation ( v1.begin( ), v1.end( ), mod_lesser );

   cout << "After the first prev_permutation, vector v1 is:\n v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   int iii = 1;
   while ( iii <= 5 ) {
      prev_permutation ( v1.begin( ), v1.end( ), mod_lesser );
      cout << "After another prev_permutation of vector v1,\n v1 =   ( " ;
      for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ;Iter1 ++ )
         cout << *Iter1  << " ";
      cout << ")." << endl;
      iii++;
   }
}
```

```Output
The original deque of CInts is deq1 = ( CInt( 1 ), CInt( 5 ), CInt( 10 ) ).
The lexicographically previous permutation doesn't exist
and the lexicographically smallest permutation
has replaced the original ordering of the sequence in deq1.
After one application of prev_permutation,
deq1 = ( CInt( 10 ), CInt( 5 ), CInt( 1 ) ).

Vector v1 is ( -3 -2 -1 0 1 2 3 ).
After the first prev_permutation, vector v1 is:
v1 = ( -3 -2 0 3 2 1 -1 ).
After another prev_permutation of vector v1,
v1 =   ( -3 -2 0 3 -1 2 1 ).
After another prev_permutation of vector v1,
v1 =   ( -3 -2 0 3 -1 1 2 ).
After another prev_permutation of vector v1,
v1 =   ( -3 -2 0 2 3 1 -1 ).
After another prev_permutation of vector v1,
v1 =   ( -3 -2 0 2 -1 3 1 ).
After another prev_permutation of vector v1,
v1 =   ( -3 -2 0 2 -1 1 3 ).
```

## <a name="push_heap"></a>  push_heap

Добавляет элемент, находящийся в конце диапазона, в существующую кучу, состоящую из предыдущих элементов диапазона.

```cpp
template<class RandomAccessIterator>
void push_heap( RandomAccessIterator first, RandomAccessIterator last );

template<class RandomAccessIterator, class BinaryPredicate>
void push_heap( RandomAccessIterator first, RandomAccessIterator last, BinaryPredicate comp);

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Итератор произвольного доступа, обращающийся к позиции первого элемента в куче.

*последний*<br/>
Итератор произвольного доступа, обращающийся к позиции, следующей за последним элементом в диапазоне, подлежащем преобразованию в кучу.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, задающий условие, когда один элемент меньше другого. Двоичный предикат принимает два аргумента и возвращает **true** , если условие удовлетворено, или **false** , если условие не удовлетворено.

### <a name="remarks"></a>Примечания

Элемент сначала должен быть помещен обратно в конец существующей кучи; затем используется алгоритм для добавления этого элемента в существующую кучу.

Кучи имеют два следующих свойства.

- Первый элемент — всегда наибольший.

- Элементы могут добавляться и удаляться в логарифмическое время.

Кучи — идеальный способ реализации очередей с приоритетами, и они используются в [классе priority_queue](../standard-library/priority-queue-class.md) адаптеров контейнеров библиотеки стандартных программ C++.

Указанный диапазон должен быть допустимым. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Диапазон, исключая только что добавленный в конце элемент, должен быть кучей.

Отношение сложности логарифмическое; требуется не более журнала ( *фамилия - имя*) сравнений.

### <a name="example"></a>Пример

```cpp
// alg_push_heap.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <functional>
#include <iostream>

int main() {
   using namespace std;
   vector <int> v1, v2;
   vector <int>::iterator Iter1, Iter2;

   int i;
   for ( i = 1 ; i <= 9 ; i++ )
      v1.push_back( i );

   random_shuffle( v1.begin( ), v1.end( ) );

   cout << "Vector v1 is ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Make v1 a heap with default less than ordering
   make_heap ( v1.begin( ), v1.end( ) );
   cout << "The heaped version of vector v1 is ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Add an element to the heap
   v1.push_back( 10 );
   cout << "The heap v1 with 10 pushed back is ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   push_heap( v1.begin( ), v1.end( ) );
   cout << "The reheaped v1 with 10 added is ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl << endl;

   // Make v1 a heap with greater than ordering
   make_heap ( v1.begin( ), v1.end( ), greater<int>( ) );
   cout << "The greater-than heaped version of v1 is\n ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   v1.push_back(0);
   cout << "The greater-than heap v1 with 11 pushed back is\n ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   push_heap( v1.begin( ), v1.end( ), greater<int>( ) );
   cout << "The greater than reheaped v1 with 11 added is\n ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;
}
```

## <a name="random_shuffle"></a>  random_shuffle

Функция std:: random_shuffle() является устаревшим, заменены [std::shuffle](../standard-library/algorithm-functions.md#shuffle). Дополнительные сведения и пример кода см. в разделе [ \<случайных >](../standard-library/random.md) и учет Stackoverflow [почему методы std::random_shuffle удалены устарели в C ++ 14?](http://go.microsoft.com/fwlink/p/?linkid=397954).

## <a name="remove"></a>  remove

Удаляет указанное значение из заданного диапазона без нарушения порядка остальных элементов и возвращает конец нового диапазона после удаления указанного значения.

```cpp
template<class ForwardIterator, class Type>
ForwardIterator remove(ForwardIterator first, ForwardIterator last, const Type& val);

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Прямой итератор, обращающийся к положению первого элемента в диапазоне, в котором удаляются элементы.

*последний*<br/>
Прямой итератор, обращающийся к положению за последним элементом в диапазоне, в котором удаляются элементы.

*Val*<br/>
Значение, которое необходимо удалить из диапазона.

### <a name="return-value"></a>Возвращаемое значение

Прямой итератор, обращающийся к новой конечной позиции измененного диапазона сразу за последним элементом оставшейся последовательности без указанного значения.

### <a name="remarks"></a>Примечания

Указанный диапазон должен быть допустимым. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Порядок неудаляемых элементов не меняется.

Оператор `operator==` , который используется для определения равенства между элементами, должен применить отношение эквивалентности между операндами.

Отношение сложности линейное; Существуют (`last` - `first`) сравнения на равенство.

[Класс list](../standard-library/list-class.md) имеет более эффективную версию функции члена из `remove`, которая также удаляет ссылки для указателей.

### <a name="example"></a>Пример

```cpp
// alg_remove.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <iostream>

int main() {
   using namespace std;
   vector <int> v1;
   vector <int>::iterator Iter1, Iter2, new_end;

   int i;
   for ( i = 0 ; i <= 9 ; i++ )
      v1.push_back( i );

   int ii;
   for ( ii = 0 ; ii <= 3 ; ii++ )
      v1.push_back( 7 );

   random_shuffle ( v1.begin( ), v1.end( ) );
   cout << "Vector v1 is ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Remove elements with a value of 7
   new_end = remove ( v1.begin( ), v1.end( ), 7 );

   cout << "Vector v1 with value 7 removed is ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // To change the sequence size, use erase
   v1.erase (new_end, v1.end( ) );

   cout << "Vector v1 resized with value 7 removed is ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;
}
```

## <a name="remove_copy"></a>  remove_copy

Копирует элементы из исходного диапазона в диапазон назначения за исключением того, что элементы с заданным значением не копируются, не нарушая порядок остальных элементов и возвращая конец нового диапазона назначения.

```cpp
template<class InputIterator, class OutputIterator, class Type>
OutputIterator remove_copy(InputIterator first, InputIterator last, OutputIterator result, const Type& val);

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Входной итератор, указывающий на позицию первого элемента в диапазоне, в котором удаляются элементы.

*последний*<br/>
Входной итератор, указывающий на позицию, следующую за последним элементом в диапазоне, в котором удаляются элементы.

*результат*<br/>
Выходной итератор, указывающий на позицию первого элемента в диапазоне назначения, в который удаляются элементы.

*Val*<br/>
Значение, которое необходимо удалить из диапазона.

### <a name="return-value"></a>Возвращаемое значение

Прямой итератор, обращающийся к новой конечной позиции диапазона назначения, следующей за последним элементом копии оставшейся последовательности без указанного значения.

### <a name="remarks"></a>Примечания

Исходный и конечный диапазоны, на которые указывают ссылки, должны быть допустимыми. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Диапазон назначения должен иметь достаточно места для хранения оставшихся элементов, которые будут скопированы после удаления элементов с указанным значением.

Порядок неудаляемых элементов не меняется.

Оператор `operator==` , который используется для определения равенства между элементами, должен применить отношение эквивалентности между операндами.

Отношение сложности линейное; Существуют (`last` - `first`) сравнения на предмет равенства и не более (`last` - `first`) назначений.

### <a name="example"></a>Пример

```cpp
// alg_remove_copy.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <iostream>

int main() {
   using namespace std;
   vector <int> v1, v2(10);
   vector <int>::iterator Iter1, Iter2, new_end;

   int i;
   for ( i = 0 ; i <= 9 ; i++ )
      v1.push_back( i );

   int ii;
   for ( ii = 0 ; ii <= 3 ; ii++ )
      v1.push_back( 7 );

   random_shuffle (v1.begin( ), v1.end( ) );
   cout << "The original vector v1 is:     ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Remove elements with a value of 7
   new_end = remove_copy ( v1.begin( ), v1.end( ), v2.begin( ), 7 );

   cout << "Vector v1 is left unchanged as ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   cout << "Vector v2 is a copy of v1 with the value 7 removed:\n ( " ;
   for ( Iter2 = v2.begin( ) ; Iter2 != v2.end( ) ; Iter2++ )
      cout << *Iter2 << " ";
   cout << ")." << endl;
}
```

## <a name="remove_copy_if"></a>  remove_copy_if

Копирует элементы из исходного диапазона в диапазон назначения за исключением того, что элементы, соответствующие предикату, не копируются, не нарушая порядок остальных элементов и возвращая конец нового диапазона назначения.

```cpp
template<class InputIterator, class OutputIterator, class Predicate>
OutputIterator remove_copy_if(InputIterator first, InputIterator Last, OutputIterator result, Predicate pred);

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Входной итератор, указывающий на позицию первого элемента в диапазоне, в котором удаляются элементы.

*последний*<br/>
Входной итератор, указывающий на позицию, следующую за последним элементом в диапазоне, в котором удаляются элементы.

*результат*<br/>
Выходной итератор, указывающий на позицию первого элемента в диапазоне назначения, в который удаляются элементы.

*_Pred*<br/>
Унарный предикат, который должен быть удовлетворен, является значением заменяемого элемента.

### <a name="return-value"></a>Возвращаемое значение

Прямой итератор, указывающий на новую конечную позицию диапазона назначения, следующую за последним элементом копии оставшейся последовательности без элементов, удовлетворяющих предикату.

### <a name="remarks"></a>Примечания

Указанный диапазон должен быть допустимым. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Диапазон назначения должен иметь достаточно места для хранения оставшихся элементов, которые будут скопированы после удаления элементов с указанным значением.

Порядок неудаляемых элементов не меняется.

Оператор `operator==` , который используется для определения равенства между элементами, должен применить отношение эквивалентности между операндами.

Отношение сложности линейное: существует (`last` - `first`) сравнения на предмет равенства и не более (`last` - `first`) назначений.

Сведения о действии этих функций см. в разделе [Checked Iterators](../standard-library/checked-iterators.md).

### <a name="example"></a>Пример

```cpp
// alg_remove_copy_if.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <iostream>

bool greater6 ( int value ) {
   return value > 6;
}

int main() {
   using namespace std;
   vector <int> v1, v2(10);
   vector <int>::iterator Iter1, Iter2, new_end;

   int i;
   for ( i = 0 ; i <= 9 ; i++ )
      v1.push_back( i );

   int ii;
   for ( ii = 0 ; ii <= 3 ; ii++ )
      v1.push_back( 7 );

   random_shuffle ( v1.begin( ), v1.end( ) );
   cout << "The original vector v1 is:      ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Remove elements with a value greater than 6
   new_end = remove_copy_if ( v1.begin( ), v1.end( ),
      v2.begin( ), greater6 );

   cout << "After the appliation of remove_copy_if to v1,\n "
        << "vector v1 is left unchanged as ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   cout << "Vector v2 is a copy of v1 with values greater "
        << "than 6 removed:\n ( " ;
   for ( Iter2 = v2.begin( ) ; Iter2 != new_end ; Iter2++ )
      cout << *Iter2 << " ";
   cout << ")." << endl;
}
```

## <a name="remove_if"></a>  remove_if

Удаляет элементы, соответствующие предикату, из заданного диапазона без нарушения порядка остальных элементов и возвращает конец нового диапазона после удаления указанного значения.

```cpp
template<class ForwardIterator, class Predicate>
ForwardIterator remove_if(
    ForwardIterator first,
    ForwardIterator last,
    Predicate pred);

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Прямой итератор, указывающий на позицию первого элемента в диапазоне, из которого удаляются элементы.

*последний*<br/>
Прямой итератор, указывающий на позицию, следующую за последним элементом в диапазоне, из которого удаляются элементы.

*_Pred*<br/>
Унарный предикат, который должен быть удовлетворен, является значением заменяемого элемента.

### <a name="return-value"></a>Возвращаемое значение

Прямой итератор, обращающийся к новой конечной позиции измененного диапазона сразу за последним элементом оставшейся последовательности без указанного значения.

### <a name="remarks"></a>Примечания

Указанный диапазон должен быть допустимым. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Порядок неудаляемых элементов не меняется.

Оператор `operator==` , который используется для определения равенства между элементами, должен применить отношение эквивалентности между операндами.

Отношение сложности линейное: существует (`last` - `first`) сравнения на равенство.

Класс list содержит более эффективную версию функции-члена remove, которая удаляет ссылки для указателей.

### <a name="example"></a>Пример

```cpp
// alg_remove_if.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <iostream>

bool greater6 ( int value ) {
   return value > 6;
}

int main() {
   using namespace std;
   vector <int> v1, v2;
   vector <int>::iterator Iter1, Iter2, new_end;

   int i;
   for ( i = 0 ; i <= 9 ; i++ )
      v1.push_back( i );

   int ii;
   for ( ii = 0 ; ii <= 3 ; ii++ )
      v1.push_back( 7 );

   random_shuffle ( v1.begin( ), v1.end( ) );
   cout << "Vector v1 is ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Remove elements satisfying predicate greater6
   new_end = remove_if (v1.begin( ), v1.end( ), greater6 );

   cout << "Vector v1 with elements satisfying greater6 removed is\n ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // To change the sequence size, use erase
   v1.erase (new_end, v1.end( ) );

   cout << "Vector v1 resized elements satisfying greater6 removed is\n ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;
}
```

## <a name="replace"></a>  replace

Проверяет каждый элемент в диапазоне и заменяет его, если он соответствует заданному значению.

```cpp
template<class ForwardIterator, class Type>
void replace(
    ForwardIterator first,
    ForwardIterator last,
    const Type& oldVal,
    const Type& newVal);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Прямой итератор, указывающий на позицию первого элемента в диапазоне, в котором заменяются элементы.

*последний*<br/>
Прямой итератор, указывающий на позицию, следующую за последним элементом в диапазоне, в котором заменяются элементы.

*_OldVal*<br/>
Старое значение заменяемых элементов.

*_NewVal*<br/>
Новое значение, присваиваемое элементам со старым значением.

### <a name="remarks"></a>Примечания

Указанный диапазон должен быть допустимым. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Порядок незаменяемых элементов не меняется.

Оператор `operator==` , который используется для определения равенства между элементами, должен применить отношение эквивалентности между операндами.

Отношение сложности линейное; Существуют (`last` - `first`) сравнения на предмет равенства и не более (`last` - `first`) присвоений новых значений.

### <a name="example"></a>Пример

```cpp
// alg_replace.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <iostream>

int main() {
   using namespace std;
   vector <int> v1;
   vector <int>::iterator Iter1;

   int i;
   for ( i = 0 ; i <= 9 ; i++ )
      v1.push_back( i );

   int ii;
   for ( ii = 0 ; ii <= 3 ; ii++ )
      v1.push_back( 7 );

   random_shuffle (v1.begin( ), v1.end( ) );
   cout << "The original vector v1 is:\n ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Replace elements with a value of 7 with a value of 700
   replace (v1.begin( ), v1.end( ), 7 , 700);

   cout << "The vector v1 with a value 700 replacing that of 7 is:\n ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;
}
```

## <a name="replace_copy"></a>  replace_copy

Проверяет каждый элемент в исходном диапазоне и заменяет его, если он соответствует заданному значению, одновременно копируя результат в новый диапазон назначения.

```cpp
template<class InputIterator, class OutputIterator, class Type>
OutputIterator replace_copy(
    InputIterator first,
    InputIterator last,
    OutputIterator result,
    const Type& oldVal,
    const Type& newVal);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Входной итератор, указывающий на позицию первого элемента в диапазоне, в котором заменяются элементы.

*последний*<br/>
Входной итератор, указывающий на позицию, следующую за последним элементом в диапазоне, в котором заменяются элементы.

*результат*<br/>
Выходной итератор, указывающий на первый элемент в диапазоне назначения, в который копируется измененная последовательность элементов.

*_OldVal*<br/>
Старое значение заменяемых элементов.

*_NewVal*<br/>
Новое значение, присваиваемое элементам со старым значением.

### <a name="return-value"></a>Возвращаемое значение

Выходной итератор, указывающий на позицию, следующую за последним элементом в диапазоне назначения, в который копируется измененная последовательность элементов.

### <a name="remarks"></a>Примечания

Исходный и конечный диапазоны, на которые указывают ссылки, не должны перекрываться и должны быть допустимыми. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Порядок незаменяемых элементов не меняется.

Оператор `operator==` , который используется для определения равенства между элементами, должен применить отношение эквивалентности между операндами.

Отношение сложности линейное: существует (`last` - `first`) сравнения на предмет равенства и не более (`last` - `first`) присвоений новых значений.

### <a name="example"></a>Пример

```cpp
// alg_replace_copy.cpp
// compile with: /EHsc
#include <vector>
#include <list>
#include <algorithm>
#include <iostream>

int main() {
   using namespace std;
   vector <int> v1;
   list <int> L1 (15);
   vector <int>::iterator Iter1;
   list <int>::iterator L_Iter1;

   int i;
   for ( i = 0 ; i <= 9 ; i++ )
      v1.push_back( i );

   int ii;
   for ( ii = 0 ; ii <= 3 ; ii++ )
      v1.push_back( 7 );

   random_shuffle ( v1.begin( ), v1.end( ) );

   int iii;
   for ( iii = 0 ; iii <= 15 ; iii++ )
      v1.push_back( 1 );

   cout << "The original vector v1 is:\n ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Replace elements in one part of a vector with a value of 7
   // with a value of 70 and copy into another part of the vector
   replace_copy ( v1.begin( ), v1.begin( ) + 14,v1.end( ) -15, 7 , 70);

   cout << "The vector v1 with a value 70 replacing that of 7 is:\n ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Replace elements in a vector with a value of 70
   // with a value of 1 and copy into a list
   replace_copy ( v1.begin( ), v1.begin( ) + 14,L1.begin( ), 7 , 1);

   cout << "The list copy L1 of v1 with the value 0 replacing "
        << "that of 7 is:\n ( " ;
   for ( L_Iter1 = L1.begin( ) ; L_Iter1 != L1.end( ) ; L_Iter1++ )
      cout << *L_Iter1 << " ";
   cout << ")." << endl;
}
```

## <a name="replace_copy_if"></a>  replace_copy_if

Проверяет каждый элемент в исходном диапазоне и заменяет его, если он соответствует заданному предикату, одновременно копируя результат в новый диапазон назначения.

```cpp
template<class InputIterator, class OutputIterator, class Predicate, class Type>
OutputIterator replace_copy_if(
    InputIterator first,
    InputIterator last,
    OutputIterator result,
    Predicate pred,
    const Type& val);

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Входной итератор, указывающий на позицию первого элемента в диапазоне, в котором заменяются элементы.

*последний*<br/>
Входной итератор, указывающий на позицию, следующую за последним элементом в диапазоне, в котором заменяются элементы.

*результат*<br/>
Выходной итератор, указывающий на позицию первого элемента в диапазоне назначения, в который копируются элементы.

*_Pred*<br/>
Унарный предикат, который должен быть удовлетворен, является значением заменяемого элемента.

*Val*<br/>
Новое значение, присваиваемое элементам, старые значения которых удовлетворяют предикату.

### <a name="return-value"></a>Возвращаемое значение

Выходной итератор, указывающий на позицию, следующую за последним элементом в диапазоне назначения, в который копируется измененная последовательность элементов.

### <a name="remarks"></a>Примечания

Исходный и конечный диапазоны, на которые указывают ссылки, не должны перекрываться и должны быть допустимыми. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Порядок незаменяемых элементов не меняется.

Оператор `operator==` , который используется для определения равенства между элементами, должен применить отношение эквивалентности между операндами.

Отношение сложности линейное; Существуют (`last` - `first`) сравнения на предмет равенства и не более (`last` - `first`) присвоений новых значений.

### <a name="example"></a>Пример

```cpp
// alg_replace_copy_if.cpp
// compile with: /EHsc
#include <vector>
#include <list>
#include <algorithm>
#include <iostream>

bool greater6 ( int value ) {
   return value > 6;
}

int main() {
   using namespace std;
   vector <int> v1;
   list <int> L1 (13);
   vector <int>::iterator Iter1;
   list <int>::iterator L_Iter1;

   int i;
   for ( i = 0 ; i <= 9 ; i++ )
      v1.push_back( i );

   int ii;
   for ( ii = 0 ; ii <= 3 ; ii++ )
      v1.push_back( 7 );

   random_shuffle ( v1.begin( ), v1.end( ) );

   int iii;
   for ( iii = 0 ; iii <= 13 ; iii++ )
      v1.push_back( 1 );

   cout << "The original vector v1 is:\n ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Replace elements with a value of 7 in the 1st half of a vector
   // with a value of 70 and copy it into the 2nd half of the vector
   replace_copy_if ( v1.begin( ), v1.begin( ) + 14,v1.end( ) -14,
      greater6 , 70);

   cout << "The vector v1 with values of 70 replacing those greater"
        << "\n than 6 in the 1st half & copied into the 2nd half is:\n ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Replace elements in a vector with a value of 70
   // with a value of 1 and copy into a list
   replace_copy_if ( v1.begin( ), v1.begin( ) + 13,L1.begin( ),
      greater6 , -1 );

   cout << "A list copy of vector v1 with the value -1\n replacing "
        << "those greater than 6 is:\n ( " ;
   for ( L_Iter1 = L1.begin( ) ; L_Iter1 != L1.end( ) ; L_Iter1++ )
      cout << *L_Iter1 << " ";
   cout << ")." << endl;
}
```

## <a name="replace_if"></a>  replace_if

Проверяет каждый элемент в диапазоне и заменяет его, если он соответствует заданному предикату.

```cpp
template<class ForwardIterator, class Predicate, class Type>
void replace_if(
    ForwardIterator first,
    ForwardIterator last,
    Predicate pred,
    const Type& val);

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Прямой итератор, указывающий на позицию первого элемента в диапазоне, в котором заменяются элементы.

*последний*<br/>
Итератор, указывающий на позицию, следующую за последним элементом в диапазоне, в котором заменяются элементы.

*_Pred*<br/>
Унарный предикат, который должен быть удовлетворен, является значением заменяемого элемента.

*Val*<br/>
Новое значение, присваиваемое элементам, старые значения которых удовлетворяют предикату.

### <a name="remarks"></a>Примечания

Указанный диапазон должен быть допустимым. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Порядок незаменяемых элементов не меняется.

Алгоритм `replace_if` представляет собой обобщение алгоритма `replace`, позволяя любой предикат указан, вместо равенства указанной константе.

Оператор `operator==` , который используется для определения равенства между элементами, должен применить отношение эквивалентности между операндами.

Отношение сложности линейное: существует (`last` - `first`) сравнения на предмет равенства и не более (`last` - `first`) присвоений новых значений.

### <a name="example"></a>Пример

```cpp
// alg_replace_if.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <iostream>

bool greater6 ( int value ) {
   return value > 6;
}

int main() {
   using namespace std;
   vector <int> v1;
   vector <int>::iterator Iter1;

   int i;
   for ( i = 0 ; i <= 9 ; i++ )
      v1.push_back( i );

   int ii;
   for ( ii = 0 ; ii <= 3 ; ii++ )
      v1.push_back( 7 );

   random_shuffle ( v1.begin( ), v1.end( ) );
   cout << "The original vector v1 is:\n ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Replace elements satisfying the predicate greater6
   // with a value of 70
   replace_if ( v1.begin( ), v1.end( ), greater6 , 70);

   cout << "The vector v1 with a value 70 replacing those\n "
        << "elements satisfying the greater6 predicate is:\n ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;
}
```

## <a name="reverse"></a>  reverse

Изменяет порядок элементов в диапазоне на обратный.

```cpp
template<class BidirectionalIterator>
void reverse(BidirectionalIterator first, BidirectionalIterator last);

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Двунаправленный итератор, указывающий на позицию первого элемента в диапазоне, в котором переставляются элементы.

*последний*<br/>
Двунаправленный итератор, указывающий на позицию, следующую за последним элементом в диапазоне, в котором переставляются элементы.

### <a name="remarks"></a>Примечания

Указанный диапазон должен быть допустимым. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

### <a name="example"></a>Пример

```cpp
// alg_reverse.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <iostream>

int main() {
   using namespace std;
   vector <int> v1;
   vector <int>::iterator Iter1;

   int i;
   for ( i = 0 ; i <= 9 ; i++ )
   {
      v1.push_back( i );
   }

   cout << "The original vector v1 is:\n ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Reverse the elements in the vector
   reverse (v1.begin( ), v1.end( ) );

   cout << "The modified vector v1 with values reversed is:\n ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;
}
```

```Output
The original vector v1 is:
( 0 1 2 3 4 5 6 7 8 9 ).
The modified vector v1 with values reversed is:
( 9 8 7 6 5 4 3 2 1 0 ).
```

## <a name="reverse_copy"></a>  reverse_copy

Изменяет порядок элементов в исходном диапазоне на обратный, одновременно копируя их в диапазон назначения

```cpp
template<class BidirectionalIterator, class OutputIterator>
OutputIterator reverse_copy(
    BidirectionalIterator first,
    BidirectionalIterator Last,
    OutputIterator result);

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Двунаправленный итератор, указывающий на позицию первого элемента в исходном диапазоне, в котором переставляются элементы.

*последний*<br/>
Двунаправленный итератор, указывающий на позицию, следующую за последним элементом в исходном диапазоне, в котором переставляются элементы.

*результат*<br/>
Выходной итератор, указывающий на позицию первого элемента в диапазоне назначения, в который копируются элементы.

### <a name="return-value"></a>Возвращаемое значение

Выходной итератор, указывающий на позицию, следующую за последним элементом в диапазоне назначения, в который копируется измененная последовательность элементов.

### <a name="remarks"></a>Примечания

Исходный и конечный диапазоны, на которые указывают ссылки, должны быть допустимыми. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

### <a name="example"></a>Пример

```cpp
// alg_reverse_copy.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <iostream>

int main() {
   using namespace std;
   vector <int> v1, v2( 10 );
   vector <int>::iterator Iter1, Iter2;

   int i;
   for ( i = 0 ; i <= 9 ; i++ )
   {
      v1.push_back( i );
   }

   cout << "The original vector v1 is:\n ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Reverse the elements in the vector
   reverse_copy (v1.begin( ), v1.end( ), v2.begin( ) );

   cout << "The copy v2 of the reversed vector v1 is:\n ( " ;
   for ( Iter2 = v2.begin( ) ; Iter2 != v2.end( ) ; Iter2++ )
      cout << *Iter2 << " ";
   cout << ")." << endl;

   cout << "The original vector v1 remains unmodified as:\n ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;
}
```

## <a name="rotate"></a>  rotate

Меняет местами элементы в двух соседних диапазонах.

```cpp
template<class ForwardIterator>
void rotate(
    ForwardIterator first,
    ForwardIterator middle,
    ForwardIterator last);

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Прямой итератор, указывающий на позицию первого элемента в диапазоне для изменения места.

*среднего*<br/>
Прямой итератор, определяющий границу в диапазоне и указывающий на позицию первого элемента во второй части диапазона, элементы которого должны поменяться местами с элементами в первой части диапазона.

*последний*<br/>
Прямой итератор, указывающий на позицию, следующую за последним элементом в диапазоне для изменения места.

### <a name="remarks"></a>Примечания

Указанные диапазоны должны быть допустимыми. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Отношение сложности линейное с не более (`last` - `first`) меняет местами.

### <a name="example"></a>Пример

```cpp
// alg_rotate.cpp
// compile with: /EHsc
#include <vector>
#include <deque>
#include <algorithm>
#include <iostream>

int main() {
   using namespace std;
   vector <int> v1;
   deque <int> d1;
   vector <int>::iterator v1Iter1;
   deque<int>::iterator d1Iter1;

   int i;
   for ( i = -3 ; i <= 5 ; i++ )
   {
      v1.push_back( i );
   }

   int ii;
   for ( ii =0 ; ii <= 5 ; ii++ )
   {
      d1.push_back( ii );
   }

   cout << "Vector v1 is ( " ;
   for ( v1Iter1 = v1.begin( ) ; v1Iter1 != v1.end( ) ;v1Iter1 ++ )
      cout << *v1Iter1  << " ";
   cout << ")." << endl;

   rotate ( v1.begin( ), v1.begin( ) + 3 , v1.end( ) );
   cout << "After rotating, vector v1 is ( " ;
   for ( v1Iter1 = v1.begin( ) ; v1Iter1 != v1.end( ) ;v1Iter1 ++ )
      cout << *v1Iter1  << " ";
   cout << ")." << endl;

   cout << "The original deque d1 is ( " ;
   for ( d1Iter1 = d1.begin( ) ; d1Iter1 != d1.end( ) ;d1Iter1 ++ )
      cout << *d1Iter1  << " ";
   cout << ")." << endl;

   int iii = 1;
   while ( iii <= d1.end( ) - d1.begin( ) ) {
      rotate ( d1.begin( ), d1.begin( ) + 1 , d1.end( ) );
      cout << "After the rotation of a single deque element to the back,\n d1 is   ( " ;
      for ( d1Iter1 = d1.begin( ) ; d1Iter1 != d1.end( ) ;d1Iter1 ++ )
         cout << *d1Iter1  << " ";
      cout << ")." << endl;
      iii++;
   }
}
```

```Output
Vector v1 is ( -3 -2 -1 0 1 2 3 4 5 ).
After rotating, vector v1 is ( 0 1 2 3 4 5 -3 -2 -1 ).
The original deque d1 is ( 0 1 2 3 4 5 ).
After the rotation of a single deque element to the back,
d1 is   ( 1 2 3 4 5 0 ).
After the rotation of a single deque element to the back,
d1 is   ( 2 3 4 5 0 1 ).
After the rotation of a single deque element to the back,
d1 is   ( 3 4 5 0 1 2 ).
After the rotation of a single deque element to the back,
d1 is   ( 4 5 0 1 2 3 ).
After the rotation of a single deque element to the back,
d1 is   ( 5 0 1 2 3 4 ).
After the rotation of a single deque element to the back,
d1 is   ( 0 1 2 3 4 5 ).
```

## <a name="rotate_copy"></a>  rotate_copy

Меняет местами элементы в двух соседних диапазонах в пределах исходного диапазона и копирует результат в диапазон назначения.

```cpp
template<class ForwardIterator, class OutputIterator>
OutputIterator rotate_copy(
    ForwardIterator first,
    ForwardIterator middle,
    ForwardIterator last,
    OutputIterator result );

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Прямой итератор, указывающий на позицию первого элемента в диапазоне для изменения места.

*среднего*<br/>
Прямой итератор, определяющий границу в диапазоне и указывающий на позицию первого элемента во второй части диапазона, элементы которого должны поменяться местами с элементами в первой части диапазона.

_ *Последнего* прямой итератор, указывающий позицию, следующую за последним элементом в диапазоне для изменения места.

*результат*<br/>
Итератор вывода указывает на позицию первого элемента в диапазоне назначения.

### <a name="return-value"></a>Возвращаемое значение

Выходной итератор, указывающий на позицию, следующую за последним элементом в диапазоне назначения.

### <a name="remarks"></a>Примечания

Указанные диапазоны должны быть допустимыми. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Отношение сложности линейное с не более (`last` - `first`) меняет местами.

### <a name="example"></a>Пример

```cpp
// alg_rotate_copy.cpp
// compile with: /EHsc
#include <vector>
#include <deque>
#include <algorithm>
#include <iostream>

int main() {
   using namespace std;
   vector <int> v1 , v2 ( 9 );
   deque <int> d1 , d2 ( 6 );
   vector <int>::iterator v1Iter , v2Iter;
   deque<int>::iterator d1Iter , d2Iter;

   int i;
   for ( i = -3 ; i <= 5 ; i++ )
      v1.push_back( i );

   int ii;
   for ( ii =0 ; ii <= 5 ; ii++ )
      d1.push_back( ii );

   cout << "Vector v1 is ( " ;
   for ( v1Iter = v1.begin( ) ; v1Iter != v1.end( ) ;v1Iter ++ )
      cout << *v1Iter  << " ";
   cout << ")." << endl;

   rotate_copy ( v1.begin( ), v1.begin( ) + 3 , v1.end( ), v2.begin( ) );
   cout << "After rotating, the vector v1 remains unchanged as:\n v1 = ( " ;
   for ( v1Iter = v1.begin( ) ; v1Iter != v1.end( ) ;v1Iter ++ )
      cout << *v1Iter  << " ";
   cout << ")." << endl;

   cout << "After rotating, the copy of vector v1 in v2 is:\n v2 = ( " ;
   for ( v2Iter = v2.begin( ) ; v2Iter != v2.end( ) ;v2Iter ++ )
      cout << *v2Iter  << " ";
   cout << ")." << endl;

   cout << "The original deque d1 is ( " ;
   for ( d1Iter = d1.begin( ) ; d1Iter != d1.end( ) ;d1Iter ++ )
      cout << *d1Iter  << " ";
   cout << ")." << endl;

   int iii = 1;
   while ( iii <= d1.end( ) - d1.begin( ) )
   {
      rotate_copy ( d1.begin( ), d1.begin( ) + iii , d1.end( ), d2.begin( ) );
      cout << "After the rotation of a single deque element to the back,\n d2 is   ( " ;
      for ( d2Iter = d2.begin( ) ; d2Iter != d2.end( ) ;d2Iter ++ )
         cout << *d2Iter  << " ";
      cout << ")." << endl;
      iii++;
   }
}
```

## <a name="search"></a>  search

Выполняет поиск первого вхождения последовательности в целевой диапазон, элементы которого равны указанным в заданной последовательности элементов или элементы которого равноценны в смысле, заданным бинарным предикатом, элементам в заданной последовательности.

```cpp
template<class ForwardIterator1, class ForwardIterator2>
ForwardIterator1 search(
    ForwardIterator1 first1,
    ForwardIterator1 last1,
    ForwardIterator2 first2,
    ForwardIterator2 last2);

template<class ForwardIterator1, class ForwardIterator2, class Predicate>
ForwardIterator1 search(
    ForwardIterator1 first1,
    ForwardIterator1 last1,
    ForwardIterator2 first2,
    ForwardIterator2 last2
    Predicate comp);

```

### <a name="parameters"></a>Параметры

*first1*<br/>
Прямой итератор, адресующий положение первого элемента в диапазоне для поиска.

*last1*<br/>
Прямой итератор, адресующий положение на единицу после последнего элемента в диапазоне для поиска.

*first2*<br/>
Прямой итератор, адресующий положение первого элемента в диапазоне для сравнения.

*last2*<br/>
Прямой итератор, адресующий положение на единицу после последнего элемента в диапазоне для сравнения.

*Зап.*<br/>
Заданный пользователем объект функции предиката, определяющий условие, которое должно выполняться, чтобы два элемента считались эквивалентными друг другу. Двоичный предикат принимает два аргумента и возвращает **true** , если условие удовлетворено, или **false** , если условие не удовлетворено.

### <a name="return-value"></a>Возвращаемое значение

Прямой итератор, адресующий положение первого элемента первой последовательности, совпадающей с определенной последовательностью или эквивалентной согласно условию, заданному двоичным предикатом.

### <a name="remarks"></a>Примечания

`operator==`, используемый для определения совпадения между элементом и указанным значением, должен применять отношение эквивалентности между своими операндами.

Диапазоны, на которые указывают ссылки, должны быть допустимыми; все указатели должны поддерживать сброс ссылок; в каждой последовательности должна быть возможность достижения последнего положения с первого путем приращения.

Средняя сложность — линейная относительно размера диапазона для поиска; и в наихудшем случае сложность также линейная относительно размера искомой последовательности.

### <a name="example"></a>Пример

```cpp
// alg_search.cpp
// compile with: /EHsc
#include <vector>
#include <list>
#include <algorithm>
#include <iostream>

// Return whether second element is twice the first
bool twice (int elem1, int elem2 )
{
   return 2 * elem1 == elem2;
}

int main() {
   using namespace std;
   vector <int> v1, v2;
   list <int> L1;
   vector <int>::iterator Iter1, Iter2;
   list <int>::iterator L1_Iter, L1_inIter;

   int i;
   for ( i = 0 ; i <= 5 ; i++ )
   {
      v1.push_back( 5 * i );
   }
   for ( i = 0 ; i <= 5 ; i++ )
   {
      v1.push_back( 5 * i );
   }

   int ii;
   for ( ii = 4 ; ii <= 5 ; ii++ )
   {
      L1.push_back( 5 * ii );
   }

   int iii;
   for ( iii = 2 ; iii <= 4 ; iii++ )
   {
      v2.push_back( 10 * iii );
   }

   cout << "Vector v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;

   cout << "List L1 = ( " ;
   for ( L1_Iter = L1.begin( ) ; L1_Iter!= L1.end( ) ; L1_Iter++ )
      cout << *L1_Iter << " ";
   cout << ")" << endl;

   cout << "Vector v2 = ( " ;
   for ( Iter2 = v2.begin( ) ; Iter2 != v2.end( ) ; Iter2++ )
      cout << *Iter2 << " ";
      cout << ")" << endl;

   // Searching v1 for first match to L1 under identity
   vector <int>::iterator result1;
   result1 = search (v1.begin( ), v1.end( ), L1.begin( ), L1.end( ) );

   if ( result1 == v1.end( ) )
      cout << "There is no match of L1 in v1."
           << endl;
   else
      cout << "There is at least one match of L1 in v1"
           << "\n and the first one begins at "
           << "position "<< result1 - v1.begin( ) << "." << endl;

   // Searching v1 for a match to L1 under the binary predicate twice
   vector <int>::iterator result2;
   result2 = search  (v1.begin( ), v1.end( ), v2.begin( ), v2.end( ), twice );

   if ( result2 == v1.end( ) )
      cout << "There is no match of L1 in v1."
           << endl;
   else
      cout << "There is a sequence of elements in v1 that "
           << "are equivalent\n to those in v2 under the binary "
           << "predicate twice\n and the first one begins at position "
           << result2 - v1.begin( ) << "." << endl;
}
```

```Output
Vector v1 = ( 0 5 10 15 20 25 0 5 10 15 20 25 )
List L1 = ( 20 25 )
Vector v2 = ( 20 30 40 )
There is at least one match of L1 in v1
and the first one begins at position 4.
There is a sequence of elements in v1 that are equivalent
to those in v2 under the binary predicate twice
and the first one begins at position 2.
```

## <a name="search_n"></a>  search_n

Выполняет поиск первой подпоследовательности в диапазоне заданного числа элементов, имеющих определенное значение или связанных с этим значением отношением, указанным бинарным предикатом.

```cpp
template<class ForwardIterator1, class Diff2, class Type>
ForwardIterator1 search_n(
    ForwardIterator1 first1,
    ForwardIterator1 last1,
    Diff2 count,
    const Type& val);

template<class ForwardIterator1, class Diff2, class Type, class BinaryPredicate>
ForwardIterator1 search_n(
    ForwardIterator1 first1,
    ForwardIterator1 last1,
    Diff2 count,
    const Type& val,
    BinaryPredicate comp);

```

### <a name="parameters"></a>Параметры

*first1*<br/>
Прямой итератор, адресующий положение первого элемента в диапазоне для поиска.

*last1*<br/>
Прямой итератор, адресующий положение на единицу после последнего элемента в диапазоне для поиска.

*count*<br/>
Размер искомой последовательности.

*Val*<br/>
Значение элементов в искомой последовательности.

*Зап.*<br/>
Заданный пользователем объект функции предиката, определяющий условие, которое должно выполняться, чтобы два элемента считались эквивалентными друг другу. Двоичный предикат принимает два аргумента и возвращает **true** , если условие удовлетворено, или **false** , если условие не удовлетворено.

### <a name="return-value"></a>Возвращаемое значение

Прямой итератор, адресующий положение первого элемента первой последовательности, совпадающей с определенной последовательностью или эквивалентной согласно условию, заданному двоичным предикатом.

### <a name="remarks"></a>Примечания

`operator==`, используемый для определения совпадения между элементом и указанным значением, должен применять отношение эквивалентности между своими операндами.

Указанный диапазон должен быть допустимым. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Сложность линейная по отношению к размеру диапазона поиска.

### <a name="example"></a>Пример

```cpp
// alg_search_n.cpp
// compile with: /EHsc
#include <vector>
#include <list>
#include <algorithm>
#include <iostream>

// Return whether second element is 1/2 of the first
bool one_half ( int elem1, int elem2 )
{
   return elem1 == 2 * elem2;
}

int main()
{
   using namespace std;
   vector <int> v1, v2;
   vector <int>::iterator Iter1;

   int i;
   for ( i = 0 ; i <= 5 ; i++ )
   {
      v1.push_back( 5 * i );
   }

   for ( i = 0 ; i <= 2 ; i++ )
   {
      v1.push_back( 5  );
   }

   for ( i = 0 ; i <= 5 ; i++ )
   {
      v1.push_back( 5 * i );
   }

   for ( i = 0 ; i <= 2 ; i++ )
   {
      v1.push_back( 10  );
   }

   cout << "Vector v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;

   // Searching v1 for first match to (5 5 5) under identity
   vector <int>::iterator result1;
   result1 = search_n ( v1.begin( ), v1.end( ), 3, 5 );

   if ( result1 == v1.end( ) )
      cout << "There is no match for a sequence ( 5 5 5 ) in v1."
           << endl;
   else
      cout << "There is at least one match of a sequence ( 5 5 5 )"
           << "\n in v1 and the first one begins at "
           << "position "<< result1 - v1.begin( ) << "." << endl;

   // Searching v1 for first match to (5 5 5) under one_half
   vector <int>::iterator result2;
   result2 = search_n (v1.begin( ), v1.end( ), 3, 5, one_half );

   if ( result2 == v1.end( ) )
      cout << "There is no match for a sequence ( 5 5 5 ) in v1"
           << " under the equivalence predicate one_half." << endl;
   else
      cout << "There is a match of a sequence ( 5 5 5 ) "
           << "under the equivalence\n predicate one_half "
           << "in v1 and the first one begins at "
           << "position "<< result2 - v1.begin( ) << "." << endl;
}
```

```Output
Vector v1 = ( 0 5 10 15 20 25 5 5 5 0 5 10 15 20 25 10 10 10 )
There is at least one match of a sequence ( 5 5 5 )
in v1 and the first one begins at position 6.
There is a match of a sequence ( 5 5 5 ) under the equivalence
predicate one_half in v1 and the first one begins at position 15.
```

## <a name="set_difference"></a>  set_difference

Объединяет все элементы, принадлежащие одному отсортированному исходному диапазону, но не второму отсортированному исходному диапазону, в один отсортированный диапазон назначения, где критерий упорядочивания может быть указан бинарным предикатом.

```cpp
template<class InputIterator1, class InputIterator2, class OutputIterator>
OutputIterator set_difference(
    InputIterator1  first1,
    InputIterator1  last1,
    InputIterator2  first2,
    InputIterator2  last2,
    OutputIterator  result );

template<class InputIterator1, class InputIterator2, class OutputIterator, class BinaryPredicate>
OutputIterator set_difference(
    InputIterator1  first1,
    InputIterator1  last1,
    InputIterator2  first2,
    InputIterator2  last2,
    OutputIterator  result,
    BinaryPredicate  comp );
```

### <a name="parameters"></a>Параметры

*first1*<br/>
Входной итератор, указывающий на позицию первого элемента в первом из двух упорядоченных исходных диапазонов, которые следует объединить и упорядочить в один диапазон, представляющий разность двух исходных диапазонов.

*last1*<br/>
Входной итератор, указывающий на позицию, следующую за последним элементом в первом из двух упорядоченных исходных диапазонов, которые следует объединить и упорядочить в один диапазон, представляющий разность двух исходных диапазонов.

*first2*<br/>
Входной итератор, указывающий на позицию первого элемента во втором из двух последовательных упорядоченных исходных диапазонов, которые следует объединить и упорядочить в один диапазон, представляющий разность двух исходных диапазонов.

*last2*<br/>
Входной итератор, указывающий на позицию, следующую за последним элементом во втором из двух последовательных упорядоченных исходных диапазонов, которые следует объединить и упорядочить в один диапазон, представляющий разность двух исходных диапазонов.

*результат*<br/>
Выходной итератор, указывающий на позицию первого элемента в диапазоне назначения, в котором два исходных диапазона следует объединить в один упорядоченный диапазон, представляющий разность двух исходных диапазонов.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, определяющий условие, когда один элемент больше другого. Бинарный предикат принимает два аргумента и должен возвращать значение **true** , когда первый элемент меньше второго элемента, и значение **false** в противном случае.

### <a name="return-value"></a>Возвращаемое значение

Выходной итератор, указывающий на позицию, следующую за последним элементом в упорядоченном диапазоне назначения, представляющем разность двух исходных диапазонов.

### <a name="remarks"></a>Примечания

Упорядоченные исходные диапазоны, на которые указывают ссылки, должны быть допустимыми. Все указатели должны поддерживать отмену ссылок. В каждой последовательности должна быть возможность достижения последней позиции с первой путем приращения.

Диапазон назначения не должен перекрывать исходные диапазоны и должен быть достаточно большим, чтобы содержать первый исходный диапазон.

Каждый упорядоченный исходный диапазон должны быть упорядочен в качестве предусловия для применения алгоритма `set_difference` в соответствии с теми же правилами, чтобы использоваться алгоритмом для упорядочения объединенных диапазонов.

Операция стабильна, так как в диапазоне назначения сохраняется относительный порядок элементов в каждом диапазоне. Алгоритм merge не изменяет исходные диапазоны.

В целях упорядочения типы значений входных итераторов должны подлежать сравнению "меньше чем" для установления такого порядка, чтобы, имея два элемента, можно было определить, что они равны (ни один не меньше другого) или что один меньше другого. Это приводит к упорядочению неравнозначных элементов. Если эквивалентные элементы имеются в обоих исходных диапазонах, в диапазоне назначения элементы из первого диапазона будут предшествовать элементам из второго исходного диапазона. Если исходные диапазоны содержат повторяющиеся элементы и в первом исходном диапазоне их больше, чем во втором, диапазон назначения будет содержать число, на которое вхождения этих элементов в первом исходном диапазоне превышают вхождения этих элементов во втором исходном диапазоне.

Отношение сложности алгоритма линейное более 2 \* (( *last1 - first1*)-( *last2 - first2*)) – 1 сравнений для непустых исходных диапазонов.

### <a name="example"></a>Пример

```cpp
// alg_set_diff.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <functional>      // For greater<int>( )
#include <iostream>

// Return whether modulus of elem1 is less than modulus of elem2
bool mod_lesser (int elem1, int elem2 )
{
   if (elem1 < 0)
      elem1 = - elem1;
   if (elem2 < 0)
      elem2 = - elem2;
   return elem1 < elem2;
}

int main()
{
   using namespace std;
   vector <int> v1a, v1b, v1 ( 12 );
   vector <int>::iterator Iter1a,  Iter1b, Iter1, Result1;

   // Constructing vectors v1a & v1b with default less-than ordering
   int i;
   for ( i = -1 ; i <= 4 ; i++ )
   {
      v1a.push_back(  i );
   }

   int ii;
   for ( ii =-3 ; ii <= 0 ; ii++ )
   {
      v1b.push_back(  ii  );
   }

   cout << "Original vector v1a with range sorted by the\n "
        <<  "binary predicate less than is  v1a = ( " ;
   for ( Iter1a = v1a.begin( ) ; Iter1a != v1a.end( ) ; Iter1a++ )
      cout << *Iter1a << " ";
   cout << ")." << endl;

   cout << "Original vector v1b with range sorted by the\n "
        <<  "binary predicate less than is  v1b = ( " ;
   for ( Iter1b = v1b.begin( ) ; Iter1b != v1b.end( ) ; Iter1b++ )
      cout << *Iter1b << " ";
   cout << ")." << endl;

   // Constructing vectors v2a & v2b with ranges sorted by greater
   vector <int> v2a ( v1a ) , v2b ( v1b ) ,  v2 ( v1 );
   vector <int>::iterator Iter2a, Iter2b, Iter2, Result2;
   sort ( v2a.begin( ), v2a.end( ), greater<int>( ) );
   sort ( v2b.begin( ), v2b.end( ), greater<int>( ) );

   cout << "Original vector v2a with range sorted by the\n "
        <<  "binary predicate greater is   v2a =  ( " ;
   for ( Iter2a = v2a.begin( ) ; Iter2a != v2a.end( ) ; Iter2a++ )
      cout << *Iter2a << " ";
   cout << ")." << endl;

   cout << "Original vector v2b with range sorted by the\n "
        <<  "binary predicate greater is   v2b =  ( " ;
   for ( Iter2b = v2b.begin( ) ; Iter2b != v2b.end( ) ; Iter2b++ )
      cout << *Iter2b << " ";
   cout << ")." << endl;

   // Constructing vectors v3a & v3b with ranges sorted by mod_lesser
   vector <int> v3a ( v1a ), v3b ( v1b ) ,  v3 ( v1 );
   vector <int>::iterator Iter3a,  Iter3b, Iter3, Result3;
   sort ( v3a.begin( ), v3a.end( ), mod_lesser );
   sort ( v3b.begin( ), v3b.end( ), mod_lesser  );

   cout << "Original vector v3a with range sorted by the\n "
        <<  "binary predicate mod_lesser is   v3a =  ( " ;
   for ( Iter3a = v3a.begin( ) ; Iter3a != v3a.end( ) ; Iter3a++ )
      cout << *Iter3a << " ";
   cout << ")." << endl;

   cout << "Original vector v3b with range sorted by the\n "
        <<  "binary predicate mod_lesser is   v3b =  ( " ;
   for ( Iter3b = v3b.begin( ) ; Iter3b != v3b.end( ) ; Iter3b++ )
      cout << *Iter3b << " ";
   cout << ")." << endl;

   // To combine into a difference in asscending
   // order with the default binary predicate less <int>( )
   Result1 = set_difference ( v1a.begin( ), v1a.end( ),
      v1b.begin( ), v1b.end( ), v1.begin( ) );
   cout << "Set_difference of source ranges with default order,"
        << "\n vector v1mod =  ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != Result1 ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // To combine into a difference in descending
   // order specify binary predicate greater<int>( )
   Result2 = set_difference ( v2a.begin( ), v2a.end( ),
      v2b.begin( ), v2b.end( ),v2.begin( ), greater <int>( ) );
   cout << "Set_difference of source ranges with binary"
        << "predicate greater specified,\n vector v2mod  = ( " ;
   for ( Iter2 = v2.begin( ) ; Iter2 != Result2 ; Iter2++ )
      cout << *Iter2 << " ";
   cout << ")." << endl;

   // To combine into a difference applying a user
   // defined binary predicate mod_lesser
   Result3 = set_difference (  v3a.begin( ), v3a.end( ),
      v3b.begin( ), v3b.end( ), v3.begin( ), mod_lesser );
   cout << "Set_difference of source ranges with binary "
        << "predicate mod_lesser specified,\n vector v3mod  = ( " ; ;
   for ( Iter3 = v3.begin( ) ; Iter3 != Result3 ; Iter3++ )
      cout << *Iter3 << " ";
   cout << ")." << endl;
}
```

## <a name="set_intersection"></a>  set_intersection

Объединяет все элементы, входящие в оба исходных упорядоченных диапазона, в один упорядоченный диапазон назначения, где критерий порядка сортировки может быть указан бинарным предикатом.

```cpp
template<class InputIterator1, class InputIterator2, class OutputIterator>
OutputIterator set_intersection(
    InputIterator1 first1,
    InputIterator1 last1,
    InputIterator2 first2,
    InputIterator2 last2,
    OutputIterator result );

template<class InputIterator1, class InputIterator2, class OutputIterator, class BinaryPredicate>
OutputIterator set_intersection(
    InputIterator1 first1,
    InputIterator1 last1,
    InputIterator2 first2,
    InputIterator2 last2,
    OutputIterator result,
    BinaryPredicate comp );
```

### <a name="parameters"></a>Параметры

*first1*<br/>
Входной итератор, указывающий на позицию первого элемента в первом из двух упорядоченных исходных диапазонов, которые следует объединить и упорядочить в один диапазон, представляющий пересечение двух исходных диапазонов.

*last1*<br/>
Входной итератор, указывающий на позицию, следующую за последним элементом в первом из двух упорядоченных исходных диапазонов, которые следует объединить и упорядочить в один диапазон, представляющий пересечение двух исходных диапазонов.

*first2*<br/>
Входной итератор, указывающий на позицию первого элемента во втором из двух последовательных упорядоченных исходных диапазонов, которые следует объединить и упорядочить в один диапазон, представляющий пересечение двух исходных диапазонов.

*last2*<br/>
Входной итератор, указывающий на позицию, следующую за последним элементом во втором из двух последовательных упорядоченных исходных диапазонов, которые следует объединить и упорядочить в один диапазон, представляющий пересечение двух исходных диапазонов.

**_** *Результат* выходной итератор, обращающийся к позиции первого элемента в диапазоне назначения, где два источника диапазоны, следует объединить в один упорядоченный диапазон, представляющий пересечение двух исходных диапазоны.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, определяющий условие, когда один элемент больше другого. Бинарный предикат принимает два аргумента и должен возвращать значение **true** , когда первый элемент меньше второго элемента, и значение **false** в противном случае.

### <a name="return-value"></a>Возвращаемое значение

Выходной итератор, указывающий на позицию, следующую за последним элементом в упорядоченном диапазоне назначения, представляющем пересечение двух исходных диапазонов.

### <a name="remarks"></a>Примечания

Упорядоченные исходные диапазоны, на которые указывают ссылки, должны быть допустимыми. Все указатели должны поддерживать отмену ссылок. В каждой последовательности должна быть возможность достижения последней позиции с первой путем приращения.

Диапазон назначения не должен перекрывать исходные диапазоны и должен быть достаточно большим, чтобы содержать диапазон назначения.

Каждый упорядоченный исходный диапазон должен быть упорядочен в качестве предусловия для применения алгоритма merge в соответствии с тем же правилами, чтобы использоваться алгоритмом для упорядочения объединенных диапазонов.

Операция стабильна, так как в диапазоне назначения сохраняется относительный порядок элементов в каждом диапазоне. Алгоритм не изменяет исходные диапазоны.

В целях упорядочения типы значений входных итераторов должны подлежать сравнению "меньше чем" для установления такого порядка, чтобы, имея два элемента, можно было определить, что они равны (ни один не меньше другого) или что один меньше другого. Это приводит к упорядочению неравнозначных элементов. Если эквивалентные элементы имеются в обоих исходных диапазонах, в диапазоне назначения элементы из первого диапазона будут предшествовать элементам из второго исходного диапазона. Если исходные диапазоны содержат повторяющиеся элементы, диапазон назначения будет содержать максимальное количество элементов, входящих в оба исходных диапазона.

Отношение сложности алгоритма линейное более 2 \* (( *last1 - first1*) + ( *last2 - first2*)) – 1 сравнений для непустых исходных диапазонов.

### <a name="example"></a>Пример

```cpp
// alg_set_intersection.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <functional>   // For greater<int>( )
#include <iostream>

// Return whether modulus of elem1 is less than modulus of elem2
bool mod_lesser (int elem1, int elem2 ) {
   if ( elem1 < 0 )
      elem1 = - elem1;
   if ( elem2 < 0 )
      elem2 = - elem2;
   return elem1 < elem2;
}

int main() {
   using namespace std;
   vector <int> v1a, v1b, v1 ( 12 );
   vector <int>::iterator Iter1a,  Iter1b, Iter1, Result1;

   // Constructing vectors v1a & v1b with default less than ordering
   int i;
   for ( i = -1 ; i <= 3 ; i++ )
      v1a.push_back( i );

   int ii;
   for ( ii =-3 ; ii <= 1 ; ii++ )
      v1b.push_back( ii );

   cout << "Original vector v1a with range sorted by the\n "
        <<  "binary predicate less than is  v1a = ( " ;
   for ( Iter1a = v1a.begin( ) ; Iter1a != v1a.end( ) ; Iter1a++ )
      cout << *Iter1a << " ";
   cout << ")." << endl;

   cout << "Original vector v1b with range sorted by the\n "
        <<  "binary predicate less than is  v1b = ( " ;
   for ( Iter1b = v1b.begin( ) ; Iter1b != v1b.end( ) ; Iter1b++ )
      cout << *Iter1b << " ";
   cout << ")." << endl;

   // Constructing vectors v2a & v2b with ranges sorted by greater
   vector <int> v2a ( v1a ) , v2b ( v1b ) , v2 ( v1 );
   vector <int>::iterator Iter2a, Iter2b, Iter2, Result2;
   sort ( v2a.begin( ), v2a.end( ), greater<int>( ) );
   sort ( v2b.begin( ), v2b.end( ), greater<int>( ) );

   cout << "Original vector v2a with range sorted by the\n "
        << "binary predicate greater is   v2a =  ( " ;
   for ( Iter2a = v2a.begin( ) ; Iter2a != v2a.end( ) ; Iter2a++ )
      cout << *Iter2a << " ";
   cout << ")." << endl;

   cout << "Original vector v2b with range sorted by the\n "
        << "binary predicate greater is   v2b =  ( " ;
   for ( Iter2b = v2b.begin( ) ; Iter2b != v2b.end( ) ; Iter2b++ )
      cout << *Iter2b << " ";
   cout << ")." << endl;

   // Constructing vectors v3a & v3b with ranges sorted by mod_lesser
   vector <int> v3a ( v1a ), v3b ( v1b ) , v3 ( v1 );
   vector <int>::iterator Iter3a,  Iter3b, Iter3, Result3;
   sort ( v3a.begin( ), v3a.end( ), mod_lesser );
   sort ( v3b.begin( ), v3b.end( ), mod_lesser );

   cout << "Original vector v3a with range sorted by the\n "
        <<  "binary predicate mod_lesser is   v3a =  ( " ;
   for ( Iter3a = v3a.begin( ) ; Iter3a != v3a.end( ) ; Iter3a++ )
      cout << *Iter3a << " ";
   cout << ")." << endl;

   cout << "Original vector v3b with range sorted by the\n "
           <<  "binary predicate mod_lesser is   v3b =  ( " ;
   for ( Iter3b = v3b.begin( ) ; Iter3b != v3b.end( ) ; Iter3b++ )
      cout << *Iter3b << " ";
   cout << ")." << endl;

   // To combine into an intersection in asscending order with the
   // default binary predicate less <int>( )
   Result1 = set_intersection ( v1a.begin( ), v1a.end( ),
      v1b.begin( ), v1b.end( ), v1.begin( ) );
   cout << "Intersection of source ranges with default order,"
        << "\n vector v1mod =  ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != Result1 ; ++Iter1 )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // To combine into an intersection in descending order, specify
   // binary predicate greater<int>( )
   Result2 = set_intersection ( v2a.begin( ), v2a.end( ),
      v2b.begin( ), v2b.end( ),v2.begin( ), greater <int>( ) );
   cout << "Intersection of source ranges with binary predicate"
        << " greater specified,\n vector v2mod  = ( " ;
   for ( Iter2 = v2.begin( ) ; Iter2 != Result2 ; ++Iter2 )
      cout << *Iter2 << " ";
   cout << ")." << endl;

   // To combine into an intersection applying a user-defined
   // binary predicate mod_lesser
   Result3 = set_intersection ( v3a.begin( ), v3a.end( ),
      v3b.begin( ), v3b.end( ), v3.begin( ), mod_lesser );
   cout << "Intersection of source ranges with binary predicate "
        << "mod_lesser specified,\n vector v3mod  = ( " ; ;
   for ( Iter3 = v3.begin( ) ; Iter3 != Result3 ; ++Iter3 )
      cout << *Iter3 << " ";
   cout << ")." << endl;
}
```

## <a name="set_symmetric_difference"></a>  set_symmetric_difference

Объединяет все элементы, входящие в один, но не в оба исходных упорядоченных диапазона, в один упорядоченный диапазон назначения, где критерий порядка сортировки может быть указан бинарным предикатом.

```cpp
template<class InputIterator1, class InputIterator2, class OutputIterator>
OutputIterator set_symmetric_difference(
    InputIterator1 first1,
    InputIterator1 last1,
    InputIterator2 first2,
    InputIterator2 last2,
    OutputIterator result );

template<class InputIterator1, class InputIterator2, class OutputIterator, class BinaryPredicate>
OutputIterator set_symmetric_difference(
    InputIterator1 first1,
    InputIterator1 last1,
    InputIterator2 first2,
    InputIterator2 last2,
    OutputIterator result,
    BinaryPredicate comp );

```

### <a name="parameters"></a>Параметры

*first1*<br/>
Входной итератор, указывающий на позицию первого элемента в первом из двух упорядоченных исходных диапазонов, которые следует объединить и упорядочить в один диапазон, представляющий симметрическую разность двух исходных диапазонов.

*last1*<br/>
Входной итератор, указывающий на позицию, следующую за последним элементом в первом из двух упорядоченных исходных диапазонов, которые следует объединить и упорядочить в один диапазон, представляющий симметрическую разность двух исходных диапазонов.

*first2*<br/>
Входной итератор, указывающий на позицию первого элемента во втором из двух последовательных упорядоченных исходных диапазонов, которые следует объединить и упорядочить в один диапазон, представляющий симметрическую разность двух исходных диапазонов.

*last2*<br/>
Входной итератор, указывающий на позицию, следующую за последним элементом во втором из двух последовательных упорядоченных исходных диапазонов, которые следует объединить и упорядочить в один диапазон, представляющий симметрическую разность двух исходных диапазонов.

**_** *Результат* выходной итератор, обращающийся к позиции первого элемента в диапазоне назначения, где два источника диапазоны, следует объединить в один упорядоченный диапазон, представляющий симметрическую разность двух исходных диапазонов.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, определяющий условие, когда один элемент больше другого. Бинарный предикат принимает два аргумента и должен возвращать значение **true** , когда первый элемент меньше второго элемента, и значение **false** в противном случае.

### <a name="return-value"></a>Возвращаемое значение

Выходной итератор, указывающий на позицию, следующую за последним элементом в упорядоченном диапазоне назначения, представляющем симметрическую разность двух исходных диапазонов.

### <a name="remarks"></a>Примечания

Упорядоченные исходные диапазоны, на которые указывают ссылки, должны быть допустимыми. Все указатели должны поддерживать отмену ссылок. В каждой последовательности должна быть возможность достижения последней позиции с первой путем приращения.

Диапазон назначения не должен перекрывать исходные диапазоны и должен быть достаточно большим, чтобы содержать диапазон назначения.

Каждый упорядоченный исходный диапазон должны быть упорядочен в качестве предусловия для применения алгоритма `merge*` в соответствии с теми же правилами, чтобы использоваться алгоритмом для упорядочения объединенных диапазонов.

Операция стабильна, так как в диапазоне назначения сохраняется относительный порядок элементов в каждом диапазоне. Алгоритм merge не изменяет исходные диапазоны.

В целях упорядочения типы значений входных итераторов должны подлежать сравнению "меньше чем" для установления такого порядка, чтобы, имея два элемента, можно было определить, что они равны (ни один не меньше другого) или что один меньше другого. Это приводит к упорядочению неравнозначных элементов. Если эквивалентные элементы имеются в обоих исходных диапазонах, в диапазоне назначения элементы из первого диапазона будут предшествовать элементам из второго исходного диапазона. Если исходные диапазоны содержат повторяющиеся элементы, диапазон назначения будет содержать абсолютное значение числа, на которое вхождения этих элементов в одном исходном диапазоне превышают вхождения этих элементов во втором исходном диапазоне.

Отношение сложности алгоритма линейное более 2 \* ((*last1 - first1*)-(*last2 - first2*)) – 1 сравнений для непустых исходных диапазонов.

### <a name="example"></a>Пример

```cpp
// alg_set_sym_diff.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <functional>      // For greater<int>( )
#include <iostream>

// Return whether modulus of elem1 is less than modulus of elem2
bool mod_lesser (int elem1, int elem2 )
{
   if ( elem1 < 0 )
      elem1 = - elem1;
   if ( elem2 < 0 )
      elem2 = - elem2;
   return elem1 < elem2;
}

int main()
{
   using namespace std;
   vector <int> v1a, v1b, v1 ( 12 );
   vector <int>::iterator Iter1a,  Iter1b, Iter1, Result1;

   // Constructing vectors v1a & v1b with default less-than ordering
   int i;
   for ( i = -1 ; i <= 4 ; i++ )
   {
      v1a.push_back(  i );
   }

   int ii;
   for ( ii =-3 ; ii <= 0 ; ii++ )
   {
      v1b.push_back(  ii  );
   }

   cout << "Original vector v1a with range sorted by the\n "
        <<  "binary predicate less than is  v1a = ( " ;
   for ( Iter1a = v1a.begin( ) ; Iter1a != v1a.end( ) ; Iter1a++ )
      cout << *Iter1a << " ";
   cout << ")." << endl;

   cout << "Original vector v1b with range sorted by the\n "
        <<  "binary predicate less than is  v1b = ( " ;
   for ( Iter1b = v1b.begin( ) ; Iter1b != v1b.end( ) ; Iter1b++ )
      cout << *Iter1b << " ";
   cout << ")." << endl;

   // Constructing vectors v2a & v2b with ranges sorted by greater
   vector <int> v2a ( v1a ) , v2b ( v1b ) ,  v2 ( v1 );
   vector <int>::iterator Iter2a, Iter2b, Iter2, Result2;
   sort ( v2a.begin( ), v2a.end( ), greater<int>( ) );
   sort ( v2b.begin( ), v2b.end( ), greater<int>( ) );

   cout << "Original vector v2a with range sorted by the\n "
        <<  "binary predicate greater is   v2a =  ( " ;
   for ( Iter2a = v2a.begin( ) ; Iter2a != v2a.end( ) ; Iter2a++ )
      cout << *Iter2a << " ";
   cout << ")." << endl;

   cout << "Original vector v2b with range sorted by the\n "
        <<  "binary predicate greater is   v2b =  ( " ;
   for ( Iter2b = v2b.begin( ) ; Iter2b != v2b.end( ) ; Iter2b++ )
      cout << *Iter2b << " ";
   cout << ")." << endl;

   // Constructing vectors v3a & v3b with ranges sorted by mod_lesser
   vector <int> v3a ( v1a ), v3b ( v1b ) ,  v3 ( v1 );
   vector <int>::iterator Iter3a, Iter3b, Iter3, Result3;
   sort ( v3a.begin( ), v3a.end( ), mod_lesser );
   sort ( v3b.begin( ), v3b.end( ), mod_lesser  );

   cout << "Original vector v3a with range sorted by the\n "
        <<  "binary predicate mod_lesser is   v3a =  ( " ;
   for ( Iter3a = v3a.begin( ) ; Iter3a != v3a.end( ) ; Iter3a++ )
      cout << *Iter3a << " ";
   cout << ")." << endl;

   cout << "Original vector v3b with range sorted by the\n "
        <<  "binary predicate mod_lesser is   v3b =  ( " ;
   for ( Iter3b = v3b.begin( ) ; Iter3b != v3b.end( ) ; Iter3b++ )
      cout << *Iter3b << " ";
   cout << ")." << endl;

   // To combine into a symmetric difference in ascending
   // order with the default binary predicate less <int>( )
   Result1 = set_symmetric_difference ( v1a.begin( ), v1a.end( ),
      v1b.begin( ), v1b.end( ), v1.begin( ) );
   cout << "Set_symmetric_difference of source ranges with default order,"
        << "\n vector v1mod =  ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != Result1 ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // To combine into a symmetric difference in descending
   // order, specify binary predicate greater<int>( )
   Result2 = set_symmetric_difference ( v2a.begin( ), v2a.end( ),
      v2b.begin( ), v2b.end( ),v2.begin( ), greater <int>( ) );
   cout << "Set_symmetric_difference of source ranges with binary"
        << "predicate greater specified,\n vector v2mod  = ( " ;
   for ( Iter2 = v2.begin( ) ; Iter2 != Result2 ; Iter2++ )
      cout << *Iter2 << " ";
   cout << ")." << endl;

   // To combine into a symmetric difference applying a user
   // defined binary predicate mod_lesser
   Result3 = set_symmetric_difference ( v3a.begin( ), v3a.end( ),
      v3b.begin( ), v3b.end( ), v3.begin( ), mod_lesser );
   cout << "Set_symmetric_difference of source ranges with binary "
        << "predicate mod_lesser specified,\n vector v3mod  = ( " ; ;
   for ( Iter3 = v3.begin( ) ; Iter3 != Result3 ; Iter3++ )
      cout << *Iter3 << " ";
   cout << ")." << endl;
}
```

## <a name="set_union"></a>  set_union

Объединяет все элементы, входящие в хотя бы один из двух исходных упорядоченных диапазонов, в один упорядоченный диапазон назначения, где критерий порядка сортировки может быть указан бинарным предикатом.

```cpp
template<class InputIterator1, class InputIterator2, class OutputIterator>
OutputIterator set_union(
    InputIterator1 first1,
    InputIterator1 last1,
    InputIterator2 first2,
    InputIterator2 last2,
    OutputIterator result );

template<class InputIterator1, class InputIterator2, class OutputIterator, class BinaryPredicate>
OutputIterator set_union(
    InputIterator1 first1,
    InputIterator1 last1,
    InputIterator2 first2,
    InputIterator2 last2,
    OutputIterator result,
    BinaryPredicate comp );
```

### <a name="parameters"></a>Параметры

*first1*<br/>
Входной итератор, указывающий на позицию первого элемента в первом из двух упорядоченных исходных диапазонов, которые следует объединить и упорядочить в один диапазон, представляющий объединение двух исходных диапазонов.

*last1*<br/>
Входной итератор, указывающий на позицию, следующую за последним элементом в первом из двух упорядоченных исходных диапазонов, которые следует объединить и упорядочить в один диапазон, представляющий объединение двух исходных диапазонов.

*first2*<br/>
Входной итератор, указывающий на позицию первого элемента во втором из двух последовательных упорядоченных исходных диапазонов, которые следует объединить и упорядочить в один диапазон, представляющий объединение двух исходных диапазонов.

*last2*<br/>
Входной итератор, указывающий на позицию, следующую за последним элементом во втором из двух последовательных упорядоченных исходных диапазонов, которые следует объединить и упорядочить в один диапазон, представляющий объединение двух исходных диапазонов.

**_** *Результат* выходной итератор, обращающийся к позиции первого элемента в диапазоне назначения, где два источника диапазоны, следует объединить в один упорядоченный диапазон, представляющий объединение двух исходных диапазонов.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, определяющий условие, когда один элемент больше другого. Бинарный предикат принимает два аргумента и должен возвращать значение **true** , когда первый элемент меньше второго элемента, и значение **false** в противном случае.

### <a name="return-value"></a>Возвращаемое значение

Выходной итератор, указывающий на позицию, следующую за последним элементом в упорядоченном диапазоне назначения, представляющем объединение двух исходных диапазонов.

### <a name="remarks"></a>Примечания

Упорядоченные исходные диапазоны, на которые указывают ссылки, должны быть допустимыми. Все указатели должны поддерживать отмену ссылок. В каждой последовательности должна быть возможность достижения последней позиции с первой путем приращения.

Диапазон назначения не должен перекрывать исходные диапазоны и должен быть достаточно большим, чтобы содержать диапазон назначения.

Каждый упорядоченный исходный диапазон должны быть упорядочен в качестве предусловия для применения алгоритма `merge` в соответствии с теми же правилами, чтобы использоваться алгоритмом для упорядочения объединенных диапазонов.

Операция стабильна, так как в диапазоне назначения сохраняется относительный порядок элементов в каждом диапазоне. Алгоритм не изменяет исходные диапазоны `merge`.

В целях упорядочения типы значений входных итераторов должны подлежать сравнению "меньше чем" для установления такого порядка, чтобы, имея два элемента, можно было определить, что они равны (ни один не меньше другого) или что один меньше другого. Это приводит к упорядочению неравнозначных элементов. Если эквивалентные элементы имеются в обоих исходных диапазонах, в диапазоне назначения элементы из первого диапазона будут предшествовать элементам из второго исходного диапазона. Если исходные диапазоны содержат повторяющиеся элементы, диапазон назначения будет содержать максимальное количество элементов, входящих в оба исходных диапазона.

Отношение сложности алгоритма линейное более 2 \* (( *last1 - first1*)-( *last2 - first2*)) – 1 сравнений.

### <a name="example"></a>Пример

```cpp
// alg_set_union.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <functional>      // For greater<int>( )
#include <iostream>

// Return whether modulus of elem1 is less than modulus of elem2
bool mod_lesser ( int elem1, int elem2 )
{
   if ( elem1 < 0 )
      elem1 = - elem1;
   if ( elem2 < 0 )
      elem2 = - elem2;
   return elem1 < elem2;
}

int main()
{
   using namespace std;
   vector <int> v1a, v1b, v1 ( 12 );
   vector <int>::iterator Iter1a, Iter1b, Iter1, Result1;

   // Constructing vectors v1a & v1b with default less than ordering
   int i;
   for ( i = -1 ; i <= 3 ; i++ )
   {
      v1a.push_back(  i );
   }

   int ii;
   for ( ii =-3 ; ii <= 1 ; ii++ )
   {
      v1b.push_back(  ii  );
   }

   cout << "Original vector v1a with range sorted by the\n "
        <<  "binary predicate less than is  v1a = ( " ;
   for ( Iter1a = v1a.begin( ) ; Iter1a != v1a.end( ) ; Iter1a++ )
      cout << *Iter1a << " ";
   cout << ")." << endl;

   cout << "Original vector v1b with range sorted by the\n "
        <<  "binary predicate less than is  v1b = ( " ;
   for ( Iter1b = v1b.begin( ) ; Iter1b != v1b.end( ) ; Iter1b++ )
      cout << *Iter1b << " ";
   cout << ")." << endl;

   // Constructing vectors v2a & v2b with ranges sorted by greater
   vector <int> v2a ( v1a ) , v2b ( v1b ) , v2 ( v1 );
   vector <int>::iterator Iter2a,  Iter2b, Iter2, Result2;
   sort ( v2a.begin( ), v2a.end( ), greater<int>( ) );
   sort ( v2b.begin( ), v2b.end( ), greater<int>( ) );

   cout << "Original vector v2a with range sorted by the\n "
        <<  "binary predicate greater is   v2a =  ( " ;
   for ( Iter2a = v2a.begin( ) ; Iter2a != v2a.end( ) ; Iter2a++ )
      cout << *Iter2a << " ";
   cout << ")." << endl;

   cout << "Original vector v2b with range sorted by the\n "
        <<  "binary predicate greater is   v2b =  ( " ;
   for ( Iter2b = v2b.begin( ) ; Iter2b != v2b.end( ) ; Iter2b++ )
      cout << *Iter2b << " ";
   cout << ")." << endl;

   // Constructing vectors v3a & v3b with ranges sorted by mod_lesser
   vector <int> v3a ( v1a ), v3b ( v1b ) ,  v3 ( v1 );
   vector <int>::iterator Iter3a, Iter3b, Iter3, Result3;
   sort ( v3a.begin( ), v3a.end( ), mod_lesser );
   sort ( v3b.begin( ), v3b.end( ), mod_lesser  );

   cout << "Original vector v3a with range sorted by the\n "
        <<  "binary predicate mod_lesser is   v3a =  ( " ;
   for ( Iter3a = v3a.begin( ) ; Iter3a != v3a.end( ) ; Iter3a++ )
      cout << *Iter3a << " ";
   cout << ")." << endl;

   cout << "Original vector v3b with range sorted by the\n "
        <<  "binary predicate mod_lesser is   v3b =  ( " ;
   for ( Iter3b = v3b.begin( ) ; Iter3b != v3b.end( ) ; Iter3b++ )
      cout << *Iter3b << " ";
   cout << ")." << endl;

   // To combine into a union in ascending order with the default
    // binary predicate less <int>( )
   Result1 = set_union ( v1a.begin( ), v1a.end( ),
      v1b.begin( ), v1b.end( ), v1.begin( ) );
   cout << "Union of source ranges with default order,"
        << "\n vector v1mod =  ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != Result1 ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // To combine into a union in descending order, specify binary
   // predicate greater<int>( )
   Result2 = set_union (  v2a.begin( ), v2a.end( ),
      v2b.begin( ), v2b.end( ),v2.begin( ), greater <int>( ) );
   cout << "Union of source ranges with binary predicate greater "
        << "specified,\n vector v2mod  = ( " ;
   for ( Iter2 = v2.begin( ) ; Iter2 != Result2 ; Iter2++ )
      cout << *Iter2 << " ";
   cout << ")." << endl;

   // To combine into a union applying a user-defined
   // binary predicate mod_lesser
   Result3 = set_union ( v3a.begin( ), v3a.end( ),
      v3b.begin( ), v3b.end( ), v3.begin( ), mod_lesser );
   cout << "Union of source ranges with binary predicate "
        << "mod_lesser specified,\n vector v3mod  = ( " ; ;
   for ( Iter3 = v3.begin( ) ; Iter3 != Result3 ; Iter3++ )
      cout << *Iter3 << " ";
   cout << ")." << endl;
}
```

## <a name="shuffle"></a>  std::shuffle

Перемешивает (изменяет порядок) элементы в указанном диапазоне, используя генератор случайных чисел.

```cpp
template<class RandomAccessIterator, class UniformRandomNumberGenerator>
void shuffle(RandomAccessIterator first,
    RandomAccessIterator last,
    UniformRandomNumberGenerator&& gen);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Итератор первого элемента в диапазоне, который необходимо перемешать (инклюзивно). Должен соответствовать требованиям `RandomAccessIterator` и `ValueSwappable`.

*последний*<br/>
Итератор последнего элемента в диапазоне, который необходимо перемешать (эксклюзивно). Должен соответствовать требованиям `RandomAccessIterator` и `ValueSwappable`.

*Gen*<br/>
Генератор случайных чисел, который будет использовать функция `shuffle()`. Должен соответствовать требованиям `UniformRandomNumberGenerator`.

### <a name="remarks"></a>Примечания

Дополнительные сведения и пример кода, использующего `shuffle()`, см. в разделе [\<random>](../standard-library/random.md).

## <a name="sort"></a>  sort

Упорядочивает элементы в указанном диапазоне в не нисходящем порядке или согласно критерию упорядочивания, заданному бинарным предикатом.

```cpp
template<class RandomAccessIterator>
   void sort(
      RandomAccessIterator first,
      RandomAccessIterator last);

template<class RandomAccessIterator, class Predicate>
   void sort(
      RandomAccessIterator first,
      RandomAccessIterator last,
      Predicate comp);

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Итератор произвольного доступа, обращающийся к позиции первого элемента в сортируемом диапазоне.

*последний*<br/>
Итератор произвольного доступа, обращающийся к позиции после последнего элемента в сортируемом диапазоне.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, задающий критерий сравнения, который должен соблюдаться идущими подряд элементами при упорядочении. Этот бинарный предикат принимает два аргумента и возвращает **true** Если оба аргумента являются в порядке и **false** в противном случае. Эта функция средства сравнения должна задать строгое слабое упорядочение пар элементов последовательности. Дополнительные сведения см. в разделе [Алгоритмы](../standard-library/algorithms.md).

### <a name="remarks"></a>Примечания

Указанный диапазон должен быть допустимым. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Если ни один из элементов не меньше другого, то эти элементы эквивалентны, но не обязательно равны. Алгоритм `sort` нестабилен и поэтому не гарантирует, что относительный порядок эквивалентных элементов будет сохранен. Алгоритм `stable_sort` сохраняет этот исходный порядок.

Средняя сложность сортировки — *O*( *N* журнала *N*), где *N* =  *фамилия - имя*.

### <a name="example"></a>Пример

```cpp
// alg_sort.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <functional>      // For greater<int>( )
#include <iostream>

// Return whether first element is greater than the second
bool UDgreater ( int elem1, int elem2 )
{
   return elem1 > elem2;
}

int main()
{
   using namespace std;
   vector <int> v1;
   vector <int>::iterator Iter1;

   int i;
   for ( i = 0 ; i <= 5 ; i++ )
   {
      v1.push_back( 2 * i );
   }

   int ii;
   for ( ii = 0 ; ii <= 5 ; ii++ )
   {
      v1.push_back( 2 * ii + 1 );
   }

   cout << "Original vector v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;

   sort( v1.begin( ), v1.end( ) );
   cout << "Sorted vector v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;

   // To sort in descending order. specify binary predicate
   sort( v1.begin( ), v1.end( ), greater<int>( ) );
   cout << "Resorted (greater) vector v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;

   // A user-defined (UD) binary predicate can also be used
   sort( v1.begin( ), v1.end( ), UDgreater );
   cout << "Resorted (UDgreater) vector v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;
}
```

```Output
Original vector v1 = ( 0 2 4 6 8 10 1 3 5 7 9 11 )
Sorted vector v1 = ( 0 1 2 3 4 5 6 7 8 9 10 11 )
Resorted (greater) vector v1 = ( 11 10 9 8 7 6 5 4 3 2 1 0 )
Resorted (UDgreater) vector v1 = ( 11 10 9 8 7 6 5 4 3 2 1 0 )
```

## <a name="sort_heap"></a>  sort_heap

Преобразует кучу в упорядоченный диапазон.

```cpp
template<class RandomAccessIterator>
   void sort_heap(
      RandomAccessIterator first,
      RandomAccessIterator last);

template<class RandomAccessIterator, class Predicate>
   void sort_heap(
      RandomAccessIterator first,
      RandomAccessIterator last,
      Predicate comp);
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Итератор произвольного доступа, обращающийся к позиции первого элемента в целевой куче.

*последний*<br/>
Итератор произвольного доступа, обращающийся к позиции, следующей за последним элементом в целевой куче.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, задающий условие, когда один элемент меньше другого. Двоичный предикат принимает два аргумента и возвращает **true** , если условие удовлетворено, или **false** , если условие не удовлетворено.

### <a name="remarks"></a>Примечания

Кучи имеют два следующих свойства.

- Первый элемент — всегда наибольший.

- Элементы могут добавляться и удаляться в логарифмическое время.

После применения этого алгоритма диапазон, к которому он был применен, больше не является кучей.

Это не устойчивая сортировка, так как относительный порядок эквивалентных элементов не обязательно сохраняется.

Кучи — идеальный способ реализации очередей с приоритетами, и они используются в [классе priority_queue](../standard-library/priority-queue-class.md) адаптеров контейнеров библиотеки стандартных программ C++.

Указанный диапазон должен быть допустимым. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Отношение сложности — не более *N* журнала *N*, где *N* = ( *фамилия - имя*).

### <a name="example"></a>Пример

```cpp
// alg_sort_heap.cpp
// compile with: /EHsc
#include <algorithm>
#include <functional>
#include <iostream>
#include <ostream>
#include <string>
#include <vector>
using namespace std;

void print(const string& s, const vector<int>& v) {
    cout << s << ": ( ";

    for (auto i = v.begin(); i != v.end(); ++i) {
        cout << *i << " ";
    }

    cout << ")" << endl;
}

int main() {
    vector<int> v;
    for (int i = 1; i <= 9; ++i) {
        v.push_back(i);
    }
    print("Initially", v);

    random_shuffle(v.begin(), v.end());
    print("After random_shuffle", v);

    make_heap(v.begin(), v.end());
    print("     After make_heap", v);

    sort_heap(v.begin(), v.end());
    print("     After sort_heap", v);

    random_shuffle(v.begin(), v.end());
    print("             After random_shuffle", v);

    make_heap(v.begin(), v.end(), greater<int>());
    print("After make_heap with greater<int>", v);

    sort_heap(v.begin(), v.end(), greater<int>());
    print("After sort_heap with greater<int>", v);
}
```

## <a name="stable_partition"></a>  stable_partition

Разделяет элементы диапазона на два непересекающихся множества, при этом элементы, удовлетворяющие унарному предикату, расположены перед теми, которые ему не удовлетворяют, с сохранением относительного порядка равноценных элементов.

```cpp
template<class BidirectionalIterator, class Predicate>
BidirectionalIterator stable_partition(
    BidirectionalIterator first,
    BidirectionalIterator last,
    Predicate pred );

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Двунаправленный итератор адресует позицию первого элемента в разделяемом диапазоне.

*последний*<br/>
Двунаправленный итератор, указывающий позицию, следующую за последним элементом в разделяемом диапазоне.

*_Pred*<br/>
Определенный пользователем объект функции предиката, задающий условие, которое должно удовлетворяться, чтобы элемент был классифицирован. Предикат принимает один аргумент и возвращает значение **true** или **false**.

### <a name="return-value"></a>Возвращаемое значение

Двунаправленный итератор указывает позицию первого элемента в диапазоне, не соответствующего условию предиката.

### <a name="remarks"></a>Примечания

Указанный диапазон должен быть допустимым. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Элементы *a* и *b* эквивалентны, но не обязательно равны, если и *Pr* (*a*, *b*) имеет значение false, и *Pr* (*b*, *a*) имеет значение false, где *Pr* — это предикат, заданный в параметре. `stable_ partition` Алгоритм стабилен и гарантирует, что относительный порядок эквивалентных элементов будет сохранен. Алгоритм `partition` не обязательно сохраняет этот исходный порядок.

### <a name="example"></a>Пример

```cpp
// alg_stable_partition.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <iostream>

bool greater5 ( int value ) {
   return value > 5;
}

int main() {
   using namespace std;
   vector <int> v1, v2;
   vector <int>::iterator Iter1, Iter2, result;

   int i;
   for ( i = 0 ; i <= 10 ; i++ )
      v1.push_back( i );

   int ii;
   for ( ii = 0 ; ii <= 4 ; ii++ )
      v1.push_back( 5 );

   random_shuffle(v1.begin( ), v1.end( ) );

   cout << "Vector v1 is ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Partition the range with predicate greater10
   result = stable_partition (v1.begin( ), v1.end( ), greater5 );
   cout << "The partitioned set of elements in v1 is:\n ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   cout << "The first element in v1 to fail to satisfy the"
        << "\n predicate greater5 is: " << *result << "." << endl;
}
```

## <a name="stable_sort"></a>  stable_sort

Упорядочивает элементы в указанном диапазоне в не нисходящем порядке или согласно критерию упорядочивания, заданному бинарным предикатом, и сохраняет относительный порядок равноценных элементов.

```cpp
template<class BidirectionalIterator>
void stable_sort( BidirectionalIterator first, BidirectionalIterator last );

template<class BidirectionalIterator, class BinaryPredicate>
void stable_sort(
    BidirectionalIterator first,
    BidirectionalIterator last,
    BinaryPredicate comp );

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Двунаправленный итератор указывает позицию первого элемента в диапазоне для сортировки.

*последний*<br/>
Двунаправленный итератор указывает позицию, следующую за последним элементом в диапазоне для сортировки.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, задающий критерий сравнения, который должен соблюдаться идущими подряд элементами при упорядочении. Двоичный предикат принимает два аргумента и возвращает **true** , если условие удовлетворено, или **false** , если условие не удовлетворено.

### <a name="remarks"></a>Примечания

Указанный диапазон должен быть допустимым. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один.

Если ни один из элементов не меньше другого, то эти элементы эквивалентны, но не обязательно равны. `sort` Алгоритм стабилен и гарантирует, что относительный порядок эквивалентных элементов будет сохранен.

Сложность выполнения `stable_sort` зависит от объема доступной памяти, но (при наличии достаточного объема памяти) лучшим вариантом является *O*( *N* журнала *N*) и в худшем случае — *O*( *N* (журнала *N* ) 2), где *N* =  *last - First.* Как правило `sort` алгоритм работает значительно быстрее, чем `stable_sort`.

### <a name="example"></a>Пример

```cpp
// alg_stable_sort.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <functional>      // For greater<int>( )
#include <iostream>

// Return whether first element is greater than the second
bool UDgreater (int elem1, int elem2 )
{
   return elem1 > elem2;
}

int main()
{
   using namespace std;
   vector <int> v1;
   vector <int>::iterator Iter1;

   int i;
   for ( i = 0 ; i <= 5 ; i++ )
   {
      v1.push_back( 2 * i );
   }

   for ( i = 0 ; i <= 5 ; i++ )
   {
      v1.push_back( 2 * i  );
   }

   cout << "Original vector v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;

   stable_sort(v1.begin( ), v1.end( ) );
   cout << "Sorted vector v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;

   // To sort in descending order, specify binary predicate
   stable_sort(v1.begin( ), v1.end( ), greater<int>( ) );
   cout << "Resorted (greater) vector v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;

   // A user-defined (UD) binary predicate can also be used
   stable_sort(v1.begin( ), v1.end( ), UDgreater );
   cout << "Resorted (UDgreater) vector v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")" << endl;
}
```

```Output
Original vector v1 = ( 0 2 4 6 8 10 0 2 4 6 8 10 )
Sorted vector v1 = ( 0 0 2 2 4 4 6 6 8 8 10 10 )
Resorted (greater) vector v1 = ( 10 10 8 8 6 6 4 4 2 2 0 0 )
Resorted (UDgreater) vector v1 = ( 10 10 8 8 6 6 4 4 2 2 0 0 )
```

## <a name="swap"></a>  swap

Первое переопределение меняет местами значения двух объектов. Второе переопределение меняет местами значения двух массивов объектов.

```cpp
template<class Type>
   void swap(
      Type& left,
      Type& right);
template<class Type, size_t N>
   void swap(
      Type (& left)[N],
      Type (& right)[N]);\r

```

### <a name="parameters"></a>Параметры

*left*<br/>
Для первого переопределения — первый объект для обмена его содержимого. Для второго переопределения — первый массив для обмена его содержимого.

*right*<br/>
Для первого переопределения — второй объект для обмена его содержимого. Для второго переопределения — второй массив для обмена его содержимого.

### <a name="remarks"></a>Примечания

Первая перегрузка предназначена для работы с отдельными объектами. Вторая перегрузка меняет местами содержимое объектов в двух массивах.

### <a name="example"></a>Пример

```cpp
// alg_swap.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <iostream>

int main()
{
   using namespace std;
   vector <int> v1, v2;
   vector <int>::iterator Iter1, Iter2, result;

   for ( int i = 0 ; i <= 10 ; i++ )
   {
      v1.push_back( i );
   }

   for ( int ii = 0 ; ii <= 4 ; ii++ )
   {
      v2.push_back( 5 );
   }

   cout << "Vector v1 is ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   cout << "Vector v2 is ( " ;
   for ( Iter2 = v2.begin( ) ; Iter2 != v2.end( ) ; Iter2++ )
      cout << *Iter2 << " ";
   cout << ")." << endl;

   swap( v1, v2 );

   cout << "Vector v1 is ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   cout << "Vector v2 is ( " ;
   for ( Iter2 = v2.begin( ) ; Iter2 != v2.end( ) ; Iter2++ )
      cout << *Iter2 << " ";
   cout << ")." << endl;
}
```

```Output
Vector v1 is ( 0 1 2 3 4 5 6 7 8 9 10 ).
Vector v2 is ( 5 5 5 5 5 ).
Vector v1 is ( 5 5 5 5 5 ).
Vector v2 is ( 0 1 2 3 4 5 6 7 8 9 10 ).
```

## <a name="swap_ranges"></a>  swap_ranges

Меняет местами элементы одного диапазона с элементами другого диапазона такого же размера.

```cpp
template<class ForwardIterator1, class ForwardIterator2>
ForwardIterator2 swap_ranges(
   ForwardIterator1 first1,
   ForwardIterator1 last1,
   ForwardIterator2 first2 );

```

### <a name="parameters"></a>Параметры

*first1*<br/>
Прямой итератор, указывающий первую позицию первого диапазона элементов для обмена.

*last1*<br/>
Прямой итератор, указывающий позицию, следующую за последней позицией первого диапазона элементов для обмена.

*first2*<br/>
Прямой итератор, указывающий первую позицию второго диапазона элементов для обмена.

### <a name="return-value"></a>Возвращаемое значение

Прямой итератор, указывающий позицию, следующую за последней позицией второго диапазона элементов для обмена.

### <a name="remarks"></a>Примечания

Диапазоны, на которые указывают ссылки, должны быть допустимыми; все указатели должны поддерживать сброс ссылок; в каждой последовательности должна быть возможность достижения последнего положения с первого путем приращения. Второй диапазон должен достигать размеров первого диапазона.

Отношение сложности линейное *last1* - *first1* выполненных перестановок. Если переставляются элементы из контейнеров одного и того же типа, то должна использоваться функция-член `swap` из этого контейнера, так как функция-член обычно имеет постоянную сложность.

### <a name="example"></a>Пример

```cpp
// alg_swap_ranges.cpp
// compile with: /EHsc
#include <vector>
#include <deque>
#include <algorithm>
#include <iostream>

int main()
{
   using namespace std;
   vector <int> v1;
   deque <int> d1;
   vector <int>::iterator v1Iter1;
   deque<int>::iterator d1Iter1;

   int i;
   for ( i = 0 ; i <= 5 ; i++ )
   {
      v1.push_back( i );
   }

   int ii;
   for ( ii =4 ; ii <= 9 ; ii++ )
   {
      d1.push_back( 6 );
   }

   cout << "Vector v1 is ( " ;
   for ( v1Iter1 = v1.begin( ) ; v1Iter1 != v1.end( ) ;v1Iter1 ++ )
      cout << *v1Iter1  << " ";
   cout << ")." << endl;

   cout << "Deque d1 is  ( " ;
   for ( d1Iter1 = d1.begin( ) ; d1Iter1 != d1.end( ) ;d1Iter1 ++ )
      cout << *d1Iter1  << " ";
   cout << ")." << endl;

   swap_ranges ( v1.begin( ), v1.end( ), d1.begin( ) );

   cout << "After the swap_range, vector v1 is ( " ;
   for ( v1Iter1 = v1.begin( ) ; v1Iter1 != v1.end( ) ;v1Iter1 ++ )
      cout << *v1Iter1 << " ";
   cout << ")." << endl;

   cout << "After the swap_range deque d1 is   ( " ;
   for ( d1Iter1 = d1.begin( ) ; d1Iter1 != d1.end( ) ;d1Iter1 ++ )
      cout << *d1Iter1 << " ";
   cout << ")." << endl;
}
```

```Output
Vector v1 is ( 0 1 2 3 4 5 ).
Deque d1 is  ( 6 6 6 6 6 6 ).
After the swap_range, vector v1 is ( 6 6 6 6 6 6 ).
After the swap_range deque d1 is   ( 0 1 2 3 4 5 ).
```

## <a name="transform"></a>  transform

Применяет заданный объект функции к каждому элементу в исходном диапазоне или к паре элементов из двух исходных диапазонов и копирует возвращаемые значения объекта функции в диапазон назначения.

```cpp
template<class InputIterator, class OutputIterator, class UnaryFunction>
OutputIterator transform(
    InputIterator first1,
    InputIterator last1,
    OutputIterator result,
    UnaryFunction func );

template<class InputIterator1, class InputIterator2, class OutputIterator, class BinaryFunction>
OutputIterator transform(
    InputIterator1 first1,
    InputIterator1 last1,
    InputIterator2 first2,
    OutputIterator result,
    BinaryFunction func );
```

### <a name="parameters"></a>Параметры

*first1*<br/>
Итератор ввода указывает на позицию первого элемента в первом исходном обрабатываемом диапазоне.

*last1*<br/>
Итератор ввода указывает на позицию, следующую за последним элементом в первом исходном обрабатываемом диапазоне.

*first2*<br/>
Итератор ввода указывает на позицию первого элемента во втором исходном обрабатываемом диапазоне.

*результат*<br/>
Итератор вывода указывает на позицию первого элемента в диапазоне назначения.

*_Func*<br/>
Определенный пользователем объект унарной функции, используемый в первой версии алгоритма, который применяется к каждому элементу в первом исходном диапазоне, или определенный пользователем объект бинарной функции, используемый во второй версии алгоритма, который применяется попарно в прямом порядке к двум исходным диапазонам.

### <a name="return-value"></a>Возвращаемое значение

Итератор вывода указывает на позицию после последнего элемента в диапазоне назначения, который получает выходные элементы, преобразованные объектом функции.

### <a name="remarks"></a>Примечания

Диапазоны, на которые указывают ссылки, должны быть допустимыми; все указатели должны поддерживать сброс ссылок; в каждой последовательности должна быть возможность достижения последнего положения с первого путем приращения. Диапазон назначения должен быть достаточно большим, чтобы содержать преобразованный исходный диапазон.

Если *результат* приравнивается к *first1* в первой версии алгоритма, затем исходный и конечный диапазоны будут совпадать и последовательность будет изменена на месте. Но *результат* может не соответствовать положение в диапазоне [`first1` + 1, `last1`).

Отношение сложности линейное с не более (`last1` - `first1`) сравнений.

### <a name="example"></a>Пример

```cpp
// alg_transform.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <functional>
#include <iostream>

// The function object multiplies an element by a Factor
template <class Type>
class MultValue
{
   private:
      Type Factor;   // The value to multiply by
   public:
      // Constructor initializes the value to multiply by
      MultValue ( const Type& val ) : Factor ( val ) {
      }

      // The function call for the element to be multiplied
      Type operator( ) ( Type& elem ) const
      {
         return elem * Factor;
      }
};

int main()
{
   using namespace std;
   vector <int> v1, v2 ( 7 ), v3 ( 7 );
   vector <int>::iterator Iter1, Iter2 , Iter3;

   // Constructing vector v1
   int i;
   for ( i = -4 ; i <= 2 ; i++ )
   {
      v1.push_back(  i );
   }

   cout << "Original vector  v1 = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Modifying the vector v1 in place
   transform (v1.begin( ), v1.end( ), v1.begin( ), MultValue<int> ( 2 ) );
   cout << "The elements of the vector v1 multiplied by 2 in place gives:"
        << "\n v1mod = ( " ;
   for ( Iter1 = v1.begin( ) ; Iter1 != v1.end( ) ; Iter1++ )
      cout << *Iter1 << " ";
   cout << ")." << endl;

   // Using transform to multiply each element by a factor of 5
   transform ( v1.begin( ), v1.end( ), v2.begin( ), MultValue<int> ( 5 ) );

   cout << "Multiplying the elements of the vector v1mod\n "
        <<  "by the factor 5 & copying to v2 gives:\n v2 = ( " ;
   for ( Iter2 = v2.begin( ) ; Iter2 != v2.end( ) ; Iter2++ )
      cout << *Iter2 << " ";
   cout << ")." << endl;

   // The second version of transform used to multiply the
   // elements of the vectors v1mod & v2 pairwise
   transform ( v1.begin( ), v1.end( ),  v2.begin( ), v3.begin( ),
      multiplies <int>( ) );

   cout << "Multiplying elements of the vectors v1mod and v2 pairwise "
        <<  "gives:\n v3 = ( " ;
   for ( Iter3 = v3.begin( ) ; Iter3 != v3.end( ) ; Iter3++ )
      cout << *Iter3 << " ";
   cout << ")." << endl;
}
```

```Output
Original vector  v1 = ( -4 -3 -2 -1 0 1 2 ).
The elements of the vector v1 multiplied by 2 in place gives:
v1mod = ( -8 -6 -4 -2 0 2 4 ).
Multiplying the elements of the vector v1mod
by the factor 5 & copying to v2 gives:
v2 = ( -40 -30 -20 -10 0 10 20 ).
Multiplying elements of the vectors v1mod and v2 pairwise gives:
v3 = ( 320 180 80 20 0 20 80 ).
```

## <a name="unique"></a>  unique

Удаляет повторяющиеся элементы, расположенные в указанном диапазоне рядом друг с другом.

```cpp
template<class ForwardIterator>
   ForwardIterator unique(
      ForwardIterator first,
      ForwardIterator last);

template<class ForwardIterator, class Predicate>
   ForwardIterator unique(
      ForwardIterator first,
      ForwardIterator last,
      Predicate comp);

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Прямой итератор, указывающий позицию первого элемента в диапазоне, который должен проверяться для поиска и удаления дубликатов.

*последний*<br/>
Прямой итератор, указывающий позицию, следующую за последним элементом в диапазоне, который должен проверяться для поиска и удаления дубликатов.

*Зап.*<br/>
Заданный пользователем объект функции предиката, определяющий условие, которое должно выполняться, чтобы два элемента считались эквивалентными друг другу. Двоичный предикат принимает два аргумента и возвращает **true** , если условие удовлетворено, или **false** , если условие не удовлетворено.

### <a name="return-value"></a>Возвращаемое значение

Прямой итератор в новый конец измененной последовательности, которая не содержит последовательных дубликатов, указывающий позицию, следующую за последним неудаленным элементом.

### <a name="remarks"></a>Примечания

Обе формы алгоритма удаляют второй дубликат последовательной пары равных элементов.

Действие алгоритма стабильно, поэтому относительный порядок неудаленных элементов не изменяется.

Указанный диапазон должен быть допустимым. Все указатели должны поддерживать удаление ссылок, а последняя позиция в последовательности должна быть доступна из первой позиции за счет увеличения на один. число элементов в последовательности не изменяется алгоритмом `unique` и элементы за пределами измененной последовательности удаляются, но не указано.

Отношение сложности линейное; требуется (`last` - `first`) – 1 сравнений.

В классе list имеется более эффективная функция-член unique, которая может работать лучше.

Эти алгоритмы не могут использоваться в ассоциативном контейнере.

### <a name="example"></a>Пример

```cpp
// alg_unique.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <functional>
#include <iostream>
#include <ostream>

using namespace std;

// Return whether modulus of elem1 is equal to modulus of elem2
bool mod_equal ( int elem1, int elem2 )
{
   if ( elem1 < 0 )
      elem1 = - elem1;
   if ( elem2 < 0 )
      elem2 = - elem2;
   return elem1 == elem2;
};

int main()
{
   vector <int> v1;
   vector <int>::iterator v1_Iter1, v1_Iter2, v1_Iter3,
         v1_NewEnd1, v1_NewEnd2, v1_NewEnd3;

   int i;
   for ( i = 0 ; i <= 3 ; i++ )
   {
      v1.push_back( 5 );
      v1.push_back( -5 );
   }

   int ii;
   for ( ii = 0 ; ii <= 3 ; ii++ )
   {
      v1.push_back( 4 );
   }
   v1.push_back( 7 );

   cout << "Vector v1 is ( " ;
   for ( v1_Iter1 = v1.begin( ) ; v1_Iter1 != v1.end( ) ; v1_Iter1++ )
      cout << *v1_Iter1 << " ";
   cout << ")." << endl;

   // Remove consecutive duplicates
   v1_NewEnd1 = unique ( v1.begin( ), v1.end( ) );

   cout << "Removing adjacent duplicates from vector v1 gives\n ( " ;
   for ( v1_Iter1 = v1.begin( ) ; v1_Iter1 != v1_NewEnd1 ; v1_Iter1++ )
      cout << *v1_Iter1 << " ";
   cout << ")." << endl;

   // Remove consecutive duplicates under the binary prediate mod_equals
   v1_NewEnd2 = unique ( v1.begin( ), v1_NewEnd1 , mod_equal );

   cout << "Removing adjacent duplicates from vector v1 under the\n "
        << " binary predicate mod_equal gives\n ( " ;
   for ( v1_Iter2 = v1.begin( ) ; v1_Iter2 != v1_NewEnd2 ; v1_Iter2++ )
      cout << *v1_Iter2 << " ";
   cout << ")." << endl;

   // Remove elements if preceded by an element that was greater
   v1_NewEnd3 = unique ( v1.begin( ), v1_NewEnd2, greater<int>( ) );

   cout << "Removing adjacent elements satisfying the binary\n "
        << " predicate mod_equal from vector v1 gives ( " ;
   for ( v1_Iter3 = v1.begin( ) ; v1_Iter3 != v1_NewEnd3 ; v1_Iter3++ )
      cout << *v1_Iter3 << " ";
   cout << ")." << endl;
}
```

```Output
Vector v1 is ( 5 -5 5 -5 5 -5 5 -5 4 4 4 4 7 ).
Removing adjacent duplicates from vector v1 gives
( 5 -5 5 -5 5 -5 5 -5 4 7 ).
Removing adjacent duplicates from vector v1 under the
  binary predicate mod_equal gives
( 5 4 7 ).
Removing adjacent elements satisfying the binary
  predicate mod_equal from vector v1 gives ( 5 7 ).
```

## <a name="unique_copy"></a>  unique_copy

Копирует элементы из исходного диапазона в диапазон назначения за исключением повторяющихся элементов, расположенных рядом друг с другом.

```cpp
template<class InputIterator, class OutputIterator>
OutputIterator unique_copy( InputIterator first,
    InputIterator last,
    OutputIterator result );

template<class InputIterator, class OutputIterator, class BinaryPredicate>
OutputIterator unique_copy( InputIterator first,
    InputIterator last,
    OutputIterator result,
    BinaryPredicate comp );
```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Прямой итератор, указывающий на позицию первого элемента в исходном диапазоне для копирования.

*последний*<br/>
Прямой итератор, указывающий на позицию, следующую за последним элементом в исходном диапазоне для копирования.

*результат*<br/>
Выходной итератор, указывающий на позицию первого элемента в диапазоне назначения, получающем копию с последовательными удаленными дубликатами.

*Зап.*<br/>
Заданный пользователем объект функции предиката, определяющий условие, которое должно выполняться, чтобы два элемента считались эквивалентными друг другу. Двоичный предикат принимает два аргумента и возвращает **true** , если условие удовлетворено, или **false** , если условие не удовлетворено.

### <a name="return-value"></a>Возвращаемое значение

Выходной итератор, указывающий на позицию, следующую за последним элементом в диапазоне назначения, получающем копию с последовательными удаленными дубликатами.

### <a name="remarks"></a>Примечания

Обе формы алгоритма удаляют второй дубликат последовательной пары равных элементов.

Действие алгоритма стабильно, поэтому относительный порядок неудаленных элементов не изменяется.

Диапазоны, на которые указывают ссылки, должны быть допустимыми. Все указатели должны поддерживать сброс ссылок. В каждой последовательности должна быть возможность достижения последнего положения с первого путем приращения.

Отношение сложности линейное; требуется (`last` - `first`) сравнений.

### <a name="example"></a>Пример

```cpp
// alg_unique_copy.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <functional>
#include <iostream>
#include <ostream>

using namespace std;

// Return whether modulus of elem1 is equal to modulus of elem2
bool mod_equal ( int elem1, int elem2 ) {
   if ( elem1 < 0 )
      elem1 = - elem1;
   if ( elem2 < 0 )
      elem2 = - elem2;
   return elem1 == elem2;
};

int main() {
   vector <int> v1;
   vector <int>::iterator v1_Iter1, v1_Iter2,
         v1_NewEnd1, v1_NewEnd2;

   int i;
   for ( i = 0 ; i <= 1 ; i++ ) {
      v1.push_back( 5 );
      v1.push_back( -5 );
   }

   int ii;
   for ( ii = 0 ; ii <= 2 ; ii++ )
      v1.push_back( 4 );
   v1.push_back( 7 );

   int iii;
   for ( iii = 0 ; iii <= 5 ; iii++ )
      v1.push_back( 10 );

   cout << "Vector v1 is\n ( " ;
   for ( v1_Iter1 = v1.begin( ) ; v1_Iter1 != v1.end( ) ; v1_Iter1++ )
      cout << *v1_Iter1 << " ";
   cout << ")." << endl;

   // Copy first half to second, removing consecutive duplicates
   v1_NewEnd1 = unique_copy ( v1.begin( ), v1.begin( ) + 8, v1.begin( ) + 8 );

   cout << "Copying the first half of the vector to the second half\n "
        << "while removing adjacent duplicates gives\n ( " ;
   for ( v1_Iter1 = v1.begin( ) ; v1_Iter1 != v1_NewEnd1 ; v1_Iter1++ )
      cout << *v1_Iter1 << " ";
   cout << ")." << endl;

   int iv;
   for ( iv = 0 ; iv <= 7 ; iv++ )
      v1.push_back( 10 );

   // Remove consecutive duplicates under the binary prediate mod_equals
   v1_NewEnd2 = unique_copy ( v1.begin( ), v1.begin( ) + 14,
      v1.begin( ) + 14 , mod_equal );

   cout << "Copying the first half of the vector to the second half\n "
        << " removing adjacent duplicates under mod_equals gives\n ( " ;
   for ( v1_Iter2 = v1.begin( ) ; v1_Iter2 != v1_NewEnd2 ; v1_Iter2++ )
      cout << *v1_Iter2 << " ";
   cout << ")." << endl;
}
```

## <a name="upper_bound"></a>  upper_bound

Находит позицию первого элемента в упорядоченном диапазоне, который имеет значение больше указанного значения, где критерий упорядочивания может быть задан бинарным предикатом.

```cpp
template<class ForwardIterator, class Type>
   ForwardIterator upper_bound(
      ForwardIterator first,
      ForwardIterator last,
      const Type& value);

template<class ForwardIterator, class Type, class Predicate>
   ForwardIterator upper_bound(
      ForwardIterator first,
      ForwardIterator last,
      const Type& value,
      Predicate comp);

```

### <a name="parameters"></a>Параметры

*Первый*<br/>
Позиция первого элемента в диапазоне для поиска.

*последний*<br/>
Позиция, следующая за последним элементом в диапазоне для поиска.

*значение*<br/>
Значение в упорядоченном диапазоне, которое должно превышаться значением элемента, указанного возвращенным итератором.

*Зап.*<br/>
Определяемый пользователем объект функции предиката, задающий условие, когда один элемент меньше другого. Двоичный предикат принимает два аргумента и возвращает **true** , если условие удовлетворено, или **false** , если условие не удовлетворено.

### <a name="return-value"></a>Возвращаемое значение

Прямой итератор, указывающий позицию первого элемента со значением, превышающим указанное значение.

### <a name="remarks"></a>Примечания

Упорядоченный исходный диапазон, на который указывает ссылка, должен быть допустим. Все итераторы должны поддерживать отмену ссылок. В последовательности должна быть возможность достижения последней позиции с первой путем приращения.

Предварительным условием для использования `upper_bound` является упорядоченный диапазон, критерий упорядочения которого совпадает с заданным двоичным предикатом.

Диапазон не изменяется алгоритмом `upper_bound`.

В целях упорядочения типы значений прямых итераторов должны подлежать сравнению "меньше чем", чтобы при наличии двух элементов можно было определить, что они равны (т. е. ни один не меньше другого) или что один меньше другого. Это приводит к упорядочению неравнозначных элементов.

Сложность алгоритма является логарифмической для итераторов произвольного доступа и линейной в противном случае с числом шагов, пропорциональным значению (`last - first`).

### <a name="example"></a>Пример

```cpp
// alg_upper_bound.cpp
// compile with: /EHsc
#include <vector>
#include <algorithm>
#include <functional>      // greater<int>( )
#include <iostream>

// Return whether modulus of elem1 is less than modulus of elem2
bool mod_lesser( int elem1, int elem2 )
{
    if ( elem1 < 0 )
        elem1 = - elem1;
    if ( elem2 < 0 )
        elem2 = - elem2;
    return elem1 < elem2;
}

int main()
{
    using namespace std;

    vector<int> v1;
    // Constructing vector v1 with default less-than ordering
    for ( auto i = -1 ; i <= 4 ; ++i )
    {
        v1.push_back(  i );
    }

    for ( auto ii =-3 ; ii <= 0 ; ++ii )
    {
        v1.push_back(  ii  );
    }

    cout << "Starting vector v1 = ( " ;
    for (const auto &Iter : v1)
        cout << Iter << " ";
    cout << ")." << endl;

    sort(v1.begin(), v1.end());
    cout << "Original vector v1 with range sorted by the\n "
        << "binary predicate less than is v1 = ( " ;
    for (const auto &Iter : v1)
        cout << Iter << " ";
    cout << ")." << endl;

    // Constructing vector v2 with range sorted by greater
    vector<int> v2(v1);

    sort(v2.begin(), v2.end(), greater<int>());

    cout << "Original vector v2 with range sorted by the\n "
        << "binary predicate greater is v2 = ( " ;
    for (const auto &Iter : v2)
        cout << Iter << " ";
    cout << ")." << endl;

    // Constructing vectors v3 with range sorted by mod_lesser
    vector<int> v3(v1);
    sort(v3.begin(), v3.end(), mod_lesser);

    cout << "Original vector v3 with range sorted by the\n "
        <<  "binary predicate mod_lesser is v3 = ( " ;
    for (const auto &Iter : v3)
        cout << Iter << " ";
    cout << ")." << endl;

    // Demonstrate upper_bound

    vector<int>::iterator Result;

    // upper_bound of 3 in v1 with default binary predicate less<int>()
    Result = upper_bound(v1.begin(), v1.end(), 3);
    cout << "The upper_bound in v1 for the element with a value of 3 is: "
        << *Result << "." << endl;

    // upper_bound of 3 in v2 with the binary predicate greater<int>( )
    Result = upper_bound(v2.begin(), v2.end(), 3, greater<int>());
    cout << "The upper_bound in v2 for the element with a value of 3 is: "
        << *Result << "." << endl;

    // upper_bound of 3 in v3 with the binary predicate  mod_lesser
    Result = upper_bound(v3.begin(), v3.end(), 3,  mod_lesser);
    cout << "The upper_bound in v3 for the element with a value of 3 is: "
        << *Result << "." << endl;
}

```

## <a name="see-also"></a>См. также

[\<algorithm>](../standard-library/algorithm.md)<br/>