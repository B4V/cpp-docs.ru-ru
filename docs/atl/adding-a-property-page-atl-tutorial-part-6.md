---
title: "Добавление страницы свойств (ATL учебника, часть 6) | Документы Microsoft"
ms.custom: 
ms.date: 11/04/2016
ms.reviewer: 
ms.suite: 
ms.technology: cpp-windows
ms.tgt_pltfrm: 
ms.topic: get-started-article
dev_langs: C++
ms.assetid: df80d255-e7ea-49d9-b940-3f012e90cf9b
caps.latest.revision: "15"
author: mikeblome
ms.author: mblome
manager: ghogen
ms.workload: cplusplus
ms.openlocfilehash: 067c5d662fee3838a33a3b53fd5dab2946ab50cf
ms.sourcegitcommit: 8fa8fdf0fbb4f57950f1e8f4f9b81b4d39ec7d7a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/21/2017
---
# <a name="adding-a-property-page-atl-tutorial-part-6"></a>Добавление страницы свойств (учебник ATL, часть 6)
Страницы свойств реализуются как отдельные объекты COM, которые позволят им можно было использовать при необходимости. На этом шаге необходимо выполнить следующие задачи, чтобы добавить страницу свойств для элемента управления:  
  
-   Создание ресурса страницы свойств  
  
-   Добавление кода для создания и управления ими на странице свойств  
  
-   Добавление страницы свойств для элемента управления  
  
## <a name="creating-the-property-page-resource"></a>Создание ресурса страницы свойств  
 Чтобы добавить страницу свойств элемента управления, используйте мастер добавления класса ATL.  
  
#### <a name="to-add-a-property-page"></a>Добавление страницы свойств  
  
1.  В обозревателе решений щелкните правой кнопкой мыши многоугольника.  
  
2.  В контекстном меню выберите **добавить**, а затем нажмите кнопку **Добавление класса**.  
  
3.  В списке шаблонов выберите **страницы свойств ATL** и нажмите кнопку **добавить**.  
  
4.  Когда появится мастер страницы свойств ATL, введите `PolyProp` как **короткие** имя.  
  
5.  Нажмите кнопку **строки** Открытие **строки** страницы и введите **& многоугольника** как **заголовка**.  
  
     **Заголовок** свойства страница является строкой, которая отображается на вкладке этой страницы. **Строка документации** описание, использующий фрейм свойства перевести в состояние строки или в подсказках. Обратите внимание, что стандартный фрейм свойства в настоящее время не использует данной строкой, поэтому ее можно оставить содержимое по умолчанию. Не будет формировать **файл справки** в данный момент, поэтому удалите запись в этом текстовом поле.  
  
6.  Нажмите кнопку **Готово**, и будет создан объект страницы свойств.  
  
 Создаются следующие три файла:  
  
|Файл|Описание:|  
|----------|-----------------|  
|PolyProp.h|Содержит класс C++ `CPolyProp`, который реализует страницу свойств.|  
|PolyProp.cpp|Включает файл PolyProp.h.|  
|PolyProp.rgs|Скрипт реестра, который регистрирует объект страницы свойств.|  
  
 Также необходимо принять следующие изменения кода.  
  
-   Карта запись объектов в Polygon.cpp добавляется новую страницу свойств.  
  
-   `PolyProp` Класс добавляется к файлу Polygon.idl.  
  
-   Добавляется новый файл скрипта реестра PolyProp.rgs ресурсов проекта.  
  
-   Шаблон диалогового окна добавляется к ресурсу для страницы свойств проекта.  
  
-   Добавляются строки свойств, указанных в таблице строк ресурсов.  
  
 Теперь добавьте поля, которые должны отображаться на странице свойств.  
  
#### <a name="to-add-fields-to-the-property-page"></a>Добавление полей на странице свойств  
  
1.  В обозревателе решений дважды щелкните файл Polygon.rc ресурсов. Откроется представление ресурсов.  
  
2.  В представлении ресурсов раскройте узел диалог и дважды щелкните IDD_POLYPROP. Обратите внимание, что отобразившемся диалоговом ничего, кроме метки, о том, чтобы вставить здесь элементы управления.  
  
3.  Выберите, подпись и измените его для чтения `Sides:` путем изменения **заголовок** текста в **свойства** окна.  
  
4.  Изменение размера поле «Метка» так, чтобы размер текста.  
  
5.  Перетащите элемент управления редактированием из области элементов справа от метки.  
  
6.  Наконец, измените **идентификатор** элемента управления для редактирования `IDC_SIDES` с помощью окна свойств.  
  
 На этом завершается процесс создания ресурса страницы свойств.  
  
## <a name="adding-code-to-create-and-manage-the-property-page"></a>Добавление кода для создания и управления ими на странице свойств  
 После создания ресурса страницы свойств необходимо написать код реализации.  
  
 Во-первых, включите `CPolyProp` класса, чтобы задать число сторон в объекте при **применить** нажатии кнопки.  
  
#### <a name="to-modify-the-apply-function-to-set-the-number-of-sides"></a>Чтобы изменить функцию применить для задания числа сторон  
  
