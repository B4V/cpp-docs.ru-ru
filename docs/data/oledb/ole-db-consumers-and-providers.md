---
title: Получатели и поставщики | Документация Майкрософт
ms.custom: ''
ms.date: 10/22/2018
ms.technology:
- cpp-data
ms.topic: reference
dev_langs:
- C++
helpviewer_keywords:
- OLE DB providers, OLE DB data architecture
- OLE DB providers
- OLE DB consumers, OLE DB data architecture
- OLE DB consumers
- OLE DB, data model
ms.assetid: 886cb39d-652b-4557-93f0-4b1b0754d8bc
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
- data-storage
ms.openlocfilehash: 4f52177e5fcb34470e606497297985d805a151f6
ms.sourcegitcommit: a9dcbcc85b4c28eed280d8e451c494a00d8c4c25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2018
ms.locfileid: "50077599"
---
# <a name="ole-db-consumers-and-providers"></a>Получатели и поставщики OLE DB

В архитектуре OLE DB используется модель получателей и поставщиков. Потребитель выполняет запросы к данным. Поставщик отвечает на эти запросы, размещая данные в табличном формате и их возвращение в потребитель. Любой вызов, объекта-получателя должен быть реализован в поставщике.

С технической точки зрения, объект-получатель является любой системе или приложении код (не обязательно компонент OLE DB), обращается к данным через интерфейсы OLE DB. Интерфейсы реализуются в поставщике. Поэтому поставщик — любой программный компонент, который реализует интерфейсы OLE DB для инкапсуляции доступа к данным и предоставить его другим объектам (то есть, потребители).

Для ролей потребитель вызывает методы в интерфейсах OLE DB; Поставщик OLE DB реализует необходимые интерфейсы OLE DB.

OLE DB позволяет избежать условия клиентом и сервером, так как эти роли не всегда имеет смысл, особенно в n уровневых ситуации. Поскольку объект-получатель может быть компонент на уровне, обслуживающем другой компонент, для его вызова клиент может вызвать путаницу. Кроме того поставщик иногда более действует как драйвер базы данных, чем сервер.

## <a name="see-also"></a>См. также

[Программирование объектов OLE DB](../../data/oledb/ole-db-programming.md)<br/>
[Общие сведения о программировании OLE DB](../../data/oledb/ole-db-programming-overview.md)