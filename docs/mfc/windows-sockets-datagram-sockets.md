---
title: Сокеты Windows. сокеты датаграмм | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-mfc
ms.topic: conceptual
dev_langs:
- C++
helpviewer_keywords:
- sockets [MFC], datagram
- Windows Sockets [MFC], bi-directional data flow
- datagram sockets [MFC]
- Windows Sockets [MFC], datagram
- sockets [MFC], bi-directional data flow
ms.assetid: bec16a1c-74c0-4ff9-8c18-c2d87897d264
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 7a63caa786ce5198fb902b8d48101507fb2b4113
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46444220"
---
# <a name="windows-sockets-datagram-sockets"></a>Сокеты Windows. Сокеты датаграмм

В этой статье описывается сокеты датаграмм, один из двух типов сокетов Windows, которые доступны. (Другой тип — [сокета потока](../mfc/windows-sockets-stream-sockets.md).)

Сокеты датаграмм поддерживают двунаправленный поток данных, который не обязательно быть виртуализации или неповторяющиеся. Также датаграммы не гарантируется надежность; они не поступают. Данные датаграммы могут поступать не по порядку и возможно повторяющиеся, но записей границ в данных, сохраняются до тех пор, пока будут меньше, чем размер внутреннего получателя записи. Вы несете ответственность за управление виртуализации и надежности. (Надежность имеет тенденцию быть хорошо на локальной сети [локальной сети], но меньше и т. д. глобальной сети [глобальной сети], например в Интернете.)

Датаграммы являются «без установления соединения», то есть без явного подключения; передать сообщение датаграммы указанного сокета и сообщения с указанного сокета.

Пример сокета датаграмм — это приложение, в которой хранится системные часы на сети. Это иллюстрирует это дополнительная функция. сокеты датаграмм в по крайней мере некоторые параметры: широковещательная рассылка сообщений по большое количество сетевых адресов.

Сокеты датаграмм работают лучше, чем сокеты потока для данных, ориентированные на запись. Дополнительные сведения о сокеты датаграмм см. в спецификации Windows Sockets, доступных в пакете SDK для Windows.

## <a name="see-also"></a>См. также

[Сокеты Windows в MFC](../mfc/windows-sockets-in-mfc.md)<br/>
[Сокеты Windows. Фон](../mfc/windows-sockets-background.md)

