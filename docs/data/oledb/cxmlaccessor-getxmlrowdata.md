---
title: "CXMLAccessor::GetXMLRowData | Документы Microsoft"
ms.custom: 
ms.date: 11/04/2016
ms.reviewer: 
ms.suite: 
ms.technology: cpp-windows
ms.tgt_pltfrm: 
ms.topic: article
f1_keywords:
- ATL::CXMLAccessor::GetXMLRowData
- ATL.CXMLAccessor.GetXMLRowData
- CXMLAccessor::GetXMLRowData
- CXMLAccessor.GetXMLRowData
- GetXMLRowData
dev_langs: C++
helpviewer_keywords: GetXMLRowData method
ms.assetid: 156b66e3-42fd-491c-8943-38cf5e36f687
caps.latest.revision: "9"
author: mikeblome
ms.author: mblome
manager: ghogen
ms.openlocfilehash: 2b21e48439fbf4f420751e2f89903044626df9c4
ms.sourcegitcommit: ebec1d449f2bd98aa851667c2bfeb7e27ce657b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/24/2017
---
# <a name="cxmlaccessorgetxmlrowdata"></a>CXMLAccessor::GetXMLRowData
Получает все содержимое таблицы по строкам данных строка в формате XML.  
  
## <a name="syntax"></a>Синтаксис  
  
```  
  
      HRESULT GetXMLRowData(   
   CSimpleStringW& strOutput,   
   bool bAppend = false    
) throw( );  
```  
  
#### <a name="parameters"></a>Параметры  
 `strOutput`  
 [out] Ссылка на буфер, содержащий данные таблицы должны быть получены. Данные форматируются как строковые данные с XML имена тегов, которые совпадают с именами столбцов в хранилище данных.  
  
 *bAppend*  
 [in] Логическое значение, указывающее, следует ли добавить строку в конец выходных данных.  
  
## <a name="return-value"></a>Возвращаемое значение  
 Один из стандартных `HRESULT` значения.  
  
## <a name="remarks"></a>Примечания  
 Ниже показан способ форматирования данных в строке в формате XML. `DATA`ниже представляет строки данных. С помощью move методы для перемещения требуемой строки.  
  
 `<row>`  
  
 `<column name>DATA</column name>`  
  
 `</row>`  
  
## <a name="requirements"></a>Требования  
 **Заголовок:** atldbcli.h  
  
## <a name="see-also"></a>См. также  
 [Класс CXMLAccessor](../../data/oledb/cxmlaccessor-class.md)