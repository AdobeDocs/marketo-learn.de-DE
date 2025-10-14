---
title: Migration zu Adobe Identity Management
description: Dieses Tutorial hilft Ihnen, bei der Migration Ihrer Marketo Engage-Abonnements und -Benutzenden zur Adobe Admin Console zu navigieren.
role: Admin
level: Intermediate, Experienced
recommendations: noDisplay, noCatalog
last-substantial-update: 2024-07-26T00:00:00Z
feature: Marketing
exl-id: 8368a148-c0c8-462f-b166-9efc412c4a0f
source-git-commit: dcfffa299cbcfef489f5b618fae29f745b878d26
workflow-type: tm+mt
source-wordcount: '1250'
ht-degree: 0%

---

# Migration zu Adobe Identity Management

Adobe verbessert die Verwaltung Ihrer Adobe Marketo Engage-Abonnements und -Benutzer. Wir steigern die Produktivität Ihres Unternehmens, indem wir Ihre Marketo Engage-Abonnements und -Benutzer zur Adobe Admin Console migrieren.

In diesem Tutorial erfahren Sie, wie Sie die Migration durchführen, um Adobe Marketo Engage zusammen mit anderen Adobe-Konten und -Produkten für Ihre Benutzerinnen und Benutzer an einem zentralen Ort zu verwalten. Die Migration ist erforderlich und hat keine Auswirkungen auf Ihren Marketing-Workflow, Ihre Inhalte, Integrationen oder Assets.

## Checkliste vor der Migration für Marketo Engage-Administratoren {#pre-migration-checklist-for-marketo-engage-administrators}

Um sicherzustellen, dass Ihr Unternehmen Adobe Marketo Engage zum Adobe Admin Console migrieren kann, empfehlen wir, die folgende Checkliste zu befolgen, um die bevorstehenden Änderungen zu verwalten.

### 1. Bestimmen Sie Ihren/Ihre Systemadministrator(en) und Ihr IT-Team und besprechen Sie die Maßnahmen, die diese möglicherweise ergreifen müssen {#identify-your-system-administrators}

* Wenn Sie sich nicht sicher sind, wer die Systemadministratoren in Ihrem Unternehmen sind, wenden Sie sich an Ihr Adobe-Accountteam oder wenden Sie sich an den Adobe-Support `marketocares@marketo.com`.

* Bestätigen Sie die Adobe Admin Console (oder Adobe-Organisation), zu der Ihre Marketo Engage-Abonnements migriert werden. Wahrscheinlich verfügen Sie über eine Adobe Admin Console für [Dynamic Chat](/help/dynamic-chat/dynamic-chat-overview.md){target="_blank"}, ein natives Tool zur Konversationsautomatisierung in Marketo Engage. Marketo Engage-Abonnements müssen in derselben Organisation bereitgestellt werden wie Dynamic Chat.

