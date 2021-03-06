---
title: 1. Введение | Документация Майкрософт
ms.custom: ''
ms.date: 11/04/2016
ms.technology:
- cpp-parallel
ms.topic: conceptual
dev_langs:
- C++
ms.assetid: c42e72bc-0e31-4b1c-b670-cd82673c0c5a
author: mikeblome
ms.author: mblome
ms.workload:
- cplusplus
ms.openlocfilehash: 4ce963d312d145e26567a5902f32e45735eb1d89
ms.sourcegitcommit: 799f9b976623a375203ad8b2ad5147bd6a2212f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2018
ms.locfileid: "46438422"
---
# <a name="1-introduction"></a>1. Вступление

В этом документе определяет коллекцию директивы компилятора, библиотечные функции и переменные среды, которые могут использоваться для указания общей памяти параллелизма в программах на C и C++. Возможности, описываемые в этом документе которые в совокупности называются *OpenMP C/C++ приложения программа интерфейс (API)*. Цель этой спецификации — предоставить модель параллельного программирования, который позволяет программам можно переносить на другие архитектуры общей памяти от разных поставщиков. API OpenMP C/C++ будет поддерживаться компиляторами у множества поставщиков. Дополнительные сведения о OpenMP, включая *OpenMP Fortran прикладной программный интерфейс*, можно найти на веб-узла:

[http://www.openmp.org](http://www.openmp.org)

Директивы, библиотечные функции и переменные среды, определенные в этом документе позволит пользователям создавать и управлять ими параллельных программ одновременно разрешая переносимости. Директивы расширить C последовательного программирования C++ модель и с одной программы несколько конструкций данных (SPMD), конструкции совместной работы и структур синхронизации, и они обеспечивают поддержку для совместного использования и приватизация данных. Компиляторы, которые поддерживают API OpenMP C и C++ API будет включать параметр командной строки для компилятора, который активирует и позволяет интерпретацию все директивы компилятора OpenMP.