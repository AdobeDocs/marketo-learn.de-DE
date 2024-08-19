---
title: Migration zu Adobe Identity Management
description: In diesem Tutorial erfahren Sie, wie Sie durch die Migration Ihrer Marketo Engage-Abonnements und -Benutzer zur Adobe Admin Console navigieren.
role: User
level: Beginner
recommendations: noDisplay, noCatalog
last-substantial-update: 2024-07-26T00:00:00Z
feature: Marketing
exl-id: 8368a148-c0c8-462f-b166-9efc412c4a0f
source-git-commit: 4ecbe3a79ad28a38e3c630868663a7b2859428e9
workflow-type: tm+mt
source-wordcount: '1170'
ht-degree: 0%

---

# Migration zu Adobe Identity Management

Adobe verbessert die Verwaltung Ihrer Adobe Marketo Engage-Abonnements und -Benutzer. Wir steigern die Produktivität Ihres Unternehmens, indem wir Ihre Marketo Engage-Abonnements und -Benutzer in die Adobe Admin Console migrieren.

In diesem Tutorial erfahren Sie, wie Sie durch die Migration navigieren, sodass Sie Adobe Marketo Engage gemeinsam mit anderen Adobe-Konten und -Produkten für Ihre Benutzer an einem zentralen Ort verwalten können. Die Migration ist erforderlich und hat keine Auswirkungen auf Ihren Marketing-Workflow, Ihre Inhalte, Integrationen oder Assets.

## Checkliste für die Vormigration für Marketo Engage-Administratoren {#pre-migration-checklist-for-marketo-engage-administrators}

Um sicherzustellen, dass Ihr Unternehmen Adobe Marketo Engage in die Adobe Admin Console migrieren kann, empfehlen wir, die nachfolgenden Änderungen anhand der Checkliste zu verwalten.

### 1. Identifizieren Sie Ihre Systemadministratoren und Ihr IT-Team und besprechen Sie die erforderlichen Maßnahmen. {#identify-your-system-administrators}

* Wenn Sie sich nicht sicher sind, welche Systemadministratoren sich in Ihrem Unternehmen befinden, wenden Sie sich an Ihr Adobe Account-Team oder wenden Sie sich an den Adobe-Support `marketocares@marketo.com`.

* Bestätigen Sie die Adobe Admin Console (oder Adobe-Org), zu der Ihre Marketo Engage-Abonnements migriert werden sollen. Wahrscheinlich verfügen Sie über eine Adobe Admin Console für [Dynamic Chat](/help/dynamic-chat/dynamic-chat-overview.md){target="_blank"}, ein natives Tool zur Automatisierung von Konversationen im Marketo Engage. Marketo Engage-Abonnements müssen im selben Unternehmen wie Dynamic Chat bereitgestellt werden.

