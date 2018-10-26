---
title: Источники данных и сеансы | Документация Майкрософт
ms.custom: ''
ms.date: 10/22/2018
ms.technology:
- cpp-data
ms.topic: reference
dev_langs:
- C++
helpviewer_keywords:
- data sources [C++], OLE DB
- connections [C++], data source
- OLE DB consumer templates [C++], data sources
ms.assetid: 6ee52216-e082-4869-a1d6-ce561cfb76e5
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
- data-storage
ms.openlocfilehash: 0a6cb4e27f8a248b0b90454acb782b3b8994abc4
ms.sourcegitcommit: a9dcbcc85b4c28eed280d8e451c494a00d8c4c25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2018
ms.locfileid: "50056039"
---
# <a name="data-sources-and-sessions"></a>Источники данных и сеансы

На следующем рисунке показана классы, поддерживающие подключение и доступ к источнику данных. Каждый класс основан на реализации стандартного компонента OLE DB.

![Данные источника и классы сеансов](../../data/oledb/media/vcdatasourcesessionclasses.gif "vcdatasourcesessionclasses") источник данных и классы сеансов

Ниже приведены классы:

- [CDataSource](../../data/oledb/cdatasource-class.md) этот класс создает экземпляр объекта источника данных, который создает и управляет подключением к источнику данных через поставщик OLE DB. Источник данных принимает сведения, такие как данные исходного адреса и данные проверки подлинности в виде строки подключения.

   Также стоит отметить, что вспомогательный класс [CEnumerator](../../data/oledb/cenumerator-class.md) часто используется перед установкой любого соединения для получения списка поставщиков, зарегистрированных в системе. Это позволяет выбрать поставщика в качестве источника данных. Например **свойства канала передачи данных** этот класс используется диалоговое окно для заполнения списка поставщиков на **поставщики** вкладки. Он соответствует `SQLBrowseConnect` или `SQLDriverConnect` функции.

- [CSession](../../data/oledb/csession-class.md) этот класс создает объект сеанса, который представляет сеанс единого доступа к источнику данных. Тем не менее можно создать несколько сеансов на источнике данных. Для каждого сеанса можно создать наборы строк, команды и другие объекты, для доступа к данным из источника данных. Сеанс обрабатывает транзакции.

## <a name="see-also"></a>См. также

[Шаблоны потребителей OLE DB](../../data/oledb/ole-db-consumer-templates-cpp.md)