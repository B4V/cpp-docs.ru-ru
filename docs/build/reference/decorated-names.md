---
title: "Внутренние имена | Документы Microsoft"
ms.custom: 
ms.date: 11/04/2016
ms.reviewer: 
ms.suite: 
ms.technology: cpp-tools
ms.tgt_pltfrm: 
ms.topic: article
dev_langs: C++
helpviewer_keywords:
- decorated names, definition
- name decoration [C++]
- names [C++], decorated
ms.assetid: a4e9ae8e-b239-4454-b401-4102793cb344
caps.latest.revision: "10"
author: corob-msft
ms.author: corob
manager: ghogen
ms.workload: cplusplus
ms.openlocfilehash: a2ad7fc8e6d9b7fa261d7811086ef02738c77e49
ms.sourcegitcommit: 8fa8fdf0fbb4f57950f1e8f4f9b81b4d39ec7d7a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/21/2017
---
# <a name="decorated-names"></a>Внутренние имена
Функции, данные и объекты в программах на языках C и C++ внутренне представляются декорированными именами. Объект *декорированное имя* является закодированной строкой, созданным компилятором во время компиляции объекта, данных или определении функции. Оно содержит соглашения о вызовах, типы, параметры функции и другие сведения, а также имя. Такое дополнение имен, также известные как *декорированием*, помогает компоновщику найти правильные функции и объекты при компоновке исполняемого файла.  
  
 Соглашения о декорированных именах менялись в различных версиях Visual C++ и также могут различаться на различных целевых архитектурах. Для правильной компоновки с исходными файлами, созданными с помощью Visual C++, C и C++, DLL и библиотеки должны быть скомпилированы с помощью одинаковых наборов инструментов компилятора, флагов и для одной целевой архитектуры.  
  
 **Содержание**  
  