* Arbeiten Sie mit Ihrem IT-Team zusammen, um alle Adobe-Domänen, die oben in diesem Artikel ](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/configure-protocols-for-marketo){target="_blank"} aufgelistet sind, in Zulassungsliste, um eine Unterbrechung des Marketo Engage-Zugriffs nach der Migration zu Adobe Identity zu verhindern.[

* **Optional:** [Implementieren Sie Single Sign On (SSO)](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console#subscription-migration-complete){target="_blank"} vor der Benutzermigration.

* Informationen zur Kommunikation mit Ihren Systemadministratoren finden Sie im Abschnitt [Beispiel-E-Mail](#announce-the-migration-timeline).

### 2. Machen Sie sich mit den Änderungen und Auswirkungen der Migration zur Adobe Identity vertraut. {#familiarize-yourself-with-the-changes}

Im folgenden Video führt Sie das Marketo Engage Product Management-Team durch die Migration und durch die Journey.

>[!VIDEO](https://video.tv.adobe.com/v/3430920t3/?t=170/?quality=12&learn=on){transcript=true}

Weitere Informationen zu diesem Thema für Marketo Engage-Administratoren finden Sie in den folgenden Hilfeartikeln:

* [Checkliste für die Benutzereinrichtung](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/user-setup){target="_blank"}

* [Adobe Identity Management-Übersicht ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"}

* [Grundlegendes zur Marketo-Anmeldung und Benutzermigration zur Adobe Admin Console](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console){target="_blank"}

* [Migration zur Adobe Identity mit der Migrationskonsole](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity){target="_blank"}

* [Grundlegendes zur Verwendung von Adobe Admin Console](https://helpx.adobe.com/de/enterprise/using/admin-console.html){target="_blank"}

### 3. Ankündigung des Zeitplans und der Vorbereitung der Migration für Ihre internen Teams {#announce-the-migration-timeline}

* Markieren Sie das Migrationsdatum einmal in den Kalendern Ihrer Marketo Engage-Administratoren und -Benutzer.

   * Sie können das Migrationsdatum in **Admin** > **Migrationskonsole** > **Vormigration** ändern, um es Ihrer internen Zeitleiste besser anzupassen. Erfahren Sie mehr über die Neuplanung und die Einschränkungen von [Ändern des Migrationsdatums](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity#pre-migration){target="_blank"}.

* **Senden einer E-Mail an Ihre Systemadministratoren**

Nachfolgend finden Sie eine Beispiel-E-Mail, die Sie an Ihre Systemadministratoren senden können. In der Regel verwaltet Ihre IT-Abteilung alle Adobe-Lizenzen.

`---------------------------------------------------`

**Betreff: Unterstützt erforderlich - Migration von Marketo Engage-Abonnements zu Adobe Admin Console**

Sehr geehrte `[IT Administrator/NAME]`,

Unser Marketo Engage-Abonnement wird bald in das Adobe Identity Management System migriert. Der `[Marketing Operation team]` benötigt Ihre Hilfe, um einige erforderliche Schritte vor Beginn der Benutzermigration abzuschließen, um die Auswirkungen auf Marketo Engage-Benutzer zu minimieren.

`1.` Bestätigen Sie, ob das Unternehmen bereits andere Adobe-Produkte in Adobe Admin Console(s) verwaltet und ob Marketo Engage in dieselbe Konsole migriert wird.

* Marketo Engage-Abonnements müssen im selben Unternehmen wie Dynamic Chat, ein natives, mit Marketo Engage integriertes Konvertierungs-Automatisierungstool, geführt werden.

* Wenn Sie Fragen oder Bedenken bezüglich der Admin Console haben, wenden Sie sich bitte an den Adobe-Support unter `marketocares@marketo.com` und CC uns.

`2.` Suchen Sie auf der Suche nach einer E-Mail von Adobe mit der Betreffzeile &quot;Aktion erforderlich für die Verwaltung des Benutzerzugriffs auf Adobe Marketo Engage `[Package Tier]`&quot;. Diese E-Mail wurde gesendet, nachdem auf unserer Admin Console Marketo Engage-Lizenzen bereitgestellt wurden. Diese E-Mail erhalten nur Systemadministratoren. Bitte informieren Sie uns umgehend, wann Sie es erhalten.

* Adobe kann die Zustimmung von Ihnen, dem Systemadministrator der Admin Console, einholen, um Benutzer automatisch in die bestehende Konsole unseres Unternehmens zu migrieren. Klicken Sie in der E-Mail mit der Betreffzeile &quot;Für die Verwaltung des Benutzerzugriffs auf Adobe Marketo Engage erforderliche Aktion `[Package Tier]`&quot;auf die Schaltfläche &quot;Erste Schritte&quot;, um zur Einwilligungsseite zu navigieren.

`3.` Nach der Migration wird Marketo Engage von experience.adobe.com nach Adobe Experience Cloud bedient. Bitte Zulassungsliste alle Adobe-Domains, die oben in diesem Artikel ](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/configure-protocols-for-marketo){target="_blank"} aufgelistet sind, um Störungen unseres Marketo Engage-Zugriffs zu vermeiden.[

`4.` **Optional:** Einrichten der einmaligen Anmeldung (SSO) auf der Adobe Admin Console.

* Damit unsere Benutzer, die sich in Zukunft mit SSO bei ihrer Adobe Identity anmelden, SSO-Setup in der Adobe Admin Console unterstützen, bevor die Benutzermigration erfolgt.

Wir freuen uns über Ihre Mitarbeit bei dieser Umstellung. Teilen Sie mir mit, wenn Sie diese Schritte ausgeführt haben, damit ich mit der Migration fortfahren kann.

Mit freundlichen Grüßen

`[Your Name]`

`---------------------------------------------------`

* **E-Mail an Marketo Engage-Benutzer senden**

Nachfolgend finden Sie eine Beispiel-E-Mail, mit der Sie die bevorstehende Migration zu Ihren Marketo Engage-Benutzern ankündigen können, die nicht über Administratorberechtigungen verfügen.

`---------------------------------------------------`

**Betreff: Wichtige Aktualisierung—Migration von Marketo Engage-Abonnements zu Adobe Admin Console**

Sehr geehrte Marketo Engage-Benutzer,

Wir haben eine wichtige Mitteilung bezüglich unserer Marketo Engage-Instanz und wie Sie sich anmelden werden. Adobe verschiebt Marketo Engage-Abonnements und -Benutzer in die Adobe Admin Console, damit wir ihre gesamte Produktverwaltung an einem Ort zentralisieren können. Dies hat keine Auswirkungen auf Marketing-Workflows, Inhalte, Integrationen oder Assets.

**Schlüsseldetails:**

* **Migrationsdatum**: `[Specify the scheduled date - please find this in Marketo Engage under Admin > Migration Console > Pre-migration]`

* **Zeit**: Die Migration beginnt etwa um Mitternacht Ortszeit für unser Abonnement.

* **Impact**: Bei der Benutzermigration gehen keine Produktzugriffsverluste ein. Wenn Sie beim Migrieren Ihres Kontos angemeldet sind, werden Sie nach der Migration mit Adobe Identity abgemeldet und aufgefordert, sich innerhalb von Minuten wieder anzumelden.

* **Vorteile**: Authentifizieren Sie Marketo Engage- und andere Adobe-Produkte anhand einer einzigen Adobe-Identität - entweder einer Adobe ID- oder einer Adobe-Federated ID (SSO).

**Was Sie tun müssen:**

`1.` **Vorbereiten**: Es ist eine E-Mail-Überprüfung erforderlich, damit Sie zu einer Adobe-Identität migriert werden können.

i. Sie haben eine E-Mail mit einer E-Mail-Überprüfungsanforderung mit einem Link erhalten (gültig für 3 Tage). Wenn Ihr Link abgelaufen ist, können Sie die Verifizierungs-E-Mail von Marketo Engage aus erneut senden, indem Sie auf das Symbol &quot;Mein Profil&quot;klicken und dann zu **Mein Konto** > **Kontoeinstellungen** > **Überprüfung erneut senden** navigieren.

ii. Eine aktive Benutzersitzung ist für den Erfolg der E-Mail-Verifizierung erforderlich. Bitte melden Sie sich zuerst bei Ihrem Marketo Engage-Abonnement mit Ihrer Identitätsanbieter-URL (IdP) an.

`2.` **Onboard**: Sobald Ihr Benutzerkonto migriert wurde, erhalten Sie eine E-Mail von Adobe bezüglich der Änderungen an Ihrer Anmeldemethode.

i. Akzeptieren Sie die neue Einladung, indem Sie auf die Schaltfläche &quot;Einladung annehmen&quot;klicken und sich mit Adobe Identity anmelden.

ii. Melden Sie sich auf der Adobe-Anmeldeseite mit einer bestehenden Adobe ID an.

iii. Sie müssen sich zunächst bei der Marketo Engage-Instanz für jede zuvor mit Lesezeichen versehene URL in der Domäne engage-xx.marketo.com anmelden, zu der Sie navigieren.

`3.` **Kontakt**: Wenn Sie Fragen haben oder Hilfe benötigen, nachdem Ihr Konto migriert wurde, oder wenn Ihr Konto nicht migriert wurde und Sie den Zugriff auf Marketo Engage verloren haben, wenden Sie sich an das Marketo Engage-Migrationsteam unter `[your internal contact email/phone]`.

Wir freuen uns über Ihre Mitarbeit bei dieser Umstellung. Vielen Dank für Ihr Verständnis und Ihr Engagement, unsere Systeme sicher zu halten.

Mit freundlichen Grüßen

`[Your Name]`

`---------------------------------------------------`
