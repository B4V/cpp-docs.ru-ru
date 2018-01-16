---
title: "Сохраняемость элементов управления OLE | Документы Microsoft"
ms.custom: 
ms.date: 11/04/2016
ms.reviewer: 
ms.suite: 
ms.technology: cpp-windows
ms.tgt_pltfrm: 
ms.topic: article
f1_keywords: vc.mfc.macros.ole
dev_langs: C++
helpviewer_keywords:
- OLE controls [MFC], persistence
- persistence, OLE controls
ms.assetid: 64f8dc80-f110-41af-b3ea-14948f6bfdf7
caps.latest.revision: "17"
author: mikeblome
ms.author: mblome
manager: ghogen
ms.workload: cplusplus
ms.openlocfilehash: 3452bccd4bdf94c84e4549f99829aaa087e1803b
ms.sourcegitcommit: 8fa8fdf0fbb4f57950f1e8f4f9b81b4d39ec7d7a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/21/2017
---
# <a name="persistence-of-ole-controls"></a>Сохраняемость элементов управления OLE
Одна из возможностей элементов управления OLE является свойством сохраняемости (или сериализации), который позволяет элементу управления OLE для чтения или записи значения свойств в и из файла или потока. Приложения-контейнера можно использовать сериализацию для хранения значений свойств элемента управления, даже после того, что приложение уничтожения элемента управления. Значения свойств элемента управления OLE могут считываться из файла или потока при создании нового экземпляра элемента управления создается в дальнейшем.  
  
### <a name="persistence-of-ole-controls"></a>Сохраняемость элементов управления OLE  
  
