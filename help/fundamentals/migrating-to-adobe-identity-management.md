---
title: Migration zu Adobe Identity Management
description: Beschreibung in Kürze verfügbar.
role: User
level: Beginner
hide: true
hidefromtoc: true
feature: Marketing
exl-id: 8368a148-c0c8-462f-b166-9efc412c4a0f
source-git-commit: fe760c2fc53b96d5c176de377730bce2e89dbc74
workflow-type: tm+mt
source-wordcount: '1079'
ht-degree: 0%

---

# Migration zu Adobe Identity Management

Adobe verbessert die Verwaltung Ihrer Adobe Marketo Engage-Abonnements und -Benutzer. Wir steigern die Produktivität für Sie und Ihr Unternehmen, indem wir Ihre Marketo Engage-Abonnements und -Benutzer in die Adobe Admin Console migrieren.

In diesem Tutorial können Sie durch die Migration navigieren, sodass Sie Adobe Marketo Engage gemeinsam mit anderen Adobe-Konten und -Produkten für Ihre Benutzer an einem zentralen Ort verwalten können. Die Migration ist erforderlich und hat keine Auswirkungen auf Ihren Marketing-Workflow, Ihre Inhalte, Integrationen oder Assets.

## Checkliste für die Vormigration für Marketo Engage-Administratoren {#pre-migration-checklist-for-marketo-engage-administrators}

Um sicherzustellen, dass Ihr Unternehmen Adobe Marketo Engage in die Adobe Admin Console migrieren kann, empfehlen wir Ihnen, die unten stehende Checkliste zu befolgen, um die bevorstehenden Änderungen zu verwalten.

### 1. Identifizieren Sie Ihre Systemadministratoren und besprechen Sie die für sie erforderlichen Maßnahmen. {#identify-your-system-administrators}

* Wenn Sie sich nicht sicher sind, welche Systemadministratoren sich in Ihrem Unternehmen befinden, wenden Sie sich an Ihr Adobe Account-Team oder wenden Sie sich an den Adobe-Support `marketocares@marketo.com`.

* Bestätigen Sie die Adobe Admin Console (oder Adobe-Org), zu der Ihre Marketo Engage-Abonnements migriert werden sollen.  Marketo Engage-Abonnements müssen im selben Unternehmen wie Dynamic Chat bereitgestellt werden, einem nativen Tool zur Automatisierung von Konversationen, das mit Marketo Engage integriert ist.
  `TBD LINK TO https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console#subscription-migration-complete`

