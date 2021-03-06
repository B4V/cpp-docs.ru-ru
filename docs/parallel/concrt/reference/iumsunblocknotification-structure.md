---
title: Структура IUMSUnblockNotification | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-concrt
ms.topic: reference
f1_keywords:
- IUMSUnblockNotification
- CONCRTRM/concurrency::IUMSUnblockNotification
- CONCRTRM/concurrency::IUMSUnblockNotification::IUMSUnblockNotification::GetContext
- CONCRTRM/concurrency::IUMSUnblockNotification::IUMSUnblockNotification::GetNextUnblockNotification
dev_langs:
- C++
helpviewer_keywords:
- IUMSUnblockNotification structure
ms.assetid: eaca9529-c1cc-472b-8ec6-722a1ff0fa2a
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 63dcd78af0804a6921d34a35611591f044c2633f
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46438032"
---
# <a name="iumsunblocknotification-structure"></a>Структура IUMSUnblockNotification

Представляет уведомление диспетчера ресурсов о том, что прокси-поток, который заблокировал и запустил возврат к заданному контексту планирования планировщика, разблокирован и готов для планирования. Этот интерфейс является недопустимым, когда связанный с прокси-потоком контекст выполнения, возвращенный из метода `GetContext`, переносится.

## <a name="syntax"></a>Синтаксис

```
struct IUMSUnblockNotification;
```

## <a name="members"></a>Участники

### <a name="public-methods"></a>Открытые методы

|Имя|Описание|
|----------|-----------------|
|[IUMSUnblockNotification::GetContext](#getcontext)|Возвращает `IExecutionContext` интерфейс для контекста выполнения, связанного с прокси-поток, который был разблокирован. Когда этот метод возвращает, базовый контекст выполнения будет повторно запущено через вызов `IThreadProxy::SwitchTo` метод, этот интерфейс больше не является допустимым.|
|[IUMSUnblockNotification::GetNextUnblockNotification](#getnextunblocknotification)|Возвращает следующий `IUMSUnblockNotification` интерфейс в цепочке, возвращенный методом `IUMSCompletionList::GetUnblockNotifications`.|

## <a name="inheritance-hierarchy"></a>Иерархия наследования

`IUMSUnblockNotification`

## <a name="requirements"></a>Требования

**Заголовок:** concrtrm.h

**Пространство имен:** concurrency

##  <a name="getcontext"></a>  Метод IUMSUnblockNotification::GetContext

Возвращает `IExecutionContext` интерфейс для контекста выполнения, связанного с прокси-поток, который был разблокирован. Когда этот метод возвращает, базовый контекст выполнения будет повторно запущено через вызов `IThreadProxy::SwitchTo` метод, этот интерфейс больше не является допустимым.

```
virtual IExecutionContext* GetContext() = 0;
```

### <a name="return-value"></a>Возвращаемое значение

`IExecutionContext` Интерфейс для контекста выполнения для прокси-поток, который был разблокирован.

##  <a name="getnextunblocknotification"></a>  Метод IUMSUnblockNotification::GetNextUnblockNotification

Возвращает следующий `IUMSUnblockNotification` интерфейс в цепочке, возвращенный методом `IUMSCompletionList::GetUnblockNotifications`.

```
virtual IUMSUnblockNotification* GetNextUnblockNotification() = 0;
```

### <a name="return-value"></a>Возвращаемое значение

Следующий `IUMSUnblockNotification` интерфейс в цепочке, возвращенный методом `IUMSCompletionList::GetUnblockNotifications`.

## <a name="see-also"></a>См. также

[Пространство имен concurrency](concurrency-namespace.md)<br/>
[Структура IUMSScheduler](iumsscheduler-structure.md)<br/>
[Структура IUMSCompletionList](iumscompletionlist-structure.md)
