---
title: Предоставление активации без окна | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-mfc
ms.topic: conceptual
dev_langs:
- C++
helpviewer_keywords:
- windowless activation of MFC ActiveX controls
- activation [MFC], MFC ActiveX controls
- MFC ActiveX controls [MFC], activate options
- activation [MFC], windowless
ms.assetid: 094903b5-c344-42fa-96ff-ce01e16891c5
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 8e8fc079921b3f2eddd117f93ee9d2f6cad60925
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46441232"
---
# <a name="providing-windowless-activation"></a>Предоставление активации без окна

Окно создания кода (то есть все, что происходит при вызове `CreateWindow`) является затратным, для выполнения. Элемент управления, который поддерживает на экране окно приходится управлять сообщения окна. Элементы управления без окон таким образом происходит быстрее, чем элементы управления с windows.

Дополнительные элементы управления без окон удобен тем, что в отличие от оконными элементами управления, элементы управления без окон поддерживает прозрачное Рисование и области непрямоугольное экрана. Распространенным примером прозрачный элемент управления является элементом управления "текст" с прозрачным фоном. Элементы управления закрашивает текст, но не фоновом режиме, поэтому все, что находится под текстом видно. Более новые форм часто делают использовать непрямоугольных элементов управления, например кнопки со стрелками и округление кнопок.

Часто элемент управления не требуется собственного окна и, вместо этого можно использовать для служб Windows контейнера, при условии, что контейнер записан в поддерживающих объекты. Элементы управления без окон обладают обратной совместимостью с более старой контейнерами. В более старых контейнеры не написано для поддержки элементов управления без окон элементы управления без окон создать окно, в активном состоянии.

Поскольку элементы управления без окон не имеют собственные окна, контейнер (установить окно) отвечает за предоставление служб, которые бы в противном случае были предоставлены с помощью элемента управления собственного окна. Например если элемент управления должен запросить фокус клавиатуры, захвата мыши или получения контекста устройства, эти операции управляются контейнером. Контейнер направляет сообщения ввода пользователя, отправляемые его окна для соответствующего элемента управления без окон, с помощью `IOleInPlaceObjectWindowless` интерфейс. (См. в разделе *ActiveX SDK* описание этого интерфейса.) `COleControl` функции-члены вызывают эти службы из контейнера.

Чтобы сделать элемент управления использовать активации без окна, включите **windowlessActivate** флаг в набор флагов, возвращенный [COleControl::GetControlFlags](../mfc/reference/colecontrol-class.md#getcontrolflags). Пример:

[!code-cpp[NVC_MFC_AxOpt#5](../mfc/codesnippet/cpp/providing-windowless-activation_1.cpp)]
[!code-cpp[NVC_MFC_AxOpt#6](../mfc/codesnippet/cpp/providing-windowless-activation_2.cpp)]
[!code-cpp[NVC_MFC_AxOpt#7](../mfc/codesnippet/cpp/providing-windowless-activation_3.cpp)]

Код, включив этот флаг создается автоматически при выборе **активации без окна** параметр [параметры управления](../mfc/reference/control-settings-mfc-activex-control-wizard.md) страницы мастера элементов управления ActiveX MFC.

При включении активации без окна контейнера делегирует входящие сообщения к элементу управления `IOleInPlaceObjectWindowless` интерфейс. `COleControl`в реализации этого интерфейса отправляет сообщения через схему сообщений элемента управления, после настройки мыши координирует соответствующим образом. Сообщения, как и обычные окна сообщения, можно обработать, добавив соответствующие записи в схеме сообщений. В вашей обработчики для этих сообщений, избегайте использования *m_hWnd* переменную-член (или любой использующей ее функция-член), что его значение не равно **NULL**.

`COleControl` предоставляет функции-члены, которые вызывают захват мыши, фокус клавиатуры, прокрутка и другие окна службы из контейнера соответствующим образом, включая:

- [При получении фокуса](../mfc/reference/colecontrol-class.md#getfocus), [SetFocus](../mfc/reference/colecontrol-class.md#setfocus)

- [GetCapture](../mfc/reference/colecontrol-class.md#getcapture), [SetCapture](../mfc/reference/colecontrol-class.md#setcapture), [ReleaseCapture](../mfc/reference/colecontrol-class.md#releasecapture)

- [GetDC](../mfc/reference/colecontrol-class.md#getdc), [ReleaseDC](../mfc/reference/colecontrol-class.md#releasedc)

- [InvalidateRgn](../mfc/reference/colecontrol-class.md#invalidatergn)

- [ScrollWindow](../mfc/reference/colecontrol-class.md#scrollwindow)

- [Метода GetClientRect](../mfc/reference/colecontrol-class.md#getclientrect)

В элементы управления без окон, следует всегда использовать `COleControl` функций-членов вместо соответствующего `CWnd` функции-члены и их связанные функции Win32 API.

Вы можете безоконный элемент управления, чтобы быть целевым объектом операции перетаскивания и вставки OLE. Как правило это потребует, что окна элемента управления быть зарегистрирована в качестве целевого объекта перетаскивания. Так как элемент управления не имеет окна свои собственные, контейнер использует отдельное окно в качестве целевого объекта перетаскивания. Элемент управления предоставляет реализацию `IDropTarget` интерфейс, к которому контейнера можно делегировать вызовы в соответствующее время. Чтобы предоставить этот интерфейс для контейнера, переопределите [COleControl::GetWindowlessDropTarget](../mfc/reference/colecontrol-class.md#getwindowlessdroptarget). Пример:

[!code-cpp[NVC_MFC_AxOpt#8](../mfc/codesnippet/cpp/providing-windowless-activation_4.cpp)]

## <a name="see-also"></a>См. также

[Элементы ActiveX в MFC. Оптимизация](../mfc/mfc-activex-controls-optimization.md)