* Weitere Informationen zur Kommunikation mit Ihren Systemadministratoren finden Sie im Abschnitt [Beispiel-E-Mail](#announce-the-migration-timeline).

### 2. Machen Sie sich mit den Änderungen und Auswirkungen der Migration zur Adobe Identity vertraut. {#familiarize-yourself-with-the-changes}

Im folgenden Video führt Sie das Marketo Engage Product Management-Team durch die Migration und durch die Journey.

>[!VIDEO](https://video.tv.adobe.com/v/3430920t3/?quality=12&learn=on){transcript=true}

Weitere Informationen zu diesem Thema für Marketo Engage-Administratoren finden Sie in den folgenden Hilfeartikeln:

* [Checkliste für die Benutzereinrichtung](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/user-setup){target="_blank"}

* [Adobe Identity Management-Übersicht ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"}

* [Grundlegendes zur Marketo-Anmeldung und Benutzermigration zur Adobe Admin Console](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console){target="_blank"}

* [Migration zur Adobe Identity mit der Migrationskonsole](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity){target="_blank"}

* [Grundlegendes zur Verwendung von Adobe Admin Console](https://helpx.adobe.com/de/enterprise/using/admin-console.html){target="_blank"}

### 3. Ankündigung des Zeitplans und der Vorbereitung der Migration für Ihre internen Teams {#announce-the-migration-timeline}

* Markieren Sie das Migrationsdatum einmal in den Kalendern Ihrer Marketo Engage-Administratoren und -Benutzer.

Sie können das Migrationsdatum in &quot;**Admin**&quot;> &quot;**Migrationskonsole**&quot;> &quot;**Vormigration**&quot; ändern, um es besser an Ihre interne Zeitleiste anzupassen. Erfahren Sie mehr über die Neuplanung und die Einschränkungen von [Ändern des Migrationsdatums](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity#pre-migration){target="_blank"}.

* Senden Sie eine E-Mail zur Kommunikation mit Ihren Systemadministratoren.

Nachfolgend finden Sie eine Beispiel-E-Mail, die Sie an Ihre Systemadministratoren senden können. In der Regel verwaltet Ihre IT-Abteilung alle Adobe-Lizenzen.

`---------------------------------------------------`

**Betreff: Unterstützt erforderlich - Migration von Marketo Engage-Abonnements zu Adobe Admin Console**

Sehr geehrte `[IT Administrator/NAME]`,

Unser Marketo Engage-Abonnement wird bald in das Adobe Identity Management System migriert. Der `[Marketing Operation team]` benötigt Ihre Hilfe, um einige erforderliche Schritte vor Beginn der Benutzermigration abzuschließen, um die Auswirkungen auf Marketo Engage-Benutzer zu minimieren.

`1.` Bestätigen Sie, ob das Unternehmen bereits andere Adobe-Produkte in Adobe Admin Console(s) verwaltet und ob Marketo Engage in dieselbe Konsole migriert wird.

* Beachten Sie, dass Marketo Engage-Abonnements in derselben Organisation wie Dynamic Chat, einem nativen Tool zur Automatisierung von Konversationen, das mit Marketo Engage integriert ist, erstellt werden müssen.

* Wenn Sie Bedenken oder Fragen bezüglich der Admin Console haben, zu der Marketo Engage hinzugefügt wird, wenden Sie sich bitte an das Supportteam unter `marketocares@marketo.com` und nehmen Sie uns in Ihre Mitteilung auf.

`2.` Suchen Sie auf der Suche nach einer E-Mail von Adobe mit der Betreffzeile &quot;Aktion erforderlich für die Verwaltung des Benutzerzugriffs auf Adobe Marketo Engage `[Package Tier]`&quot;. Diese E-Mail wurde gesendet, nachdem auf unserer Admin Console Marketo Engage-Lizenzen bereitgestellt wurden. Diese E-Mail erhalten nur Systemadministratoren. Bitte informieren Sie uns umgehend, wann Sie es erhalten.

* Adobe kann die Zustimmung von Ihnen, dem Systemadministrator der Admin Console, einholen, um Benutzer automatisch in die bestehende Konsole unseres Unternehmens zu migrieren. Klicken Sie in der E-Mail mit der Betreffzeile &quot;Für die Verwaltung des Benutzerzugriffs auf Adobe Marketo Engage erforderliche Aktion `[Package Tier]`&quot;auf die Schaltfläche &quot;Erste Schritte&quot;, um zur Einwilligungsseite zu navigieren.

`3.` **Optional:** Einrichten der einmaligen Anmeldung (SSO) auf der Adobe Admin Console.

* Damit unsere Benutzer sich künftig mit SSO bei ihrer Adobe Identity anmelden können, bitten wir Sie, bei der SSO-Einrichtung in Adobe Admin Console behilflich zu sein, bevor die Benutzermigration erfolgt.
Wir freuen uns über Ihre Mitarbeit bei dieser Umstellung. Teilen Sie mir mit, wenn Sie diese Schritte ausgeführt haben, damit ich mit der Benutzermigration mit Marketo Engage fortfahren kann.
Mit freundlichen Grüßen

`[Your Name]`

`---------------------------------------------------`

* Senden Sie eine E-Mail an Marketo Engage-Benutzer.

Unten finden Sie eine Beispiel-E-Mail, mit der Sie die bevorstehende Migration zu Ihren Marketo Engage-Benutzern ankündigen können, die nicht über Administratorberechtigungen verfügen.

`---------------------------------------------------`

**Betreff: Wichtige Aktualisierung—Migration von Marketo Engage-Abonnements zu Adobe Admin Console**

Sehr geehrte Marketo Engage-Benutzer,

Wir haben eine wichtige Mitteilung bezüglich unserer Marketo Engage-Instanz und wie Sie sich anmelden werden. Adobe verschiebt Marketo Engage-Abonnements und -Benutzer in die Adobe Admin Console, damit ihre Kunden ihre gesamte Produktverwaltung zentral verwalten können. Dies hat keine Auswirkungen auf Marketing-Workflows, Inhalte, Integrationen oder Assets.

Schlüsseldetails:

* Migrationsdatum: [Geben Sie das geplante Datum an - finden Sie dieses unter Marketo Engage unter **Admin** > **Migrationskonsole** > **Vormigration**]

* Zeit: Die Migration beginnt gegen Mitternacht Ortszeit für unser Abonnement.

* Auswirkung: Bei der Benutzermigration gehen keine Produktzugriffsverluste ein. Wenn Sie beim Migrieren Ihres Kontos angemeldet sind, werden Sie nach der Migration mit Adobe Identity abgemeldet und aufgefordert, sich innerhalb von Minuten wieder anzumelden.

* Vorteile: Authentifizieren Sie Marketo Engage- und andere Adobe-Produkte mit einer einzigen Adobe-Identität, entweder mit einer Adobe ID- oder Adobe-Federated ID (SSO).

Was Sie tun müssen:

`1.` Vorbereiten: Es ist eine E-Mail-Verifizierung erforderlich, damit Sie zu einer Adobe-Identität migriert werden können.

i. Sie haben eine E-Mail mit einer E-Mail-Überprüfungsanforderung mit einem Link erhalten (gültig für 3 Tage). Wenn Ihr Link abgelaufen ist, können Sie die Verifizierungs-E-Mail erneut senden, indem Sie &quot;**Admin**&quot;> &quot;**Mein Konto**&quot;> &quot;**Kontoeinstellungen**&quot;aufrufen und auf &quot;**Überprüfung erneut durchführen**&quot;klicken.
ii. Eine aktive Benutzersitzung ist für den Erfolg der E-Mail-Verifizierung erforderlich. Bitte melden Sie sich zuerst bei Ihrem Marketo Engage-Abonnement mit Ihrer Identitätsanbieter-URL (IdP) an.

`2.` Onboard: Sobald Ihr Benutzerkonto migriert wurde, erhalten Sie eine E-Mail von Adobe bezüglich der Änderungen an Ihrer Anmeldemethode.

i. Akzeptieren Sie die neue Einladung, indem Sie auf die Schaltfläche &quot;Einladung annehmen&quot;klicken und sich mit Adobe Identity anmelden.
ii. Melden Sie sich auf der Adobe-Anmeldeseite mit einer bestehenden Adobe ID an.

`3.` Kontakt: Wenn Sie Fragen haben oder Hilfe benötigen, nachdem Ihr Konto migriert wurde oder wenn Ihr Konto nicht migriert wurde und Sie keinen Zugriff auf Marketo Engage haben, wenden Sie sich an das Marketo Engage-Migrationsteam unter `[your internal contact email/phone]`.

Wir freuen uns über Ihre Mitarbeit bei dieser Umstellung. Vielen Dank für Ihr Verständnis und Ihr Engagement, unsere Systeme sicher zu halten.

Mit freundlichen Grüßen

`[Your Name]`

`---------------------------------------------------`
