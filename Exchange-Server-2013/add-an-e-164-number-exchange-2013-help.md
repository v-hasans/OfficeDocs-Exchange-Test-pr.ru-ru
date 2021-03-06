﻿---
title: 'Добавление номера E.164: Exchange 2013 Help'
TOCTitle: Добавление номера E.164
ms:assetid: fab86207-be03-40ef-9fea-045a50f3d122
ms:mtpsurl: https://technet.microsoft.com/ru-ru/library/JJ662762(v=EXCHG.150)
ms:contentKeyID: 50556509
ms.date: 05/22/2018
mtps_version: v=EXCHG.150
ms.translationtype: MT
---

# Добавление номера E.164

 

_**Применимо к:** Exchange Online, Exchange Server 2013, Exchange Server 2016_

_**Последнее изменение раздела:** 2012-11-14_

Когда вы включаете для пользователя единую систему обмена сообщениями и привязываете его к абонентской группе E.164, создаются два прокси-адреса единой системы обмена сообщениями Microsoft Exchange. Один адрес содержит добавочный номер пользователя, а другой — номер E.164 для него. Добавочный номер используется, когда пользователь выполняет вызов по номеру голосового доступа к Outlook.

Основной номер E.164, добавленный при включении для пользователя единой системы обмена сообщениями, будет приведен как основной прокси-адрес единой системы обмена сообщениями Microsoft Exchange. При удалении основного номера E.164 первый добавляемый прокси-адрес единой системы обмена сообщениями Microsoft Exchange, который содержит номер E.164 пользователя, будет указан как основной прокси-адрес этой системы. Любые дополнительные номера E.164, которые вы добавляете, будут приведены как дополнительные прокси-адреса данной системы. При добавлении дополнительных номеров E.164 вызывающие могут оставлять голосовую почту для пользователя по всем установленным номерам E.164. Все голосовые сообщения будут доставляться в почтовый ящик того же пользователя.

Добавить основной или дополнительный номер E.164 для пользователя можно с помощью Центра администрирования Exchange или командной консоли. Основной или дополнительный номер E.164 можно добавить на странице **Адрес электронной почты** в почтовом ящике пользователя в Центре администрирования Exchange. Эти номера нельзя добавлять на странице **Почтовый ящик единой системы обмена сообщениями** в Центре администрирования Exchange.

Просмотреть основной и дополнительный номера E.164 для пользователя можно с помощью командлета **Get-UMMailbox** или **Get-Mailbox** в командной консоли.

Дополнительные задачи управления, связанные с пользователями, задействованными для голосовой почты, см. в разделе [Процедуры пользователя голосовой почты](voice-mail-enabled-user-procedures-exchange-2013-help.md).

## Что нужно знать перед началом работы

  - Осталось времени до завершения: 3 минут.

  - Для выполнения этих процедур необходимы соответствующие разрешения. Сведения о необходимых разрешениях см. в статье Запись «Почтовые ящики единой системы обмена сообщениями» в разделе [Разрешения единой системы обмена сообщениями](unified-messaging-permissions-exchange-2013-help.md).

  - Перед выполнением этих процедур убедитесь, что абонентская группа единой системы обмена сообщениями E.164 создана. Дополнительные сведения см. в разделе [Создание абонентской группы единой системы обмена сообщениями](create-a-um-dial-plan-exchange-2013-help.md).

  - Перед выполнением этих процедур убедитесь, что политика почтовых ящиков единой системы обмена сообщениями создана. Дополнительные сведения см. в разделе [Создание политики почтовых ящиков единой системы обмена сообщениями](create-a-um-mailbox-policy-exchange-2013-help.md).

  - Перед выполнением этих процедур убедитесь, что для почтового ящика пользователя включена поддержка единой системы обмена сообщениями, и что ящик связан с абонентской группой E.164. Дополнительные сведения см. в разделе [Включение для пользователя поддержки голосовой почты](enable-a-user-for-voice-mail-exchange-2013-help.md).

  - Прежде чем выполнить эти процедуры, убедитесь, что номер E.164, который будет назначен пользователю, допустим и имеет правильный формат.

  - Сочетания клавиш для процедур, описанных в этой статье, приведены в статье [Сочетания клавиш в Центре администрирования Exchange](keyboard-shortcuts-in-the-exchange-admin-center-exchange-online-protection-help.md).

> [!TIP]  
> Возникли проблемы? Обратитесь за помощью к участникам форумов, посвященных Exchange. Посетите форумы по таким продуктам: <a href="https://go.microsoft.com/fwlink/p/?linkid=60612">Exchange Server</a>, <a href="https://go.microsoft.com/fwlink/p/?linkid=267542">Exchange Online</a> или <a href="https://go.microsoft.com/fwlink/p/?linkid=285351">Exchange Online Protection</a>.. 


## Что необходимо сделать?

## Добавление основного или дополнительного номера E.164 в EAC

1.  В Центре администрирования Exchange выберите пункты **Получатели** \> **Почтовые ящики**.

2.  Выберите из списка почтовый ящик, номер E.164 которого необходимо добавить, и нажмите кнопку **Правка**![Значок редактирования](images/Bb124582.6f53ccb2-1f13-4c02-bea0-30690e6ea71d(EXCHG.150).gif "Значок редактирования").

3.  На странице **Почтовый ящик пользователя** в разделе **Адрес электронной почты** нажмите кнопку **Добавить**![Значок добавления](images/JJ218640.c1e75329-d6d7-4073-a27d-498590bbb558(EXCHG.150).gif "Значок добавления").

4.  На странице **Новый адрес электронной почты** выберите **EUM** и в поле **Адрес и добавочный номер** введите новый номер E.164 пользователя.

5.  На странице **Новый адрес электронной почты** в разделе **Абонентская группа** щелкните **Обзор** для выбора абонентской группы E.164, а затем щелкните **ОК**.

6.  Нажмите кнопку **Сохранить**.

## Использование командной консоли для добавления номера E.164

В этом примере выполняется добавление номера E.164 для пользователя единой системы обмена сообщениями Tony Smith.

> [!NOTE]  
> Прежде чем добавить номер E.164 с помощью командной консоли, необходимо определить позицию прокси-адреса единой системы обмена сообщениями Microsoft Exchange, который требуется добавить. Чтобы определить позицию, используйте команду <strong>$mbx.EmailAddresses</strong>. Первый в списке адрес прокси имеет значение 0. 


    $mbx=Get-Mailbox tony.smith
    $mbx.EmailAddresses.Item(2)="eum:+14255550123;phone-context=MyDialPlan.contoso.com"
    Set-Mailbox tony.smith -EmailAddresses $mbx.EmailAddresses