|||  
|-|-|  
|[PX_Blob](#px_blob)|Меняет свойства элемента управления, в котором хранятся данные больших двоичных объектов (BLOB).|  
|[PX_Bool](#px_bool)|Меняет местами свойство элемента управления типа **BOOL**.|  
|[PX_Color](#px_color)|Меняет местами свойство цвет элемента управления.|  
|[PX_Currency](#px_currency)|Меняет местами свойство элемента управления типа **CY**.|  
|[PX_DataPath](#px_datapath)|Меняет местами свойство элемента управления типа `CDataPathProperty`.|  
|[PX_Double](#px_double)|Меняет местами свойство элемента управления типа **двойные**.|  
|[PX_Font](#px_font)|Меняет свойства шрифта элемента управления.|  
|[PX_Float](#px_float)|Меняет местами свойство элемента управления типа **float**.|  
|[PX_IUnknown](#px_iunknown)|Меняет местами свойство неопределенного типа элемента управления.|  
|[PX_Long](#px_long)|Меняет местами свойство элемента управления типа **длинные**.|  
|[PX_Picture](#px_picture)|Меняет свойства изображения элемента управления.|  
|[PX_Short](#px_short)|Меняет местами свойство элемента управления типа **короткие**.|  
|[PX_ULong](#px_ulong)|Меняет местами свойство элемента управления типа **ULONG**.|  
|[PX_UShort](#px_ushort)|Меняет местами свойство элемента управления типа **USHORT**.|  
|[PXstring](#px_string)|Меняет местами символ строковое свойство элемента управления.|  
|[PX_VBXFontConvert](#px_vbxfontconvert)|Меняет свойства, связанные со шрифтами VBX элемента управления в свойства шрифта элемента управления OLE.|  
  
 Кроме того `AfxOleTypeMatchGuid` глобальной функции предоставляется для проверки на соответствие между `TYPEDESC` и с указанным кодом GUID.  
  
##  <a name="px_blob"></a>PX_Blob  
 Вызывайте эту функцию в пределах элемента управления `DoPropExchange` функции-члена для сериализации или инициализировать свойство, которое сохраняет данные больших двоичных объектов (BLOB).  
  
```  
 
BOOL  
PX_Blob(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    HGLOBAL& 
hBlob  ,  
    HGLOBAL 
hBlobDefault  
= NULL);  
```  
  
### <a name="parameters"></a>Параметры  
 `pPX`  
 Указатель на [CPropExchange](../../mfc/reference/cpropexchange-class.md) объекта (обычно передается как параметр `DoPropExchange`).  
  
 `pszPropName`  
 Имя свойства при обмене.  
  
 `hBlob`  
 Ссылка на переменную, в котором хранится свойство (обычно переменную-член класса).  
  
 `hBlobDefault`  
 Значение по умолчанию для свойства.  
  
### <a name="return-value"></a>Возвращаемое значение  
 Ненулевое значение, если exchange был успешным; 0, если операция завершилась неудачей.  
  
### <a name="remarks"></a>Примечания  
 Значение свойства будет чтения или записи ссылается переменная `hBlob`соответствующим образом. Эта переменная должна инициализироваться **NULL** перед вызовом изначально `PX_Blob` в первый раз (как правило, это можно сделать в конструкторе элемента управления). Если `hBlobDefault` указано, оно будет использоваться как значение свойства по умолчанию. Это значение используется в том случае, если по какой-либо причине происходит сбой процесса инициализации или сериализации элемента управления.  
  
 Дескрипторы `hBlob` и `hBlobDefault` ссылаться на блок памяти, который содержит следующее:  
  
-   Объект `DWORD` , содержащее длину в байтах, двоичных данных ниже, а затем немедленно по  
  
-   Блок памяти, содержащей сами двоичные данные.  
  
 Обратите внимание, что `PX_Blob` приведет к выделению памяти, с помощью окон [GlobalAlloc](http://msdn.microsoft.com/library/windows/desktop/aa366574) API, при загрузке свойств тип большого двоичного ОБЪЕКТА. Вы несете ответственность за освобождение памяти. Таким образом, деструктор класса элемента управления должен вызывать [GlobalFree](http://msdn.microsoft.com/library/windows/desktop/aa366579) любого свойства, тип большого двоичного ОБЪЕКТА дескрипторы для освобождения вверх память, выделенная для элемента управления.  
  
##  <a name="px_bool"></a>PX_Bool  
 Вызывайте эту функцию в пределах элемента управления `DoPropExchange` функции-члена для сериализации или инициализировать свойство типа **BOOL**.  
  
```  
 
BOOL  
PX_Bool(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    BOOL& bValue);

BOOL  
PX_Bool(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    BOOL& 
bValue  ,  
    BOOL bDefault);  
```  
  
### <a name="parameters"></a>Параметры  
 `pPX`  
 Указатель на [CPropExchange](../../mfc/reference/cpropexchange-class.md) объекта (обычно передается как параметр `DoPropExchange`).  
  
 `pszPropName`  
 Имя свойства при обмене.  
  
 `bValue`  
 Ссылка на переменную, в котором хранится свойство (обычно переменную-член класса).  
  
 `bDefault`  
 Значение по умолчанию для свойства.  
  
### <a name="return-value"></a>Возвращаемое значение  
 Ненулевое значение, если exchange был успешным; 0, если операция завершилась неудачей.  
  
### <a name="remarks"></a>Примечания  
 Значение свойства будет чтения или записи ссылается переменная `bValue`соответствующим образом. Если `bDefault` указано, оно будет использоваться как значение свойства по умолчанию. Это значение используется в том случае, если по какой-либо причине происходит сбой элемента управления процессом сериализации.  
  
##  <a name="px_color"></a>PX_Color  
 Вызывайте эту функцию в пределах элемента управления `DoPropExchange` функции-члена для сериализации или инициализировать свойство типа **OLE_COLOR**.  
  
```  
 
BOOL PX_Color(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    OLE_COLOR& clrValue);

BOOL PX_Color(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    OLE_COLOR& 
clrValue  ,  
    OLE_COLOR 
clrDefault);  
```  
  
### <a name="parameters"></a>Параметры  
 `pPX`  
 Указатель на [CPropExchange](../../mfc/reference/cpropexchange-class.md) объекта (обычно передается как параметр `DoPropExchange`).  
  
 `pszPropName`  
 Имя свойства при обмене.  
  
 `clrValue`  
 Ссылка на переменную, в котором хранится свойство (обычно переменную-член класса).  
  
 `clrDefault`  
 Значение по умолчанию для свойства, определяемые разработчиком элемента управления.  
  
### <a name="return-value"></a>Возвращаемое значение  
 Ненулевое значение, если exchange был успешным; 0, если операция завершилась неудачей.  
  
### <a name="remarks"></a>Примечания  
 Значение свойства будет чтения или записи ссылается переменная `clrValue`соответствующим образом. Если `clrDefault` указано, оно будет использоваться как значение свойства по умолчанию. Это значение используется в том случае, если по какой-либо причине происходит сбой элемента управления процессом сериализации.  
  
##  <a name="px_currency"></a>PX_Currency  
 Вызывайте эту функцию в пределах элемента управления `DoPropExchange` функции-члена для сериализации или инициализировать свойство типа **валюты**.  
  
```  
 
BOOL  
PX_Currency(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    CY& cyValue);

BOOL  
PX_Currency(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    CY& 
cyValue  ,  
    CY cyDefault);  
```  
  
### <a name="parameters"></a>Параметры  
 `pPX`  
 Указатель на [CPropExchange](../../mfc/reference/cpropexchange-class.md) объекта (обычно передается как параметр `DoPropExchange`).  
  
 `pszPropName`  
 Имя свойства при обмене.  
  
 `cyValue`  
 Ссылка на переменную, в котором хранится свойство (обычно переменную-член класса).  
  
 `cyDefault`  
 Значение по умолчанию для свойства.  
  
### <a name="return-value"></a>Возвращаемое значение  
 Ненулевое значение, если exchange был успешным; 0, если операция завершилась неудачей.  
  
### <a name="remarks"></a>Примечания  
 Значение свойства будет чтения или записи ссылается переменная `cyValue`соответствующим образом. Если `cyDefault` указано, оно будет использоваться как значение свойства по умолчанию. Это значение используется в том случае, если по какой-либо причине происходит сбой элемента управления процессом сериализации.  
  
##  <a name="px_datapath"></a>PX_DataPath  
 Вызывайте эту функцию в пределах элемента управления `DoPropExchange` функции-члена для сериализации или инициализировать свойства пути данных типа [CDataPathProperty](../../mfc/reference/cdatapathproperty-class.md).  
  
```  
 
BOOL  
PX_DataPath(
    CPropExchange* 
pPX,  
    LPCTSTR 
pszPropName,  
    CDataPathProperty& dataPathProperty);

BOOL  
PX_DataPath(
    CPropExchange* 
pPX,  
    CDataPathProperty& dataPathProperty);  
```  
  
### <a name="parameters"></a>Параметры  
 `pPX`  
 Указатель на [CPropExchange](../../mfc/reference/cpropexchange-class.md) объекта (обычно передается как параметр `DoPropExchange`).  
  
 `pszPropName`  
 Имя свойства при обмене.  
  
 `dataPathProperty`  
 Ссылка на переменную, в котором хранится свойство (обычно переменную-член класса).  
  
### <a name="return-value"></a>Возвращаемое значение  
 Ненулевое значение, если exchange был успешным; 0, если операция завершилась неудачей.  
  
### <a name="remarks"></a>Примечания  
 Свойства пути данных реализации управления асинхронной свойств. Значение свойства будет чтения или записи ссылается переменная `dataPathProperty`соответствующим образом.  
  
##  <a name="px_double"></a>PX_Double  
 Вызывайте эту функцию в пределах элемента управления `DoPropExchange` функции-члена для сериализации или инициализировать свойство типа **двойные**.  
  
```  
 
BOOL  
PX_Double(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    double& doubleValue);

BOOL  
PX_Double(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    double& 
doubleValue  ,  
    double doubleDefault);  
```  
  
### <a name="parameters"></a>Параметры  
 `pPX`  
 Указатель на [CPropExchange](../../mfc/reference/cpropexchange-class.md) объекта (обычно передается как параметр `DoPropExchange`).  
  
 `pszPropName`  
 Имя свойства при обмене.  
  
 `doubleValue`  
 Ссылка на переменную, в котором хранится свойство (обычно переменную-член класса).  
  
 `doubleDefault`  
 Значение по умолчанию для свойства.  
  
### <a name="return-value"></a>Возвращаемое значение  
 Ненулевое значение, если exchange был успешным; 0, если операция завершилась неудачей.  
  
### <a name="remarks"></a>Примечания  
 Значение свойства является считывается или записывается в переменную ссылается `doubleValue`соответствующим образом. Если `doubleDefault` указано, оно будет использоваться как значение свойства по умолчанию. Это значение используется в том случае, если по какой-либо причине происходит сбой элемента управления процессом сериализации.  
  
##  <a name="px_font"></a>PX_Font  
 Вызывайте эту функцию в пределах элемента управления `DoPropExchange` функции-члена для сериализации или инициализировать свойство тип шрифта.  
  
```  
 
BOOL  
PX_Font(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    CFontHolder& 
font  ,  
    const 
FONTDESC  
FAR* 
pFontDesc  
= 
NULL,  
    LPFONTDISP 
pFontDispAmbient  
= NULL);  
```  
  
### <a name="parameters"></a>Параметры  
 `pPX`  
 Указатель на [CPropExchange](../../mfc/reference/cpropexchange-class.md) объекта (обычно передается как параметр `DoPropExchange`).  
  
 `pszPropName`  
 Имя свойства при обмене.  
  
 `font`  
 Ссылку на `CFontHolder` , содержащий свойства шрифта.  
  
 `pFontDesc`  
 Указатель на **FONTDESC** структуру, содержащую значения для использования в инициализации состояния по умолчанию свойства шрифта, в случае когда `pFontDispAmbient` — **NULL**.  
  
 `pFontDispAmbient`  
 Указатель на **IFontDisp** интерфейс шрифт, используемый при инициализации состояние свойства шрифта по умолчанию.  
  
### <a name="return-value"></a>Возвращаемое значение  
 Ненулевое значение, если exchange был успешным; 0, если операция завершилась неудачей.  
  
### <a name="remarks"></a>Примечания  
 Значение этого свойства считывается или записывается в `font`, `CFontHolder` ссылки, при необходимости. Если `pFontDesc` и `pFontDispAmbient` указаны, они используются для инициализации значения этого свойства по умолчанию, при необходимости. Эти значения используются в том случае, если по какой-либо причине происходит сбой элемента управления процессом сериализации. Как правило, передаваемому **NULL** для `pFontDesc` и окружения значения, возвращенного `COleControl::AmbientFont` для `pFontDispAmbient`. Обратите внимание, что возвращаемый объект шрифта `COleControl::AmbientFont` должны быть удалены с помощью вызова **IFontDisp::Release** функции-члена.  
  
##  <a name="px_float"></a>PX_Float  
 Вызывайте эту функцию в пределах элемента управления `DoPropExchange` функции-члена для сериализации или инициализировать свойство типа **float**.  
  
```  
 
BOOL  
PX_Float(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    float& floatValue);

BOOL  
PX_Float(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    float& 
floatValue  ,  
    float floatDefault);  
```  
  
### <a name="parameters"></a>Параметры  
 `pPX`  
 Указатель на [CPropExchange](../../mfc/reference/cpropexchange-class.md) объекта (обычно передается как параметр `DoPropExchange`).  
  
 `pszPropName`  
 Имя свойства при обмене.  
  
 `floatValue`  
 Ссылка на переменную, в котором хранится свойство (обычно переменную-член класса).  
  
 `floatDefault`  
 Значение по умолчанию для свойства.  
  
### <a name="return-value"></a>Возвращаемое значение  
 Ненулевое значение, если exchange был успешным; 0, если операция завершилась неудачей.  
  
### <a name="remarks"></a>Примечания  
 Значение свойства является считывается или записывается в переменную ссылается `floatValue`соответствующим образом. Если `floatDefault` указано, оно будет использоваться как значение свойства по умолчанию. Это значение используется в том случае, если по какой-либо причине происходит сбой элемента управления процессом сериализации.  
  
##  <a name="px_iunknown"></a>PX_IUnknown  
 Вызывайте эту функцию в пределах элемента управления `DoPropExchange` функции-члена для сериализации или инициализировать свойство, представленное объектом с **IUnknown**-производным интерфейсом.  
  
```  
 
BOOL  
PX_IUnknown(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    LPUNKNOWN& 
pUnk  ,  
    REFIID 
iid  ,  
    LPUNKNOWN 
pUnkDefault  
= NULL);  
```  
  
### <a name="parameters"></a>Параметры  
 `pPX`  
 Указатель на [CPropExchange](../../mfc/reference/cpropexchange-class.md) объекта (обычно передается как параметр `DoPropExchange`).  
  
 `pszPropName`  
 Имя свойства при обмене.  
  
 *pUnk*  
 Ссылка на переменную, содержащую интерфейс объект, представляющий значение свойства.  
  
 `iid`  
 Идентификатор интерфейса, позволяющее определить, какой интерфейс объект свойства, используемые элементом управления.  
  
 `pUnkDefault`  
 Значение по умолчанию для свойства.  
  
### <a name="return-value"></a>Возвращаемое значение  
 Ненулевое значение, если exchange был успешным; 0, если операция завершилась неудачей.  
  
### <a name="remarks"></a>Примечания  
 Значение свойства является считывается или записывается в переменную ссылается *pUnk*соответствующим образом. Если `pUnkDefault` указано, оно будет использоваться как значение свойства по умолчанию. Это значение используется в том случае, если по какой-либо причине происходит сбой элемента управления процессом сериализации.  
  
##  <a name="px_long"></a>PX_Long  
 Вызывайте эту функцию в пределах элемента управления `DoPropExchange` функции-члена для сериализации или инициализировать свойство типа **длинные**.  
  
```  
 
BOOL  
PX_Long(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    long& lValue);

BOOL  
PX_Long(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    long& 
lValue  ,  
    long lDefault);  
```  
  
### <a name="parameters"></a>Параметры  
 `pPX`  
 Указатель на [CPropExchange](../../mfc/reference/cpropexchange-class.md) объекта (обычно передается как параметр `DoPropExchange`).  
  
 `pszPropName`  
 Имя свойства при обмене.  
  
 `lValue`  
 Ссылка на переменную, в котором хранится свойство (обычно переменную-член класса).  
  
 `lDefault`  
 Значение по умолчанию для свойства.  
  
### <a name="return-value"></a>Возвращаемое значение  
 Ненулевое значение, если exchange был успешным; 0, если операция завершилась неудачей.  
  
### <a name="remarks"></a>Примечания  
 Значение свойства является считывается или записывается в переменную ссылается `lValue`соответствующим образом. Если `lDefault` указано, оно будет использоваться как значение свойства по умолчанию. Это значение используется в том случае, если по какой-либо причине происходит сбой элемента управления процессом сериализации.  
  
##  <a name="px_picture"></a>PX_Picture  
 Вызывайте эту функцию в пределах элемента управления `DoPropExchange` функции-члена для сериализации или инициализировать свойства изображения элемента управления.  
  
```  
 
BOOL  
PX_Picture(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    CPictureHolder& pict);

BOOL  
PX_Picture(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    CPictureHolder& 
pict  ,  
    CPictureHolder& pictDefault);  
```  
  
### <a name="parameters"></a>Параметры  
 `pPX`  
 Указатель на [CPropExchange](../../mfc/reference/cpropexchange-class.md) объекта (обычно передается как параметр `DoPropExchange`).  
  
 `pszPropName`  
 Имя свойства при обмене.  
  
 `pict`  
 Ссылка на [CPictureHolder](../../mfc/reference/cpictureholder-class.md) объекта, где хранится свойство (обычно переменную-член класса).  
  
 `pictDefault`  
 Значение по умолчанию для свойства.  
  
### <a name="return-value"></a>Возвращаемое значение  
 Ненулевое значение, если exchange был успешным; 0, если операция завершилась неудачей.  
  
### <a name="remarks"></a>Примечания  
 Значение свойства является считывается или записывается в переменную ссылается `pict`соответствующим образом. Если `pictDefault` указано, оно будет использоваться как значение свойства по умолчанию. Это значение используется в том случае, если по какой-либо причине происходит сбой элемента управления процессом сериализации.  
  
##  <a name="px_short"></a>PX_Short  
 Вызывайте эту функцию в пределах элемента управления `DoPropExchange` функции-члена для сериализации или инициализировать свойство типа **короткие**.  
  
```  
 
BOOL  
PX_Short(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    short& sValue);

BOOL  
PX_Short(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    short& 
sValue  ,  
    short sDefault);  
```  
  
### <a name="parameters"></a>Параметры  
 `pPX`  
 Указатель на [CPropExchange](../../mfc/reference/cpropexchange-class.md) объекта (обычно передается как параметр `DoPropExchange`).  
  
 `pszPropName`  
 Имя свойства при обмене.  
  
 `sValue`  
 Ссылка на переменную, в котором хранится свойство (обычно переменную-член класса).  
  
 `sDefault`  
 Значение по умолчанию для свойства.  
  
### <a name="return-value"></a>Возвращаемое значение  
 Ненулевое значение, если exchange был успешным; 0, если операция завершилась неудачей.  
  
### <a name="remarks"></a>Примечания  
 Значение свойства является считывается или записывается в переменную ссылается `sValue`соответствующим образом. Если `sDefault` указано, оно будет использоваться как значение свойства по умолчанию. Это значение используется в том случае, если по какой-либо причине происходит сбой элемента управления процессом сериализации.  
  
##  <a name="px_ulong"></a>PX_ULong  
 Вызывайте эту функцию в пределах элемента управления `DoPropExchange` функции-члена для сериализации или инициализировать свойство типа **ULONG**.  
  
```  
 
BOOL  
PX_ULong(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    ULONG& ulValue);

BOOL  
PX_ULong(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    ULONG& 
ulValue  ,  
    long ulDefault);  
```  
  
### <a name="parameters"></a>Параметры  
 `pPX`  
 Указатель на [CPropExchange](../../mfc/reference/cpropexchange-class.md) объекта (обычно передается как параметр `DoPropExchange`).  
  
 `pszPropName`  
 Имя свойства при обмене.  
  
 `ulValue`  
 Ссылка на переменную, в котором хранится свойство (обычно переменную-член класса).  
  
 `ulDefault`  
 Значение по умолчанию для свойства.  
  
### <a name="return-value"></a>Возвращаемое значение  
 Ненулевое значение, если exchange был успешным; 0, если операция завершилась неудачей.  
  
### <a name="remarks"></a>Примечания  
 Значение свойства является считывается или записывается в переменную ссылается `ulValue`соответствующим образом. Если `ulDefault` указано, оно будет использоваться как значение свойства по умолчанию. Это значение используется в том случае, если по какой-либо причине происходит сбой элемента управления процессом сериализации.  
  
##  <a name="px_ushort"></a>PX_UShort  
 Вызывайте эту функцию в пределах элемента управления `DoPropExchange` функции-члена для сериализации или инициализировать свойство типа `unsigned` **короткие**.  
  
```  
 
BOOL  
PX_UShort(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    USHORT& usValue);

BOOL  
PX_UShort(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    USHORT& 
usValue  ,  
    USHORT usDefault);  
```  
  
### <a name="parameters"></a>Параметры  
 `pPX`  
 Указатель на [CPropExchange](../../mfc/reference/cpropexchange-class.md) объекта (обычно передается как параметр `DoPropExchange`).  
  
 `pszPropName`  
 Имя свойства при обмене.  
  
 *usValue*  
 Ссылка на переменную, в котором хранится свойство (обычно переменную-член класса).  
  
 *usDefault*  
 Значение по умолчанию для свойства.  
  
### <a name="return-value"></a>Возвращаемое значение  
 Ненулевое значение, если exchange был успешным; 0, если операция завершилась неудачей.  
  
### <a name="remarks"></a>Примечания  
 Значение свойства является считывается или записывается в переменную ссылается *usValue*соответствующим образом. Если *usDefault* указано, оно будет использоваться как значение свойства по умолчанию. Это значение используется в том случае, если по какой-либо причине происходит сбой элемента управления процессом сериализации.  
  
##  <a name="px_string"></a>PXstring  
 Вызывайте эту функцию в пределах элемента управления **DoPropExchange** функции-члена для сериализации или инициализировать свойство строку символов.  
  
```  
 
BOOL  
PXstring(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    CString& strValue);

BOOL  
PXstring(
    CPropExchange* 
pPX  ,  
    LPCTSTR 
pszPropName  ,  
    CString& 
strValue  ,  
    CString strDefault);  
```  
  
### <a name="parameters"></a>Параметры  
 `pPX`  
 Указатель на [CPropExchange](../../mfc/reference/cpropexchange-class.md) объекта (обычно передается как параметр `DoPropExchange`).  
  
 `pszPropName`  
 Имя свойства при обмене.  
  
 `strValue`  
 Ссылка на переменную, в котором хранится свойство (обычно переменную-член класса).  
  
 `strDefault`  
 Значение по умолчанию для свойства.  
  
### <a name="return-value"></a>Возвращаемое значение  
 Ненулевое значение, если exchange был успешным; 0, если операция завершилась неудачей.  
  
### <a name="remarks"></a>Примечания  
 Значение свойства является считывается или записывается в переменную ссылается `strValue`соответствующим образом. Если `strDefault` указано, оно будет использоваться как значение свойства по умолчанию. Это значение используется в том случае, если по какой-либо причине происходит сбой элемента управления процессом сериализации.  
  
##  <a name="px_vbxfontconvert"></a>PX_VBXFontConvert  
 Вызывайте эту функцию в пределах элемента управления `DoPropExchange` функции-члена для инициализации свойства шрифта путем преобразования свойства, связанные со шрифтами VBX элемента управления.  
  
```  
 
BOOL  
PX_VBXFontConvert(
    CPropExchange* 
pPX  ,  
    CFontHolder& font);  
```  
  
### <a name="parameters"></a>Параметры  
 `pPX`  
 Указатель на [CPropExchange](../../mfc/reference/cpropexchange-class.md) объекта (обычно передается как параметр `DoPropExchange`).  
  
 `font`  
 Свойства шрифта элемента управления OLE, который будет содержать преобразованные свойства VBX шрифте.  
  
### <a name="return-value"></a>Возвращаемое значение  
 Ненулевое значение, если exchange был успешным; 0, если операция завершилась неудачей.  
  
### <a name="remarks"></a>Примечания  
 Эта функция должна использоваться только элемента управления OLE, предназначенный для прямого управления VBX замены. Если среда разработки Visual Basic преобразует форму, содержащую элемент управления VBX для использования соответствующего замены элемента управления OLE, он вызывает элемент управления **IDataObject::SetData** функции, передав свойство задано, содержит данные, свойство VBX элемента управления. Эта операция, в свою очередь, вызывает элемент управления `DoPropExchange` вызываемая функция. `DoPropExchange`можно вызвать `PX_VBXFontConvert` для преобразования свойства, связанные со шрифтами VBX элемента управления (например, «FontName,» «FontSize,» и т. д) в соответствующих компонентов свойства шрифта элемента управления OLE.  
  
 `PX_VBXFontConvert`должен вызываться только при управления фактически преобразуется из VBX формы приложения. Пример:  
  
 [!code-cpp[NVC_MFCActiveXControl#14](../../mfc/codesnippet/cpp/persistence-of-ole-controls_1.cpp)]  
[!code-cpp[NVC_MFCActiveXControl#15](../../mfc/codesnippet/cpp/persistence-of-ole-controls_2.cpp)]  
  
## <a name="see-also"></a>См. также  
 [Макросы и глобальные объекты](../../mfc/reference/mfc-macros-and-globals.md)