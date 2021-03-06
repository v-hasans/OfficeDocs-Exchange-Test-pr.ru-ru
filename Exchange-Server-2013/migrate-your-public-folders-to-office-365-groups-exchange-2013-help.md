﻿---
title: 'Перенос общедоступных папок в группы Office 365: Exchange 2013 Help'
TOCTitle: Перенос общедоступных папок в группы Office 365
ms:assetid: d89e727b-675a-4623-b572-260f8b44b966
ms:mtpsurl: https://technet.microsoft.com/ru-ru/library/Mt843872(v=EXCHG.150)
ms:contentKeyID: 74468732
ms.date: 05/22/2018
mtps_version: v=EXCHG.150
ms.translationtype: MT
---

# Перенос общедоступных папок в группы Office 365

 

_**Применимо к:** Exchange Online, Exchange Server 2010, Exchange Server 2013_

_**Последнее изменение раздела:** 2017-09-25_

**Сводка.** Аргументы за и против переноса общедоступных папок Exchange в группы Office 365.

В этой статье представлено сравнение общедоступных папок и групп Office 365, а также указаны причины, по которым то или иное решение может лучше подходить для вашей организации. Общедоступные папки существовали с первого выпуска Exchange, а служба "Группы Office 365" появилась только недавно. Если вы хотите перенести все общедоступные папки (или некоторые из них) в группы Office 365, то в этой статье вы найдете описание процесса и ссылки на статьи с пошаговыми инструкциями.

## Что такое общедоступные папки?

[Общедоступные папки](public-folders-exchange-2013-help.md) содержат различные данные, упорядоченные в виде иерархической структуры.

Ниже указаны ситуации, в которых не рекомендуется использовать общедоступные папки.

  - **Архивация данных.** Пользователи с ограничениями почтовых ящиков иногда используют для архивации общедоступные папки, а не почтовые ящики. Этого делать не рекомендуется, так как это приводит к увеличению занимаемого пространства в общедоступных папках и лишает смысла использование ограничений для почтовых ящиков.

  - **Общий доступ к документам и совместная работа.** Общедоступные папки не предоставляют возможностей управления документами, таких как управление версиями, контролируемые извлечение и возврат, а также автоматические уведомления об изменениях содержимого.

## Что такое служба "Группы Office 365"?

Благодаря группам Office 365 вы можете выбрать пользователей для совместной работы и легко настроить коллекцию ресурсов для них. Вам не придется вручную назначать разрешения для этих ресурсов, так как при добавлении членов группы они автоматически получают разрешения, необходимые для доступа к инструментам и ресурсам группы. Такие группы также упрощают выполнение задач, для которых раньше использовались списки рассылки и общие почтовые ящики.