* Auf die Zulassungsliste setzen Arbeiten Sie mit Ihrem IT-Team zusammen, um alle aufgelisteten Adobe[Domains (oben in diesem Artikel) &#x200B;](https://experienceleague.adobe.com/de/docs/marketo/using/getting-started/initial-setup/configure-protocols-for-marketo){target="_blank"}, um eine Unterbrechung des Marketo Engage-Zugriffs nach der Migration zu Adobe Identity zu vermeiden.

* **Optional:** [Implementieren von Single Sign-On (SSO)](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console#subscription-migration-complete){target="_blank"} vor der Benutzermigration.

  >[!NOTE]
  >
  >Es gibt Unterschiede zwischen dem von Marketo Engage unterstützten SSO und dem Adobe Admin Console-SSO. Daher müssen möglicherweise Änderungen an Ihrer Konfiguration implementiert werden.

* **Optional:** Passen Sie die [gewünschte maximale Sitzungsdauer](https://helpx.adobe.com/de/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"} vor der Benutzermigration an, damit Marketo Engage-Benutzer authentifiziert bleiben.

* Informationen zur Kommunikation mit Ihren Systemadministratoren finden Sie im Abschnitt [Beispiel-E-Mail](#announce-the-migration-timeline).

### 2. Machen Sie sich mit den Änderungen und Auswirkungen der Migration zu Adobe Identity vertraut. {#familiarize-yourself-with-the-changes}

Im folgenden Video führt Sie das Produktverwaltungsteam von Marketo Engage durch die Migrations-Journey und erläutert, was zu erwarten ist.

>[!VIDEO](https://video.tv.adobe.com/v/3432362/?t=170/?quality=12&learn=on&captions=ger){transcript=true}

Weitere Informationen zu diesem Thema für Marketo Engage-Administratoren finden Sie in den folgenden Hilfeartikeln:

* [Checkliste für die Benutzereinrichtung](https://experienceleague.adobe.com/de/docs/marketo/using/getting-started/initial-setup/user-setup){target="_blank"}

* [Übersicht über Adobe Identity Management](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"}

* [Grundlegendes zu Marketo-Abonnements und Benutzermigration zur Adobe Admin Console](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console){target="_blank"}

* [Migration zu Adobe Identity mit Migrationskonsole](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity){target="_blank"}

* [Erfahren Sie, wie Sie Adobe Admin Console verwenden](https://helpx.adobe.com/de/enterprise/using/admin-console.html){target="_blank"}

### 3. Den Zeitplan und die erforderliche Vorbereitung für die Migration für Ihre internen Teams bekannt geben {#announce-the-migration-timeline}

* Markieren Sie das Migrationsdatum in den Kalendern Ihrer Marketo Engage-Administratoren und -Benutzer nach Zeitplan.

   * Sie können das Migrationsdatum unter **Admin** > **Migrationskonsole** > **Vormigration** an Ihren internen Zeitplan anpassen. Erfahren Sie mehr über die Neuplanung und die Einschränkungen [Ändern des Migrationsdatums](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity#pre-migration){target="_blank"}.

* **Senden Sie eine E-Mail an Ihre Systemadministratoren**

Nachfolgend finden Sie eine Beispiel-E-Mail, die Sie an Ihre Administratoren senden können. In der Regel verwaltet Ihre IT-Abteilung alle Adobe-Lizenzen.

+++ Beispiel-E-Mail, die an Ihre Systemadministratoren gesendet werden soll

**Betreff: Erforderlicher Support - Migration von Marketo Engage-Abonnements auf Adobe Admin Console**

Sehr geehrte `[IT Administrator/NAME]`,

Unser Marketo Engage-Abonnement wird bald in das Adobe Identity Management-System migriert. Der `[Marketing Operation team]` benötigt Ihre Hilfe, um einige erforderliche Schritte vor Beginn der Benutzermigration auszuführen und so die Auswirkungen auf Marketo Engage-Benutzende zu minimieren.

`1.` Bestätigen Sie, ob das Unternehmen bereits andere Adobe-Produkte in Adobe Admin Console(s) verwaltet und ob Marketo Engage in dieselbe Konsole migriert wird.

* Marketo Engage-Abonnements müssen sich in derselben Organisation befinden wie Dynamic Chat, ein natives Tool zur Konversationsautomatisierung, das in Marketo Engage integriert ist.

* Wenn Sie Fragen oder Bedenken bezüglich der Admin Console haben, wenden Sie sich bitte an den Adobe-Support unter `marketocares@marketo.com` und CC us.

`2.` suchen Sie nach einer E-Mail von Adobe mit der Betreffzeile „Aktion erforderlich, um den Benutzerzugriff auf Adobe Marketo Engage `[Package Tier]` zu verwalten“. Diese E-Mail wurde versendet, nachdem Marketo Engage-Lizenzen auf unserer Admin Console bereitgestellt wurden. Diese E-Mail wird nur von Systemadministratoren empfangen. Bitte informieren Sie uns umgehend, wenn Sie es erhalten.

* Adobe kann von Ihnen, dem Systemadministrator der Admin Console, die Zustimmung einholen, Benutzer automatisch zur bestehenden Konsole Ihres Unternehmens zu migrieren. Klicken Sie in der E-Mail mit der Betreffzeile „Aktion erforderlich, um den Benutzerzugriff auf Adobe Marketo Engage `[Package Tier]` zu verwalten“ auf die Schaltfläche „Erste Schritte“, um zur Einverständnisseite zu navigieren.

`3.` Nach der Migration wird Marketo Engage nicht mehr von experience.adobe.com, sondern von Adobe Experience Cloud bereitgestellt. Zulassungsliste aller Adobe Domains [oben in diesem Artikel), &#x200B;](https://experienceleague.adobe.com/de/docs/marketo/using/getting-started/initial-setup/configure-protocols-for-marketo){target="_blank"} eine Unterbrechung unseres Marketo Engage-Zugriffs zu vermeiden.

`4.` **Optional:** Richten Sie SSO (Single Sign-On) in der Adobe Admin Console ein.

* Damit unsere Benutzer auch künftig von der SSO-Anmeldung mit ihrer Adobe-Identität profitieren können, sollten Sie sich vor der Benutzermigration bei der SSO-Einrichtung in der Adobe Admin Console unterstützen.

`5.` **Optional:** Legen Sie eine längere [maximale Sitzungsdauer) &#x200B;](https://helpx.adobe.com/de/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"} Adobe Admin Console fest.

* Um zu verhindern, dass sich Benutzer häufig anmelden müssen, passen Sie die Sitzungsdauer in den erweiterten Einstellungen für eine längere Dauer an.

Wir danken Ihnen für Ihre Mitarbeit während dieser Übergangsphase. Lassen Sie es mich wissen, wenn Sie diese Schritte abgeschlossen haben, damit ich mit der Migration fortfahren kann.

Mit freundlichen Grüßen

`[Your Name]`

+++

* **Senden einer E-Mail an Marketo Engage-Benutzer**

Nachfolgend finden Sie eine Beispiel-E-Mail für Marketo Engage-Benutzende **die** Administratorrechte haben.

+++ Beispiel-E-Mail zur Ankündigung der bevorstehenden Migration

**Betreff: Wichtiges Update - Migration von Marketo Engage-Abonnements auf Adobe Admin Console**

Sehr geehrte Marketo Engage-Benutzer,

Wir haben eine wichtige Ankündigung bezüglich unserer Marketo Engage-Instanz und wie Sie sich anmelden werden. Adobe verschiebt Marketo Engage-Abonnements und -Benutzer in die Adobe Admin Console, damit wir ihre gesamte Produktverwaltung an einem Ort zentralisieren können. Dies hat keine Auswirkungen auf Marketing-Workflows, Inhalte, Integrationen oder Assets.

**Wichtige Details:**

* **Migrationsdatum**: `[Specify the scheduled date - please find this in Marketo Engage under Admin > Migration Console > Pre-migration]`

* **Zeit**: Die Migration beginnt um Mitternacht (Ortszeit) für unser Abonnement.

* **Auswirkung**: Bei der Benutzermigration tritt kein Verlust des Produktzugriffs auf. Wenn Sie während der Migration Ihres Kontos angemeldet sind, werden Sie abgemeldet und nach der Migration aufgefordert, sich innerhalb von Minuten mit Adobe Identity erneut anzumelden.

* **Vorteile**: Authentifizierung von Marketo Engage und anderen Adobe-Produkten mithilfe einer einzigen Adobe-Identität - entweder Adobe ID oder Adobe Federated ID (SSO).

**Was Sie tun müssen:**

`1.` **Vorbereiten**: Für die Migration zu einer Adobe-Identität ist eine E-Mail-Bestätigung erforderlich.

i. Sie haben eine E-Mail mit einer Bestätigungsanfrage per E-Mail mit einem Link erhalten (bleibt 3 Tage gültig). Wenn Ihr Link abgelaufen ist, können Sie die Verifizierungs-E-Mail aus Marketo Engage erneut senden, indem Sie auf das Symbol „Mein Profil“ klicken und dann zu **Mein Konto** > **Kontoeinstellungen** > **Verifizierung erneut senden** navigieren.

II. Für eine erfolgreiche E-Mail-Überprüfung ist eine aktive Benutzersitzung erforderlich. Bitte melden Sie sich zuerst mit Ihrer Identitätsanbieter-URL (IdP) bei Ihrem Marketo Engage-Abonnement an.

`2.` **Onboard**: Nachdem Ihr Benutzerkonto migriert wurde, erhalten Sie eine E-Mail von Adobe über die Änderungen an Ihrer Anmeldemethode.

i. Akzeptieren Sie die neue Einladung, indem Sie auf die Schaltfläche „Einladung annehmen“ klicken und sich mit Adobe Identity anmelden.

II. Melden Sie sich auf der Adobe-Anmeldeseite mit einer bestehenden Adobe ID an.

III. Sie müssen sich zuerst bei der Marketo Engage-Instanz anmelden, um eine zuvor mit Lesezeichen versehene URL auf der Domain engage-xx.marketo.com zu erhalten, zu der Sie navigieren.

`3.` **Kontakt**: Wenn Sie Fragen haben oder Hilfe benötigen, nachdem Ihr Konto migriert wurde, oder wenn Ihr Konto nicht migriert wurde und Sie den Zugriff auf Marketo Engage verloren haben, wenden Sie sich unter `[your internal contact email/phone]` an das Marketo Engage-Migrationsteam.

Wir danken Ihnen für Ihre Mitarbeit während dieser Übergangsphase. Vielen Dank für Ihr Verständnis und Ihr Engagement für die Sicherheit unserer Systeme.

Mit freundlichen Grüßen

`[Your Name]`

+++
