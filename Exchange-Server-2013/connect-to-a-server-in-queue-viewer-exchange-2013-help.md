﻿---
title: 'Подключение к серверу в средстве просмотра очереди: Exchange 2013 Help'
TOCTitle: Подключение к серверу в средстве просмотра очереди
ms:assetid: 6c1ad574-9ab5-4dcc-9398-ec10eca4fd11
ms:mtpsurl: https://technet.microsoft.com/ru-ru/library/Aa998669(v=EXCHG.150)
ms:contentKeyID: 50488192
ms.date: 04/30/2018
mtps_version: v=EXCHG.150
ms.translationtype: HT
---

# Подключение к серверу в средстве просмотра очереди

 

_**Применимо к:** Exchange Server 2013_

_**Последнее изменение раздела:** 2012-10-03_

При использовании средства просмотра очередей в наборе инструментов Exchange на сервере Microsoft Exchange Server 2013, расположенном в организации Exchange, можно подключиться к другим серверам почтовых ящиков. По умолчанию при открытии средства просмотра очередей на сервере почтовых ящиков оно подключается к базе данных очередей на локальном сервере. При этом можно запустить несколько экземпляров средства просмотра очередей, чтобы разные экземпляры подключались к разным серверам. Чтобы облегчить одновременное наблюдение за несколькими серверами почтовых ящиков, также можно расположить на экране окна средства просмотра очереди в мозаичном порядке.

В средстве просмотра очередей можно также указать сервер, который используется удаленной средой PowerShell для выполнения задач. Этот сервер не обязательно должен совпадать с удаленным сервером, которым вы управляете в средстве просмотра очередей.

## Что нужно знать перед началом работы?

  - Осталось времени до завершения: 5 минут

  - Для выполнения этих процедур необходимы соответствующие разрешения. Сведения о необходимых разрешениях см. в статье Запись "Очереди" в разделе [Разрешения потока обработки почты](mail-flow-permissions-exchange-2013-help.md).

  - Процедуры, описанные в этом разделе, не относятся к пограничным транспортным серверам. При использовании средства просмотра очереди на пограничном транспортном сервере невозможно изменить фокус средства.

  - Сочетания клавиш для процедур, описанных в этой статье, приведены в статье [Сочетания клавиш в Центре администрирования Exchange](keyboard-shortcuts-in-the-exchange-admin-center-exchange-online-protection-help.md).

> [!TIP]  
> Возникли проблемы? Обратитесь за помощью к участникам форумов, посвященных Exchange. Посетите форумы по таким продуктам: <a href="https://go.microsoft.com/fwlink/p/?linkid=60612">Exchange Server</a>, <a href="https://go.microsoft.com/fwlink/p/?linkid=267542">Exchange Online</a> или <a href="https://go.microsoft.com/fwlink/p/?linkid=285351">Exchange Online Protection</a>.


## Что необходимо сделать?

## Использование набора инструментов Exchange для указания сервера, которым требуется управлять в средстве просмотра очередей

1.  Нажмите кнопку **Пуск** и последовательно выберите пункты **Все программы** \> **Microsoft Exchange Server 2013** \> **Панель элементов Exchange**.

2.  В разделе **Средства для потока почты** дважды щелкните элемент **Средство просмотра очереди**.

3.  В области действий щелкните пункт **Подключиться к серверу**.

4.  В окне **Подключение к серверу** нажмите кнопку **Обзор**, чтобы просмотреть список доступных серверов почтовых ящиков.

5.  В окне **Выбор сервера Exchange** выберите сервер почтовых ящиков. Чтобы провести поиск сервера почтовых ящиков, используйте один из следующих процедур:
    
      - Введите точное имя сервера или первые несколько букв имени сервера в поле **Поиск** и щелкните **Найти**. Выберите сервер в области результатов.
    
      - В меню **Вид** выберите пункт **Показать фильтр**. В столбце **Имя** или столбце **Версия** щелкните значок фильтра, а затем выберите оператор фильтра. Введите критерии фильтрации в поле **Ввод текста**. Нажмите клавишу ВВОД. Выберите сервер в области результатов.

6.  Нажмите кнопку **ОК**, чтобы закрыть окно **Выбор сервера Exchange Server**.

7.  После выбора сервера для того, чтобы при каждом открытии средства просмотра очереди фокус находился на этом сервере, установите в окне **Подключение к серверу** флажок **Установить в качестве сервера по умолчанию**.

8.  В окне **Подключение к серверу** нажмите кнопку **Подключить**.

## Использование набора инструментов Exchange для указания сервера, который средство просмотра очередей использует для запуска удаленной среды PowerShell

1.  Нажмите кнопку **Пуск** и последовательно выберите пункты **Все программы** \> **Microsoft Exchange Server 2013** \> **Панель элементов Exchange**.

2.  В разделе **Средства для потока почты** дважды щелкните элемент **Средство просмотра очереди**.

3.  В области действий выберите пункт **Свойства**.

4.  В диалоговом окне **Средство просмотра очереди — свойства \<имя сервера\>** выберите один из следующих параметров:
    
      - **Подключиться к автоматически выбранному серверу**   Выберите данный параметр для автоматического подключения к серверу для управления очередями через удаленную среду PowerShell.
    
      - **Укажите сервер для подключения**   Выберите данный параметр, чтобы указать сервер для запуска удаленной командной консоли PowerShell. При выборе данного параметра нажмите кнопку **Обзор**, чтобы открыть диалоговое окно **Выбор сервера Exchange**. Выберите сервер, на котором будет запущена удаленная среда PowerShell, а затем щелкните **ОК**.

## Как проверить, что все получилось?

Вы сможете управлять очередями на указанном сервере почтовых ящиков.

