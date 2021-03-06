---
title: _fcvt | Документы Майкрософт
ms.custom: ''
ms.date: 04/05/2018
ms.technology:
- cpp-standard-libraries
ms.topic: reference
apiname:
- _fcvt
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
- ucrtbase.dll
- api-ms-win-crt-convert-l1-1-0.dll
apitype: DLLExport
f1_keywords:
- _fcvt
dev_langs:
- C++
helpviewer_keywords:
- converting floating point, to strings
- _fcvt function
- floating-point functions, converting number to string
- fcvt function
- floating-point functions
ms.assetid: 74584c88-f0dd-4907-8fca-52da5df583f5
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 272b8e4ba5e57d71b4b785bceef7e5ea2f0ac7c2
ms.sourcegitcommit: 6e3cf8df676d59119ce88bf5321d063cf479108c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2018
ms.locfileid: "34450424"
---
# <a name="fcvt"></a>_fcvt

Преобразует число с плавающей запятой в строку. Существует более безопасная версия этой функции, см. раздел [_fcvt_s](fcvt-s.md).

## <a name="syntax"></a>Синтаксис

```C
char *_fcvt(
   double value,
   int count,
   int *dec,
   int *sign
);
```

### <a name="parameters"></a>Параметры

*значение*<br/>
Число, которое требуется преобразовать.

*count*<br/>
Число разрядов после десятичной запятой.

*dec*<br/>
Указатель на сохраненную позицию десятичной запятой.

*sign*<br/>
Указатель на сохраненный индикатор знака.

## <a name="return-value"></a>Возвращаемое значение

**_fcvt** возвращает указатель на строку десятичных разрядов, **NULL** при возникновении ошибки.

## <a name="remarks"></a>Примечания

**_Fcvt** функция преобразует число с плавающей запятой в строку, завершающуюся значением null. *Значение* представляет собой число с плавающей запятой для преобразования. **_fcvt** сохраняет цифры параметра *значение* как строка и добавляет символ null («\0»). *Число* указывает количество цифр, сохраняемых после десятичной запятой. Избыточные цифры округляются до *число* помещает. Если доступно менее *число* значащих цифр, строка дополняется нулями.

Общее количество цифр, возвращенных **_fcvt** не может превышать **_CVTBUFSIZE**.

В строке сохраняются только цифры. Положение десятичной запятой и знак *значение* можно получить из *dec* и входа после вызова метода. *Dec* указывает на целочисленное значение; это целочисленное значение представляет положение десятичной запятой относительно начала строки. Ноль или отрицательное целое число означают, что десятичная запятая располагается слева от первой цифры. Параметр *входа* указывает на целое число, указывающее знак *значение*. Целое число имеет значение 0, если *значение* имеет положительное значение и задайте ненулевое значение, если *значение* является отрицательным значением.

Разница между **_ecvt** и **_fcvt** заключается в интерпретации из *число* параметра. **_ecvt** интерпретирует *число* как общее число цифр в выходной строке, в то время как **_fcvt** интерпретирует *число* как количество цифр после десятичной запятой.

**_ecvt** и **_fcvt** используют для преобразования один статически выделенный буфер. Каждый вызов одной из этих подпрограмм уничтожает результат предыдущего вызова.

Эта функция проверяет свои параметры. Если *dec* или *входа* — **NULL**, или *число* равно 0, вызывается обработчик недопустимого параметра, как описано в [параметр Проверка](../../c-runtime-library/parameter-validation.md). Если выполнение может быть продолжено, **errno** равно **EINVAL** и **NULL** возвращается.

## <a name="requirements"></a>Требования

|Функция|Обязательный заголовок|
|--------------|---------------------|
|**_fcvt**|\<stdlib.h>|

Дополнительные сведения о совместимости см. в разделе [Совместимость](../../c-runtime-library/compatibility.md).

## <a name="example"></a>Пример

```C
// crt_fcvt.c
// compile with: /W3
// This program converts the constant
// 3.1415926535 to a string and sets the pointer
// buffer to point to that string.

#include <stdlib.h>
#include <stdio.h>

int main( void )
{
   int  decimal, sign;
   char *buffer;
   double source = 3.1415926535;

   buffer = _fcvt( source, 7, &decimal, &sign ); // C4996
   // Note: _fcvt is deprecated; consider using _fcvt_s instead
   printf( "source: %2.10f   buffer: '%s'   decimal: %d   sign: %d\n",
            source, buffer, decimal, sign );
}
```

```Output
source: 3.1415926535   buffer: '31415927'   decimal: 1   sign: 0
```

## <a name="see-also"></a>См. также

[Преобразование данных](../../c-runtime-library/data-conversion.md)<br/>
[Поддержка чисел с плавающей запятой](../../c-runtime-library/floating-point-support.md)<br/>
[atof, _atof_l, _wtof, _wtof_l](atof-atof-l-wtof-wtof-l.md)<br/>
[_ecvt](ecvt.md)<br/>
[_gcvt](gcvt.md)<br/>
