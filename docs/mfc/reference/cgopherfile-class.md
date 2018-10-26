---
title: Класс CGopherFile | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-mfc
ms.topic: reference
f1_keywords:
- CGopherFile
- AFXINET/CGopherFile
- AFXINET/CGopherFile::CGopherFile
dev_langs:
- C++
helpviewer_keywords:
- CGopherFile [MFC], CGopherFile
ms.assetid: 3ca9898f-8cdb-4495-bbde-46d40100feda
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 083ed824ce8586295e398d32ed14e17f8d334358
ms.sourcegitcommit: a9dcbcc85b4c28eed280d8e451c494a00d8c4c25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2018
ms.locfileid: "50080953"
---
# <a name="cgopherfile-class"></a>Класс CGopherFile

Обеспечивает возможность поиска и чтения файлов на сервере gopher.

> [!NOTE]
>  Классы `CGopherConnection`, `CGopherFile`, `CGopherFileFind`, `CGopherLocator` и их члены являются устаревшими, так как они не работают на платформе Windows XP, но они будут продолжать работать на более ранние платформы.

## <a name="syntax"></a>Синтаксис

```
class CGopherFile : public CInternetFile
```

## <a name="members"></a>Участники

### <a name="protected-constructors"></a>Защищенные конструкторы

|Имя|Описание|
|----------|-----------------|
|[CGopherFile::CGopherFile](#cgopherfile)|Создает объект `CGopherFile`.|

## <a name="remarks"></a>Примечания

Эта служба gopher разрешает пользователям записывать данные в файл gopher, так как эта служба работает главным образом как интерфейс на основе меню для поиска сведений. `CGopherFile` Функции-члены `Write`, `WriteString`, и `Flush` не реализованы для `CGopherFile`. Вызов этих функций для `CGopherFile` объекта возвращает [CNotSupportedException](../../mfc/reference/cnotsupportedexception-class.md).

Дополнительные сведения о том, как `CGopherFile` работает с другими классами MFC Интернет, см. в статье [Internet программирование с использованием WinInet](../../mfc/win32-internet-extensions-wininet.md).

## <a name="inheritance-hierarchy"></a>Иерархия наследования

[CObject](../../mfc/reference/cobject-class.md)

[CFile](../../mfc/reference/cfile-class.md)

[CStdioFile](../../mfc/reference/cstdiofile-class.md)

[CInternetFile](../../mfc/reference/cinternetfile-class.md)

`CGopherFile`

## <a name="requirements"></a>Требования

**Заголовок:** afxinet.h

##  <a name="cgopherfile"></a>  CGopherFile::CGopherFile

Эта функция-член вызывается для создания `CGopherFile` объекта.

```
CGopherFile(
    HINTERNET hFile,
    CGopherLocator& refLocator,
    CGopherConnection* pConnection);

CGopherFile(
    HINTERNET hFile,
    HINTERNET hSession,
    LPCTSTR pstrLocator,
    DWORD dwLocLen,
    DWORD_PTR dwContext);
```

### <a name="parameters"></a>Параметры

*hFile*<br/>
Дескриптор файла HINTERNET.

*refLocator*<br/>
Ссылку на [CGopherLocator](../../mfc/reference/cgopherlocator-class.md) объекта.

*pConnection*<br/>
Указатель на [CGopherConnection](../../mfc/reference/cgopherconnection-class.md) объекта.

*hSession*<br/>
Дескриптор текущего сеанса Интернет.

*pstrLocator*<br/>
Указатель на строку, используемую для обнаружения сервера gopher. См. в разделе [сеансы Gopher](cgopherlocator-class.md) Дополнительные сведения о указатели gopher.

*dwLocLen*<br/>
DWORD, содержащее число байтов в *pstrLocator*.

*dwContext*<br/>
Указатель на идентификатор контекста для открываемого файла.

### <a name="remarks"></a>Примечания

Вам потребуется `CGopherFile` для чтения из файла во время сеанса Internet gopher.

Никогда не создаст `CGopherFile` объекта напрямую. Вместо этого необходимо вызвать [CGopherConnection::OpenFile](../../mfc/reference/cgopherconnection-class.md#openfile) Открытие файла на сервере gopher.

## <a name="see-also"></a>См. также

[Класс CInternetFile](../../mfc/reference/cinternetfile-class.md)<br/>
[Диаграмма иерархии](../../mfc/hierarchy-chart.md)<br/>
[Класс CInternetFile](../../mfc/reference/cinternetfile-class.md)<br/>
[Класс CGopherLocator](../../mfc/reference/cgopherlocator-class.md)<br/>
[Класс CGopherFileFind](../../mfc/reference/cgopherfilefind-class.md)<br/>
[Класс CGopherConnection](../../mfc/reference/cgopherconnection-class.md)
