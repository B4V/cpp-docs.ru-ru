---
title: qsort | Документы Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-standard-libraries
ms.topic: reference
apiname:
- qsort
apilocation:
- msvcrt.dll
- msvcr80.dll
- msvcr90.dll
- msvcr100.dll
- msvcr100_clr0400.dll
- msvcr110.dll
- msvcr110_clr0400.dll
- msvcr120.dll
- msvcr120_clr0400.dll
- ntdll.dll
- ucrtbase.dll
- api-ms-win-crt-utility-l1-1-0.dll
apitype: DLLExport
f1_keywords:
- qsort
dev_langs:
- C++
helpviewer_keywords:
- qsort function
- quick-sort algorithm
- sorting arrays
- arrays [CRT], sorting
ms.assetid: d6cb33eb-d209-485f-8d41-229eb743c027
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 87e9ba6ef9bcb4a909e97466d7ea71ee18374991
ms.sourcegitcommit: 761c5f7c506915f5a62ef3847714f43e9b815352
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2018
ms.locfileid: "44110205"
---
# <a name="qsort"></a>qsort

Выполняет быструю сортировку. Существует более безопасная версия этой функции, см. раздел [qsort_s](qsort-s.md).

## <a name="syntax"></a>Синтаксис

```C
void qsort(
   void *base,
   size_t num,
   size_t width,
   int (__cdecl *compare )(const void *, const void *)
);
```

### <a name="parameters"></a>Параметры

<br/>
Начало целевого массива.

*номер*<br/>
Размер массива в элементах.

*width*<br/>
Размер элементов в байтах.

*compare*<br/>
Указатель на пользовательскую подпрограмму, которая сравнивает два элемента массива и возвращает значение, показывающее, как соотносятся их значения.

## <a name="remarks"></a>Примечания

**Qsort** функция реализует алгоритм быстрой сортировки для сортировки массива *номер* элементов, каждый из которых *ширины* байт. Аргумент *базового* является указателем на базовый массив был отсортирован. **qsort** перезаписывает этот массив с использованием отсортированных элементов.

**qsort** вызовы *сравнения* рутинных один или несколько раз во время сортировки и передает указатели на два элемента массива при каждом вызове.

```C
compare( (void *) & elem1, (void *) & elem2 );
```

Подпрограмма сравнивает элементы и возвращает одно из следующих значений.

|Сравнение возвращаемого значения функции|Описание|
|-----------------------------------|-----------------|
|< 0|**elem1** меньше, чем **elem2**|
|0|**elem1** эквивалентно **elem2**|
|> 0|**elem1** больше, чем **elem2**|

Массив сортируется по возрастанию, как определено функцией сравнения. Для сортировки массива по убыванию измените смысл значений "больше" и "меньше" на противоположный в функции сравнения.

Эта функция проверяет свои параметры. Если *сравнения* или *номер* — **NULL**, или если *базового* — **NULL** и **номер* не равно нулю, или если *ширины* меньше нуля, вызывается обработчик недопустимого параметра, как описано в разделе [проверка параметров](../../c-runtime-library/parameter-validation.md). Если выполнение может быть продолжено, функция возвращает и **errno** присваивается **EINVAL**.

## <a name="requirements"></a>Требования

|Подпрограмма|Обязательный заголовок|
|-------------|---------------------|
|**qsort**|\<stdlib.h> и \<search.h>|

Дополнительные сведения о совместимости см. в разделе [Совместимость](../../c-runtime-library/compatibility.md).

## <a name="example"></a>Пример

```C
// crt_qsort.c
// arguments: every good boy deserves favor

/* This program reads the command-line
* parameters and uses qsort to sort them. It
* then displays the sorted arguments.
*/

#include <stdlib.h>
#include <string.h>
#include <stdio.h>

int compare( const void *arg1, const void *arg2 );

int main( int argc, char **argv )
{
   int i;
   /* Eliminate argv[0] from sort: */
   argv++;
   argc--;

   /* Sort remaining args using Quicksort algorithm: */
   qsort( (void *)argv, (size_t)argc, sizeof( char * ), compare );

   /* Output sorted list: */
   for( i = 0; i < argc; ++i )
      printf( " %s", argv[i] );
   printf( "\n" );
}

int compare( const void *arg1, const void *arg2 )
{
   /* Compare all of both strings: */
   return _stricmp( * ( char** ) arg1, * ( char** ) arg2 );
}
```

```Output
boy deserves every favor good
```

## <a name="see-also"></a>См. также

[Сортировка и поиск](../../c-runtime-library/searching-and-sorting.md)<br/>
[bsearch](bsearch.md)<br/>
[_lsearch](lsearch.md)<br/>
