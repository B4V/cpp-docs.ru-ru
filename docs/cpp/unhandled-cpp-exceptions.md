---
title: Необработанные исключения C++ | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-language
ms.topic: language-reference
dev_langs:
- C++
helpviewer_keywords:
- event handlers [C++], unhandled exceptions
- catch keyword [C++], handler not found
- exceptions [C++], unhandled
- C++ exception handling, unhandled exceptions
- unhandled exceptions [C++]
ms.assetid: 13f09c53-9254-4407-9db9-14e730e047cc
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 57d014762ebc5427ccc4b9d26fff75addc883759
ms.sourcegitcommit: 913c3bf23937b64b90ac05181fdff3df947d9f1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2018
ms.locfileid: "46097774"
---
# <a name="unhandled-c-exceptions"></a>Необработанные исключения C++

Если подходящий обработчик (или кнопку с многоточием **catch** обработчик) не удается найти для текущего исключения, предопределенный `terminate` вызове функции времени выполнения. (Функцию `terminate` также можно явным образом вызвать из любого обработчика.) Действие по умолчанию для `terminate` заключается в том, что она вызывает функцию `abort`. Если вам необходимо, чтобы перед выходом из приложения функция `terminate` в вашей программе вызывала какую-то другую функцию, вызовите функцию `set_terminate`, указав в качестве ее единственного аргумента ту функцию, которую нужно вызвать. Функцию `set_terminate` можно вызвать из любого места программы. `terminate` Подпрограмма всегда вызывает последнюю функцию, заданную в качестве аргумента для `set_terminate`.

## <a name="example"></a>Пример

В следующем примере создается исключение типа `char *`, однако в нем нет обработчика, предназначенного для перехвата исключений `char *`. Вызов `set_terminate` содержит инструкцию, согласно которой `terminate` вызывает функцию `term_func`.

```cpp
// exceptions_Unhandled_Exceptions.cpp
// compile with: /EHsc
#include <iostream>
using namespace std;
void term_func() {
   cout << "term_func was called by terminate." << endl;
   exit( -1 );
}
int main() {
   try
   {
      set_terminate( term_func );
      throw "Out of memory!"; // No catch handler for this exception
   }
   catch( int )
   {
      cout << "Integer exception raised." << endl;
   }
   return 0;
}
```

## <a name="output"></a>Вывод

```Output
term_func was called by terminate.
```

Функция `term_func` должна завершать программу или текущий поток (желательно путем вызова функции `exit`). Если вместо этого она возвращает управление вызвавшему объекту, то вызывается функция `abort`.

## <a name="see-also"></a>См. также

[Обработка исключений С++](../cpp/cpp-exception-handling.md)