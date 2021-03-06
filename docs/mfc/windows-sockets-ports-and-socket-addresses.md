---
title: 'Сокеты Windows: Порты и адреса сокета | Документация Майкрософт'
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-mfc
ms.topic: conceptual
dev_langs:
- C++
helpviewer_keywords:
- ports [MFC], definition
- Windows Sockets [MFC], ports
- Windows Sockets [MFC], addresses
- ports [MFC]
- addresses [MFC], socket
- sockets [MFC], addresses
- sockets [MFC], ports
ms.assetid: e050261a-9285-4f31-a1c5-6c8033af5b4a
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 7f97bfa42e379f0806eb85e3f030465b2a181d01
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46379673"
---
# <a name="windows-sockets-ports-and-socket-addresses"></a>Сокеты Windows. Порты и адреса сокета

Здесь объясняются термины «порт» и «адрес», как используемого с помощью сокетов Windows.

##  <a name="_core_port"></a> Порт

Порт определяет уникальный процесс, для которого может предоставляться услуга. В контексте присутствует порт связан с приложение, поддерживающее Windows Sockets. Идея состоит в том, для уникальной идентификации каждого приложения Windows Sockets, тем самым давая возможность более чем одним приложением Windows Sockets, работающей на машине, в то же время.

Определенные порты, зарезервированы для распространенных служб, таких как FTP. Следует избегать использования этих портов, если вы предоставляете такого рода службы. В спецификации Windows Sockets подробно эти резервные порты. Файл WINSOCK. H также перечислены их.

Чтобы библиотеки DLL Windows Sockets выберите порт может использоваться для, передайте 0 в качестве значения порта. MFC выбирает значение порта больше 1024 decimal. Можно получить номер порта, выбранное в MFC, вызвав [CAsyncSocket::GetSockName](../mfc/reference/casyncsocket-class.md#getsockname) функция-член.

##  <a name="_core_socket_address"></a> Адрес сокета

Каждый объект сокета связан с адресом протокола Интернета (IP) в сети. Как правило адрес — это имя компьютера, например «ftp.microsoft.com», или точками номер, например «128.56.22.8».

При выполнении поиска создать сокет, обычно не нужно указать свой адрес.

> [!NOTE]
>  Возможно, что компьютер имеет несколько сетевых карт (или когда-нибудь может выполняться приложение такому компьютеру), каждый из которых представляет другую сеть. Если это так, может потребоваться предоставить адрес, чтобы указать, какой сетевой карты, сокет будет использовать. Это быть расширенное использование и проблема возможных переносимости.

Дополнительные сведения:

- [Сокеты Windows. Использование класса CAsyncSocket](../mfc/windows-sockets-using-class-casyncsocket.md)

- [Сокеты Windows. Использование сокетов с архивами](../mfc/windows-sockets-using-sockets-with-archives.md)

- [Сокеты Windows. Работа сокетов с архивами](../mfc/windows-sockets-how-sockets-with-archives-work.md)

- [Сокеты Windows. Сокеты потоков](../mfc/windows-sockets-stream-sockets.md)

- [Сокеты Windows. Сокеты датаграмм](../mfc/windows-sockets-datagram-sockets.md)

## <a name="see-also"></a>См. также

[Сокеты Windows в MFC](../mfc/windows-sockets-in-mfc.md)

