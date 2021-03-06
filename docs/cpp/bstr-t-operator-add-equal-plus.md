---
title: _bstr_t::operator += + | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-language
ms.topic: language-reference
f1_keywords:
- _bstr_t::operator+
- _bstr_t::operator+=
dev_langs:
- C++
helpviewer_keywords:
- += operator [C++], appending strings
- + operator [C++], _bstr_t objects
ms.assetid: d28316ce-c2c8-4a38-bdb3-44fa4e582c44
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: a440e8b8d078c7849de2a0b29f1d50b140d70070
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46044773"
---
# <a name="bstrtoperator--"></a>_bstr_t::operator +=, +

**Блок, относящийся только к системам Microsoft**

Добавляет символы в конец объекта `_bstr_t` или объединяет две строки.

## <a name="syntax"></a>Синтаксис

```
_bstr_t& operator+=( const _bstr_t& s1 );
_bstr_t operator+( const _bstr_t& s1 );
friend _bstr_t operator+( const char* s2, const _bstr_t& s1);
friend _bstr_t operator+( const wchar_t* s3, const _bstr_t& s1);
```

#### <a name="parameters"></a>Параметры

*s1*<br/>
Объект `_bstr_t`.

*s2*<br/>
Многобайтовая строка.

*S3*<br/>
Строка Юникода.

## <a name="remarks"></a>Примечания

Эти операторы выполняют объединение строк:

- **оператор += (***s1***)** добавляет символы из инкапсулированного `BSTR` из *s1* в конец этого объекта инкапсулированный `BSTR`.

- **оператор + (***s1***)** возврат нового `_bstr_t` , образуется путем объединения этого объекта `BSTR` с данными о *s1*.

- **оператор + (***s2***&#124;***s1***)** возвращает новый `_bstr_t` , образуется путем объединения Многобайтовая строка *s2*, преобразованной в Юникод, с помощью `BSTR` инкапсулирован в *s1*.

- **оператор + (***s3* **,***s1***)** возвращает новый `_bstr_t` который образуется путем объединения строки Юникод *s3* с `BSTR` инкапсулирован в *s1*.

**Завершение блока, относящегося только к системам Майкрософт**

## <a name="see-also"></a>См. также

[_bstr_t Class](../cpp/bstr-t-class.md)