Полное описание групп см. в статье [Узнайте о группах в Office 365](https://go.microsoft.com/fwlink/p/?linkid=858521).

## Следует ли переносить общедоступные папки в группы Office 365?

Служба "Группы Office 365" — это новейшее решение для совместной работы от корпорации Майкрософт. Это означает, что есть много причин использовать его вместо общедоступных папок, намного более старой технологии. Например, в Outlook такие группы могут полностью заменить общедоступные папки, поддерживающие почту. Невозможно составить полный список сценариев, в которых группы Office 365 работают лучше, чем общедоступные папки. Ниже представлены некоторые наглядные примеры.

  - **Совместная работа с электронной почтой.** Для групп в Outlook существует специальный раздел **Беседы**, где хранятся все сообщения, а пользователи могут совместно работать с ними. Группу даже можно настроить на получение сообщений от пользователей, не состоящих в группе или в организации. Например, если в настоящее время вы используете общедоступные папки, поддерживающие почту, для хранения обсуждений проектов или заказов на покупку, которые должны быть доступны нескольким людям, то использовать группы будет предпочтительнее. Кроме того, группы лучше подходят для тех случаев, когда вам просто нужно публиковать сведения для нескольких пользователей.

  - **Совместная работа с документами.** В Outlook для групп Office 365 есть специальная вкладка **Файлы**, на которой отображаются все файлы с сайта группы SharePoint и из почтовых вложений. Все файлы отображаются в одном представлении, и их не приходится искать повсюду, как в общедоступных папках. Совместное редактирование также становится проще. Если вы используете общедоступные папки для хранения файлов, предназначенных для использования несколькими людьми, рассмотрите возможность миграции в службу "Группы Office 365".

  - **Общий календарь.** После создания каждой группы ей назначается общий календарь. Любой член группы может создавать события в этом календаре. Когда вы добавляете группу в избранное, календарь этой группы может отображаться наряду с вашим личным календарем. Вы также можете подписаться на события группы. В этом случае события, созданные в соответствующей группе, отображаются в вашем личном календаре. Если вы размещаете в общедоступных папках календари для своей команды, например, чтобы у нее был доступ к расписанию или графику, то служба "Группы Office 365" также расширит ваши возможности.

  - **Упрощенные разрешения.** При назначении пользователей группе они сразу получают необходимые им разрешения, а в случае общедоступных папок требуется назначать разрешения вручную. Пользователей можно добавлять в качестве владельцев или членов группы. У владельцев есть все права в группе, включая возможность выполнять операции по управлению группой. Члены группы могут создавать содержимое и редактировать файлы, как и владельцы, но не могут удалять содержимое, созданное другими пользователями. Если модель разрешений для общедоступных папок слишком сложна для вас и вам нужно что-то более простое и удобное, "Группы Office 365" — то, что вам нужно.

  - **Поддержка мобильных устройств и Интернета.** К общедоступным папкам невозможно получать доступ с мобильных устройств, а в Интернете доступен только ограниченный набор функций. С другой стороны, группы Office 365 доступны через мобильные приложения Outlook, а в Интернете предоставляется более широкий набор возможностей. Если члены вашей команды постоянно путешествуют и им нужен мобильный доступ, то следует использовать службу "Группы Office 365".

  - **Доступ к широкому ряду приложений Office 365.** При создании группы открывается доступ к широкому ряду приложений из набора Office 365. Вы получаете сайт группы SharePoint для хранения файлов и расписание в Планировщике для отслеживания задач. "Группы Office 365" — служба, предусматривающая наличие членства, в которой совмещаются различные элементы набора Office 365.

У службы "Группы Office 365" много преимуществ, но следует учитывать несколько значительных отличий, которые станут заметны после отказа от общедоступных папок. Ниже перечислены основные отличия.

  - **Иерархия папок.** Общедоступные папки часто применяются для упорядочивания содержимого с использованием многоуровневой иерархии, но структура службы "Группы Office 365" одноуровневая. Все сообщения группы хранятся в разделе бесед, а все документы — на вкладке **Файлы**. Кроме того, в группах Office 365 невозможно создавать вложенные папки.

  - **Роли с различными разрешениями.** Для общедоступных папок предусмотрено множество ролей с различными разрешениями, а для групп Office 365 — только две (владелец и член группы).

Прежде чем переходить на "Группы Office 365", также рекомендуем учесть различные ограничения, связанные с созданием и обслуживанием групп. Дополнительные сведения см. в разделе *Как можно управлять группами?* статьи [Узнайте о группах в Office 365](https://go.microsoft.com/fwlink/p/?linkid=858521).

## Перенос общедоступных папок в службу "Группы Office 365"

Если вы решите перейти на "Группы Office 365", можно использовать так называемую *пакетную миграцию*, чтобы переместить содержимое электронной почты и календаря из имеющихся общедоступных папок в эту службу. Конкретный способ запуска пакетной миграции зависит от того, в какой версии Exchange на данный момент размещается иерархия общедоступных папок. В конце этой статьи вы найдете ссылки на пошаговые инструкции по пакетной миграции.

> [!NOTE]  
> По завершении переноса общедоступной папки, поддерживающей почту, в определенную группу в Office 365 все сообщения, адресованные общедоступной папке, будет получать группа.


Ниже перечислены ключевые преимущества пакетной миграции.

  - **Миграция с использованием службы репликации почтовых ящиков (MRS).** При миграции используются командлеты для работы с пакетами миграции. В одном пакете миграции можно запустить миграцию в несколько групп. Кроме того, доступны скрипты, которые помогут вам выполнить миграцию.

  - **Поддержка общедоступных папок почты и календаря.** Скопированные сообщения и публикации будут отображаться как групповые чаты, а скопированные элементы календаря — в календарях группы. Для других типов общедоступных папок, например с задачами и контактами, в настоящее время не поддерживается такая миграция.

  - **Локальные общедоступные папки можно переносить непосредственно в "Группы Office 365".** При такой миграции не требуется перемещать общедоступные папки сначала в Office 365, а затем в "Группы Office 365". Командлеты для копирования данных MRS считывают данные общедоступных папок непосредственно из локальной среды, а затем копируют их в группы Office 365. Обратите внимание, что для общедоступных папок Exchange 2010 потребуется конечная точка мобильного Outlook. Для общедоступных папок Exchange 2013 и Exchange 2016 необходима конечная точка на основе прокси MRS.

  - **Переносить все сразу не обязательно.** Вы можете выбрать определенные общедоступные папки, которые будут перенесены в "Группы Office 365".

  - **Копирование данных за один подход.** Пакетная миграция — это одноразовое копирование данных из исходных общедоступных папок в целевые группы, не обремененное добавочной синхронизацией и окончательной обработкой.

  - **Объединение данных общедоступных папок с имеющимися данными в группе.** При копировании данных содержимое общедоступных папок объединяется с имеющимся содержимым группы (если оно есть). Если требуется добавочное копирование данных, вы можете запускать эту операцию сколько угодно раз. При этом в группу будут скопированы дополнительные данные.

## Обзор пакетной миграции

Ниже перечислены основные этапы переноса содержимого общедоступных папок в группы Office 365 при пакетной миграции. Подробности представлены в перечисленных ниже статьях.

1.  **Выбор исходного объекта:**  выберите общедоступные папки, которые требуется перенести. Вы можете выбрать любую папку, содержащую почту или календарь.

2.  **Создание целевого объекта:**  создайте для папок соответствующие группы с нужными настройками (например, с заданными членами групп, параметрами конфиденциальности и классификации данных).

3.  **Копирование данных:**  скопируйте данные из общедоступных папок в "Группы Office 365" с помощью командлетов пакетной миграции.

4.  **Блокировка исходного объекта:**  проверив данные в группах, заблокируйте общедоступные папки.

5.  **Перенос:**  скопируйте все новые данные, созданные на этапах 3 и 4.

Обратите внимание на то, что общедоступные папки и соответствующие им группы останутся доступны пользователям во время этапов 1–3. После этапа 3 вы можете определить целесообразность продолжения миграции, проанализировав удобство работы со службой "Группы Office 365" и решив, подходит ли она для пользователей и организации. На этом этапе вы можете откатить миграцию и вернуться к использованию общедоступных папок. Если вы продолжите миграцию, то по завершении этапа 5 вы можете удалить исходные общедоступные папки. Даже после миграции можно вернуться к общедоступным папкам, если вы сохраните файлы резервной копии и не удалите исходные общедоступные папки.

## Необходимые условия и пошаговые инструкции по пакетной миграции

Ниже перечислены необходимые условия для пакетной миграции в среде Exchange. Конкретные требования зависят от используемой в данный момент версии Exchange.

1.  Если общедоступные папки находятся в локальной среде, то серверы должны работать под управлением одной из следующих версий:
    
      - Exchange 2010 с пакетом обновления 3 (SP3) и накопительным пакетом обновления 8 (RU8) или более поздней версии;
    
      - Exchange 2013 с накопительным пакетом обновления 15 (CU15) или более поздней версии;
    
      - Exchange 2016 с накопительным пакетом обновления 4 (CU4) или более поздней версии.

2.  Если общедоступные папки находятся в локальной среде, должна быть настроена гибридная среда Exchange. Дополнительные сведения см. в статье [Гибридные развертывания Exchange Server](https://technet.microsoft.com/ru-ru/library/jj200581\(v=exchg.150\)).

**Инструкции по миграции**

Чтобы получить пошаговые инструкции по запуску пакетной миграции, выберите соответствующую ссылку ниже.

  - [Use batch migration to migrate Exchange Online public folders to Office 365 Groups](https://technet.microsoft.com/ru-ru/library/mt843871\(v=exchg.150\))

  - [Использование пакетной миграции для переноса общедоступных папок Exchange 2010 в группы Office 365](use-batch-migration-to-migrate-exchange-2010-public-folders-to-office-365-groups-exchange-2013-help.md)

  - [Использование пакетной миграции для переноса общедоступных папок Exchange 2013 в группы Office 365](use-batch-migration-to-migrate-exchange-2013-public-folders-to-office-365-groups-exchange-2013-help.md)

  - [Перенос общедоступных папок Exchange 2016 в "Группы Office 365" с помощью пакетной миграции](https://go.microsoft.com/fwlink/p/?linkid=859171)

