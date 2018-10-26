---
title: __vmx_vmread | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-tools
ms.topic: reference
f1_keywords:
- __vmx_vmread
dev_langs:
- C++
helpviewer_keywords:
- VMREAD instruction
- __vmx_vmread intrinsic
ms.assetid: 08bdd7a0-6435-4ea6-b9a0-f592d870e5aa
author: corob-msft
ms.author: corob
ms.workload:
- cplusplus
ms.openlocfilehash: 0d9483dafd763112f31f5299a5e0e7e54c224459
ms.sourcegitcommit: a738519aa491a493a8f213971354356c0e6a5f3a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/05/2018
ms.locfileid: "48821027"
---
# <a name="vmxvmread"></a>__vmx_vmread

**Блок, относящийся только к системам Microsoft**

Считывает указанное поле из текущую структуру управления виртуальной машины (VMCS) и помещает его в указанном расположении.

## <a name="syntax"></a>Синтаксис

```
unsigned char __vmx_vmread(
   size_t Field,
   size_t *FieldValue
);
```

#### <a name="parameters"></a>Параметры

|Параметр|Описание:|
|---------------|-----------------|
|*Поле*|[in] Поле VMCS для чтения.|
|*FieldValue*|[in] Указатель на расположение для хранения значения чтения из VMCS поле, указанное параметром `Field` параметр.|

## <a name="return-value"></a>Возвращаемое значение

|Значение|Смысл|
|-----------|-------------|
|0|Операция успешно выполнена.|
|1|Не удалось выполнить операцию; расширенные сведения о состоянии доступны в `VM-instruction error field` текущей структуре VMCS.|
|2|Сбой операции без сведений о состоянии.|

## <a name="remarks"></a>Примечания

`__vmx_vmread` Функция эквивалентна `VMREAD` инструкции компьютера. Значение `Field` параметр является индекс кодировке поля, который описан в документации Intel. Дополнительные сведения в документе «Intel Virtualization технические спецификации для архитектуры IA-32 Intel,» номер документа C97063-002, на [корпорации Intel](https://software.intel.com/articles/intel-sdm) сайта, а затем см. в приложении С этим документом .

## <a name="requirements"></a>Требования

|Встроенная функция|Архитектура|
|---------------|------------------|
|`__vmx_vmread`|X64|

**Файл заголовка** \<intrin.h >

**Завершение блока, относящегося только к системам Майкрософт**

## <a name="see-also"></a>См. также

[Встроенные инструкции компилятора](../intrinsics/compiler-intrinsics.md)<br/>
[__vmx_vmwrite](../intrinsics/vmx-vmwrite.md)