1.  Замените `Apply` функции в PolyProp.h следующим кодом:  
  
     [!code-cpp[NVC_ATL_Windowing#58](../atl/codesnippet/cpp/adding-a-property-page-atl-tutorial-part-6_1.h)]  
  
 Страница свойств может иметь несколько клиентов, подключенных к нему одновременно, поэтому `Apply` функция циклы вокруг и вызывает `put_Sides` на каждом клиенте со значением, полученные из текстового поля. Вы используете [CComQIPtr](../atl/reference/ccomqiptr-class.md) класс, который выполняет `QueryInterface` для каждого объекта, чтобы получить `IPolyCtl` интерфейс из **IUnknown** интерфейса (хранятся в `m_ppUnk` массива).  
  
 Код теперь проверяет эту настройку `Sides` факт свойство. В случае неудачи, код отображает окно сообщения, отображающее сведения об ошибке из **IErrorInfo** интерфейса. Как правило, контейнер запрашивает объект для **ISupportErrorInfo** интерфейс и вызовы `InterfaceSupportsErrorInfo` первой, чтобы определить, поддерживает ли объект параметра сведений об ошибках. Эту задачу можно пропустить.  
  
 [CComPtr](../atl/reference/ccomptr-class.md) помогает обрабатывая автоматически подсчет ссылок, поэтому не нужно вызывать `Release` в интерфейсе. `CComBSTR`поможет вам с `BSTR` обработки, поэтому необходимо выполнить окончательное `SysFreeString` вызова. Можно также использовать один из различные классы преобразования строк, поэтому можно преобразовать `BSTR` при необходимости (поэтому `USES_CONVERSION` макрос находится в начале функции).  
  
 Также необходимо установить флаг «грязные» страницы свойств для указания того, что **применить** кнопка должна быть включена. Это происходит, когда пользователь изменяет значение в **сторон** "Правка".  
  
#### <a name="to-handle-the-apply-button"></a>Для обработки кнопки «Применить»  
  
1.  В представлении классов щелкните правой кнопкой мыши CPolyProp и нажмите кнопку **свойства** в контекстном меню.  
  
2.  В окне «Свойства» щелкните **события** значок.  
  
3.  Разверните узел `IDC_SIDES` узла в списке событий.  
  
4.  Выберите `EN_CHANGE`и из раскрывающегося меню справа выберите  **\<Добавить > OnEnChangeSides**. `OnEnChangeSides` Объявление обработчика будет добавляться к Polyprop.h и реализация обработчика для Polyprop.cpp.  
  
 Далее предстоит изменить обработчик.  
  
#### <a name="to-modify-the-onenchangesides-method"></a>Чтобы изменить метод OnEnChangeSides  
  
1.  Добавьте следующий код в Polyprop.cpp для `OnEnChangeSides` метод (удаление любой код, который мастер помещены туда):  
  
     [!code-cpp[NVC_ATL_Windowing#59](../atl/codesnippet/cpp/adding-a-property-page-atl-tutorial-part-6_2.cpp)]  
  
 `OnEnChangeSides`будет вызван при **WM_COMMAND** сообщение отправляется с **EN_CHANGE** уведомления для `IDC_SIDES` элемента управления. `OnEnChangeSides`затем вызывает `SetDirty` и передает `TRUE` для указания свойства страницы теперь содержит "грязные" и **применить** кнопка должна быть включена.  
  
## <a name="adding-the-property-page-to-the-control"></a>Добавление страницы свойств для элемента управления  
 Мастер добавления класса ATL и мастер страницы свойств ATL не добавляют страницы свойств в элемент управления для вас автоматически, поскольку в проекте может быть несколько элементов управления. Необходимо добавить запись в схеме сопоставления свойств элемента управления.  
  
#### <a name="to-add-the-property-page"></a>Добавление страницы свойств  
  
1.  Откройте PolyCtl.h и добавьте следующую строку в схеме сопоставления свойств.  
  
     [!code-cpp[NVC_ATL_Windowing#60](../atl/codesnippet/cpp/adding-a-property-page-atl-tutorial-part-6_3.h)]  
  
 Сопоставление свойств элемента управления теперь выглядит следующим образом:  
  
 [!code-cpp[NVC_ATL_Windowing#61](../atl/codesnippet/cpp/adding-a-property-page-atl-tutorial-part-6_4.h)]  
  
 Можно добавить `PROP_PAGE` макрос с CLSID страницы свойств, однако если `PROP_ENTRY` макросов, как показано, `Sides` значение свойства сохраняется при сохранении элемента управления.  
  
 Три параметры макроса — описание свойства DISPID свойства и CLSID страницы свойств, содержащий свойство, на нем. Это полезно в том случае, если, например, загрузки элемента управления в Visual Basic и задать число сторон во время разработки. Так как число сторон сохраняется после перезагрузки проекта Visual Basic, будут восстановлены число сторон.  
  
## <a name="building-and-testing-the-control"></a>Построение и тестирование элемента управления  
 Выполните сборку этого элемента управления и вставить его в тестовом контейнере элемента управления ActiveX. В тестовом контейнере на **изменить** меню, нажмите кнопку **объекта класса PolyCtl**. Откроется страница свойств; Нажмите кнопку **многоугольника** вкладки.  
  
 **Применить** кнопку первоначально будет отключено. Начните вводить значение в **сторон** поле и **применить** станет активной кнопка. После завершения ввода значения щелкните **применить** кнопки. Изменения отображения элемента управления и **применить** снова будет отключена кнопка. Попробуйте ввести недопустимое значение. Появится окно сообщения, содержащее описание ошибки, устанавливаемое из `put_Sides` функции.  
  
 Далее будет поместить элемент управления на веб-странице.  
  
 [Вернитесь к шагу 5](../atl/adding-an-event-atl-tutorial-part-5.md) &#124; [На шаге 7](../atl/putting-the-control-on-a-web-page-atl-tutorial-part-7.md)  
  
## <a name="see-also"></a>См. также  
 [Учебник](../atl/active-template-library-atl-tutorial.md)