-   [Использование внутренних имен](#Using)  
  
-   [Формат C++ внутреннего имени](#Format)  
  
-   [Формат C внутреннего имени](#FormatC)  
  
-   [Просмотр внутренних имен](#Viewing)  
  
-   [Просмотр внешних имен](#Undecorated)  
  
##  <a name="Using"></a>Использование внутренних имен  
 Как правило, не нужно знать внутреннее имя, чтобы написать код, который успешно компилируется и компонуется. Внутренние имена — это внутренние средства для компилятора и компоновщика. Инструменты обычно могут обрабатывать имя в недекорированной форме. Тем не менее внутреннее имя иногда требуется при указании имени функции для компоновщика и других средств. Например, для сопоставления перегруженных функций C++, элементов пространств имен, конструкторов, деструкторов и специальных функций-членов класса, необходимо указать внутреннее имя. Дополнительные сведения о флагах и других ситуациях, для которых требуются внутренние имена, см. в документации по средствам и параметрам, которые вы используете.  
  
 При изменении имени функции, класса, соглашении о вызовах, возвращаемого типа или какого-либо параметра внутреннее имя также изменяется. В этом случае необходимо получить новое внутреннее имя и использовать его везде, где оно указано.  
  
 Декорирование имен также важно при компоновке с кодом, написанным на других языках программирования, или при использовании других компиляторов. Разные компиляторы используют различные соглашения о дополнении имен. Если исполняемый файл связывается с кодом, написанным на другом языке, необходимо уделить особое внимание сопоставлению экспортированных и импортированных параметров и соглашений о вызовах. В коде языка сборки необходимо использовать внутренние имена и соглашения о вызовах Visual C++ для компоновки с исходным кодом, написанном на Visual C++.  
  
##  <a name="Format"></a>Формат C++ внутреннего имени  
 Внутреннее имя функции C++ содержит следующие сведения.  
  
-   Имя функции.  
  
-   Класс, членом которого является функция, если это функция-член. Это может быть класс, в который входит содержащий функцию класс, и т. д.  
  
-   Пространство имен, которой принадлежит функция, если она входит в пространство имен.  
  
-   Типы параметров функции.  
  
-   Соглашение о вызовах.  
  
-   Тип значения, возвращаемого функцией.  
  
 Имена функций и классов кодируются во внутреннем имени. Остальная часть внутреннего имени — это код, который имеет смысл только для компилятора и компоновщика. Ниже приведены примеры внешних и внутренних имен C++.  
  
|Внешнее имя|Внутреннее имя|  
|----------------------|--------------------|  
|`int a(char){int i=3;return i;};`|`?a@@YAHD@Z`|  
|`void __stdcall b::c(float){};`|`?c@b@@AAGXM@Z`|  
  
##  <a name="FormatC"></a>Формат C внутреннего имени  
 Формат декорирования для функции C зависит от соглашения о вызовах, используемого в ее объявлении, как показано в следующей таблице. Этот же формат используется, если в коде C++ объявлена компоновка `extern "C"`. Соглашение о вызовах по умолчанию — `__cdecl`. Обратите внимание, что в 64-разрядной среде, функции не декорируются.  
  
|Соглашение о вызовах|Оформление|  
|------------------------|----------------|  
|`__cdecl`|Символ подчеркивания в начале (**_**)|  
|`__stdcall`|Символ подчеркивания в начале (**_**) и конечный символ (@) за которым следует число байтов в списке параметров в десятичном формате|  
|`__fastcall`|Начальные и конечные символы @, за которым следует десятичное число, представляющее количество байтов в списке параметров|  
|`__vectorcall`|Два конечных символа @@, за которыми следует десятичное число байтов в списке параметров|  
  
##  <a name="Viewing"></a>Просмотр внутренних имен  
 Вы можете получить внутреннюю форму имени символа после компиляции исходного файла, содержащего данные, объект, определение или прототип функции. Для просмотра внутренних имен в программе можно использовать один из следующих методов.  
  
-   #### <a name="to-use-a-listing-to-view-decorated-names"></a>Использование листинга для просмотра внутренних имен  
  
    1.  Создайте листинг, скомпилировав исходный файл, содержащий данные, объект, или определение функции или прототип с [тип файла кода](../../build/reference/fa-fa-listing-file.md) параметр компилятора сборка с исходным кодом (**/FAs**).  
  
         Например, введите `cl /c /FAs example.cpp` в командной строке разработчика, чтобы создать файл листинга example.asm.  
  
    2.  В полученном файле листинга найдите строку, которая начинается с PUBLIC и завершается точкой с запятой, за которой следует внешнее имя данных или функции. Символ между PUBLIC и точкой с запятой представляет внутреннее имя.  
  
-   #### <a name="to-use-dumpbin-to-view-decorated-names"></a>Использование служебной программы DUMPBIN для просмотра внутренних имен  
  
    1.  Для просмотра экспортированных символов в файле OBJ- или LIB-файл, введите `dumpbin /symbols` `objfile` в командной строке разработчика.  
  
    2.  Чтобы найти внутреннюю форму символа, найдите внешнее имя в скобках. Внутреннее имя в той же строке после вертикальной черты (&#124;) символов и перед внешним именем.  
  
##  <a name="Undecorated"></a>Просмотр внешних имен  
 Можно использовать программу undname.exe для преобразования внутреннего имени в недекорированную форму. В этом примере показано, как это работает.  
  
```  
C:\>undname ?func1@a@@AAEXH@Z  
Microsoft (R) C++ Name Undecorator  
Copyright (C) Microsoft Corporation. All rights reserved.  
  
Undecoration of :- "?func1@a@@AAEXH@Z"  
is :- "private: void __thiscall a::func1(int)"  
```  
  
## <a name="see-also"></a>См. также  
 [Средства построения C/C++](../../build/reference/c-cpp-build-tools.md)   
 [Использование ключевого слова extern для задания компоновки](../../cpp/using-extern-to-specify-linkage.md)