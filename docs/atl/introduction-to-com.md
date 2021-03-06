---
title: Введение в модель COM | Документация Майкрософт
ms.custom: index-page
ms.date: 11/04/2016
ms.technology:
- cpp-atl
ms.topic: conceptual
dev_langs:
- C++
helpviewer_keywords:
- COM
ms.assetid: 120735d9-db71-4ad3-a730-ce576ea2354e
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: a98c7bb473e36e53e8cbe0f90f9dd94f655392d6
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46073230"
---
# <a name="introduction-to-com"></a>Введение в модель COM

COM является фундаментальным «объектную модель» на какие элементы управления ActiveX и OLE. COM позволяет объекту предоставлять свою функциональность другим компонентам и ведущим приложениям. Он определяет, как работает этот раскрытия, процессов и в разных сетях и как объект предоставляет сам. Модель COM также определяет жизненный цикл объекта.

Основа для COM — эти понятия:

- [Интерфейсы](../atl/interfaces-atl.md) — механизм, через который объект предоставляет свои функции.

- [IUnknown](../atl/iunknown.md) — базовый интерфейс, на котором основаны все остальные. Он реализует пересчет ссылок и интерфейс запроса механизмы обработки с помощью COM.

- [Подсчет ссылок](../atl/reference-counting.md) — метод, по которому объект (или, строго говоря, интерфейс) решает, когда больше не используется и поэтому предоставляется бесплатно удалить себя.

- [QueryInterface](../atl/queryinterface.md) — метод, используемый для запроса объектов для заданного интерфейса.

- [Маршалинг](../atl/marshaling.md) — механизм, позволяющий объектов, которое будет использоваться в поток, процессов и границы сети, что обеспечивает независимость от местонахождения.

- [Агрегирование](../atl/aggregation.md) — использовать другой метод, в которой один объект.

## <a name="see-also"></a>См. также

[Введение в модель COM и ATL](../atl/introduction-to-com-and-atl.md)<br/>
[Модель COM](/windows/desktop/com/the-component-object-model)

