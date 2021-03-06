﻿---
title: 'Настройка свойств глобального списка адресов: Exchange 2013 Help'
TOCTitle: Настройка свойств глобального списка адресов
ms:assetid: 5fd2c96f-fe93-4b5a-8495-70c450511a37
ms:mtpsurl: https://technet.microsoft.com/ru-ru/library/Bb232068(v=EXCHG.150)
ms:contentKeyID: 50488122
ms.date: 04/30/2018
mtps_version: v=EXCHG.150
ms.translationtype: HT
---

# Настройка свойств глобального списка адресов

 

_**Применимо к:** Exchange Online, Exchange Server 2013_

_**Последнее изменение раздела:** 2014-12-16_

В этом разделе объясняется, как изменить параметры глобального списка адресов (GAL).

Дополнительные сведения о задачах управления, связанных со списками адресов, см. в разделе [Процедуры списка адресов](address-list-procedures-exchange-2013-help.md).

## Что нужно знать перед началом работы

  - Предполагаемое время для завершения каждой процедуры: 5 минут.

  - Для выполнения этих процедур необходимы соответствующие разрешения. Сведения о необходимых разрешениях см. в статье Запись "Списки адресов" в разделе [Разрешения для электронных адресов и адресных книг](email-address-and-address-book-permissions-exchange-2013-help.md).

  - По умолчанию Exchange Online роль "Список адресов" не назначена ни одной из групп ролей. Чтобы использовать командлеты, для которых требуется эта роль, ее необходимо добавить в группу ролей. Дополнительные сведения см. в разделе "Добавление роли в группу ролей" статьи [Управление группами ролей](manage-role-groups-exchange-2013-help.md).

  - Нельзя изменить параметры глобального списка адресов, используемого по умолчанию.

  - Невозможно использовать Центр администрирования Exchange (EAC) для выполнения этой процедуры. Необходимо использовать командную консоль.

  - Сочетания клавиш для процедур, описанных в этой статье, приведены в статье [Сочетания клавиш в Центре администрирования Exchange](keyboard-shortcuts-in-the-exchange-admin-center-exchange-online-protection-help.md).

> [!TIP]  
> Возникли проблемы? Обратитесь за помощью к участникам форумов, посвященных Exchange. Посетите форумы по таким продуктам: <a href="https://go.microsoft.com/fwlink/p/?linkid=60612">Exchange Server</a>, <a href="https://go.microsoft.com/fwlink/p/?linkid=267542">Exchange Online</a> или <a href="https://go.microsoft.com/fwlink/p/?linkid=285351">Exchange Online Protection</a>.


## Использование командной консоли для настройки свойств глобального списка адресов

В этом примере глобальному списку адресов с идентификатором GUID 96d0c505-eba8-4103-ad4f-577a1bf4ad7b назначается новое имя FourthCoffee.

    Set-GlobalAddressList -Identity 96d0c505-eba8-4103-ad4f-577a1bf4ad7b -Name FourthCoffee

> [!NOTE]  
> Если используются свойства предустановленного условного фильтра, значение параметра <em>IncludedRecipients</em> не может быть пустым.


В этом примере показано, как получатели, включаемые в глобальный список адресов Fourth Coffee, изменяются на тех получателей, для компании которых установлено значение Fourth Coffee.

    Set-GlobalAddressList -Identity Fourth Coffee -RecipientFilter {Company -eq "Fourth Coffee"}

Подробные сведения о синтаксисе и параметрах см. в разделе [Set-GlobalAddressList](https://technet.microsoft.com/ru-ru/library/bb123877\(v=exchg.150\)).

