---
title: Migrieren zu Adobe Identity Management
description: Dieses Tutorial hilft Ihnen bei der Migration Ihrer Marketo Engage-Abonnements und -Benutzenden zur Adobe Admin Console.
role: Admin
level: Intermediate, Experienced
recommendations: noDisplay, noCatalog
last-substantial-update: 2024-07-26T00:00:00Z
feature: Marketing
exl-id: 8368a148-c0c8-462f-b166-9efc412c4a0f
source-git-commit: 096d4b42008446a72f92b8fe509c0c216bc8f904
workflow-type: tm+mt
source-wordcount: '1428'
ht-degree: 93%

---

# Migrieren zu Adobe Identity Management

Adobe erleichtert die Verwaltung Ihrer Adobe Marketo Engage-Abonnements und -Benutzenden. Wir steigern die Produktivität Ihres Unternehmens, indem wir Ihre Marketo Engage-Abonnements und -Benutzenden zur Adobe Admin Console migrieren.

In diesem Tutorial erfahren Sie, wie Sie die Migration durchführen, um Adobe Marketo Engage zusammen mit anderen Adobe-Konten und -Produkten für Ihre Benutzenden an einem zentralen Ort zu verwalten. Die Migration ist erforderlich und hat keine Auswirkungen auf Ihren Marketing-Workflow bzw. auf Inhalte, Integrationen oder Assets.

## Checkliste vor der Migration für Marketo Engage-Admins {#pre-migration-checklist-for-marketo-engage-administrators}

Um sicherzustellen, dass Ihr Unternehmen Adobe Marketo Engage in die Adobe Admin Console migrieren kann, empfehlen wir, die folgende Checkliste zu konsultieren. So können Sie die anstehenden Änderungen leichter verwalten.

### &#x200B;1. Bestimmen Sie Ihre(n) Systemadministrator(in) und Ihr IT-Team und besprechen Sie die erforderlichen Maßnahmen {#identify-your-system-administrators}

* Wenn Sie nicht genau wissen, wer die Systemadmins in Ihrem Unternehmen sind, wenden Sie sich an Ihr Adobe-Accountteam oder an den Adobe-Support `marketocares@marketo.com`.

* Prüfen Sie die Adobe Admin Console (oder Adobe-Org), zu der Ihre Marketo Engage-Abonnements migriert werden sollen. Wahrscheinlich haben Sie eine Adobe Admin Console für [Dynamic Chat](/help/main/dynamic-chat/dynamic-chat-overview.md){target="_blank"}, ein natives Tool zur Automatisierung von Konversationen in Marketo Engage. Marketo Engage-Abonnements müssen in derselben Organisation bereitgestellt werden wie Dynamic Chat.

* Arbeiten Sie mit Ihrem IT-Team zusammen, um alle Adobe-Domains, die [oben in diesem Artikel](https://experienceleague.adobe.com/de/docs/marketo/using/getting-started/initial-setup/configure-protocols-for-marketo){target="_blank"} aufgeführt werden, auf die Zulassungsliste zu setzen. So können Sie eine Unterbrechung des Marketo Engage-Zugriffs nach der Migration zu Adobe Identity verhindern.

* **Optional:** [Implementieren Sie Single Sign-On (SSO)](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console#subscription-migration-complete){target="_blank"} vor der Benutzermigration.

  >[!NOTE]
  >
  >Es gibt Unterschiede zwischen SSO, das von Marketo Engage bzw. der Adobe Admin Console unterstützt wird. Daher müssen Sie ggf. Änderungen an Ihrer Konfiguration implementieren.

* **Optional:** Passen Sie vor der Benutzermigration die [gewünschte maximale Sitzungsdauer](https://helpx.adobe.com/de/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"} an, damit Marketo Engage-Benutzende authentifiziert bleiben.

* Informationen zur Kommunikation mit Ihren Systemadmins finden Sie im Abschnitt [Beispiel-E-Mail](#announce-the-migration-timeline).

### &#x200B;2. Machen Sie sich mit den Änderungen und Auswirkungen der Migration zu Adobe Identity vertraut. {#familiarize-yourself-with-the-changes}

Im folgenden Video führt Sie das Produkt-Management-Team von Marketo Engage durch die Migrations und erläutert, was zu erwarten ist.

>[!VIDEO](https://video.tv.adobe.com/v/3430920t3/?t=170/?quality=12&learn=on){transcript=true}

Weitere Informationen zu diesem Thema für Marketo Engage-Admins finden Sie in den folgenden Hilfeartikeln:

* [Checkliste für die Benutzereinrichtung](https://experienceleague.adobe.com/de/docs/marketo/using/getting-started/initial-setup/user-setup){target="_blank"}

* [Überblick über Adobe Identity Management](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"}

* [Grundlegendes zur Marketo-Abonnement- und -Benutzermigration zur Adobe Admin Console](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console){target="_blank"}

* [Migrieren zu Adobe Identity mit der Migrationskonsole](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity){target="_blank"}

* [Verwendung von Adobe Admin Console](https://helpx.adobe.com/de/enterprise/using/admin-console.html){target="_blank"}

### &#x200B;3. Geben Sie den Zeitplan und die Vorbereitung der Migration an, die für Ihre internen Teams erforderlich sind {#announce-the-migration-timeline}

* Tragen Sie das Migrationsdatum in die Kalender Ihrer Marketo Engage-Admins und -Benutzenden ein, sobald der Zeitplan steht.

   * Sie können das Migrationsdatum unter **Admin** > **Migrationskonsole** > **Vormigration** an Ihren internen Zeitplan anpassen. Erfahren Sie mehr über die Neuplanung und Einschränkungen beim [Ändern des Migrationsdatums](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity#pre-migration){target="_blank"}.

* **Senden einer E-Mail an Ihre Systemadmins**

Nachfolgend finden Sie eine Beispiel-E-Mail, die Sie an Ihre Admins senden können. In der Regel verwaltet Ihre IT-Abteilung alle Adobe-Lizenzen.

+++ Beispiel-E-Mail, die Sie an Ihre Systemadmins senden können

**Betreff: Support erforderlich – Migration von Marketo Engage-Abonnements zur Adobe Admin Console**

Guten Tag `[IT Administrator/NAME]`,

unser Marketo Engage-Abonnement wird bald in das Identitäts-Management-System von Adobe migriert. Das `[Marketing Operation team]` benötigt Ihre Hilfe, damit es vor Beginn der Benutzermigration erforderliche Schritte ausführen und so die Auswirkungen auf Marketo Engage-Benutzende minimieren kann.

`1.` Prüfen Sie, ob die Organisation bereits andere Adobe-Produkte in Adobe Admin Console(s) verwaltet und ob Marketo Engage in dieselbe Konsole migriert werden soll.

* Marketo Engage-Abonnements müssen sich in derselben Organisation befinden wie Dynamic Chat (ein natives Tool zur Automatisierung von Konversationen, das mit Marketo Engage integriert ist).

* Wenn Sie Fragen oder Bedenken bezüglich der Admin Console haben, wenden Sie sich an den Adobe-Support unter `marketocares@marketo.com` und setzen Sie uns auf CC.

`2.` Achten Sie auf eine E-Mail von Adobe mit dem Betreff „Aktion zur Verwaltung des Benutzerzugriffs auf Adobe Marketo Engage erforderlich`[Package Tier]`“. Diese E-Mail wurde versendet, nachdem Marketo Engage-Lizenzen in unserer Admin Console bereitgestellt wurden. Diese E-Mail erhalten nur Systemadmins. Bitte informieren Sie uns umgehend, wenn Sie die E-Mail erhalten.

* Adobe kann von Ihnen – der bzw. dem Systemadmin der Admin Console – das Einverständnis einholen, Benutzende automatisch zur bestehenden Konsole der Organisation zu migrieren. Klicken Sie in der E-Mail mit dem Betreff „Aktion zur Verwaltung des Benutzerzugriffs auf Adobe Marketo Engage erforderlich`[Package Tier]`“ auf die Schaltfläche „Jetzt loslegen“, um zur Einverständnisseite zu navigieren.

`3.` Nach der Migration wird Marketo Engage nicht mehr von experience.adobe.com, sondern von Adobe Experience Cloud bereitgestellt. Setzen Sie alle Adobe-Domains, die [oben in diesem Artikel](https://experienceleague.adobe.com/de/docs/marketo/using/getting-started/initial-setup/configure-protocols-for-marketo){target="_blank"} aufgeführt werden, auf die Zulassungsliste, um eine Unterbrechung des Marketo Engage-Zugriffs zu verhindern.

`4.` **Optional:** Richten Sie in der Adobe Admin Console SSO (Single Sign-on) ein.

* Damit sich unsere Benutzenden auch künftig per SSO bei ihrer Adobe-Identität anmelden können, sollten Sie vor der Benutzermigration die SSO-Einrichtung in der Adobe Admin Console unterstützen.

`5.` **Optional:** Legen Sie eine längere [maximale Sitzungsdauer](https://helpx.adobe.com/de/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"} in der Adobe Admin Console fest.

* Um zu verhindern, dass sich Benutzende wiederholt anmelden müssen, verlängern Sie in den erweiterten Einstellungen die Sitzungsdauer.

Wir danken Ihnen für Ihre Mitarbeit während des Übergangs. Geben Sie mir Bescheid, sobald Sie diese Schritte abgeschlossen haben, damit ich mit der Migration fortfahren kann.

Mit freundlichen Grüßen

`[Your Name]`

+++

* **Senden einer E-Mail an Marketo Engage-Benutzende**

Nachfolgend finden Sie eine Beispiel-E-Mail für Marketo Engage-Benutzende, die **keine** Administratorrechte haben.

+++ Beispiel-E-Mail zur Ankündigung der bevorstehenden Migration

**Betreff: Wichtiges Update – Migration von Marketo Engage-Abonnements in die Adobe Admin Console**

Sehr geehrte Benutzende von Marketo Engage,

wir haben eine wichtige Ankündigung bezüglich unserer Marketo Engage-Instanz sowie zur Anmeldung. Adobe verschiebt Marketo Engage-Abonnements und -Benutzende in die Adobe Admin Console, damit die gesamte Produktverwaltung an einem zentralen Ort erfolgen kann. Dies hat keine Auswirkungen auf Marketing-Workflows, Inhalte, Integrationen oder Assets.

**Wichtige Details:**

* **Migrationsdatum**: `[Specify the scheduled date - please find this in Marketo Engage under Admin > Migration Console > Pre-migration]`

* **Zeit**: Die Migration beginnt um etwa Mitternacht in der für unser Abonnement gültigen Zeitzone.

* **Auswirkung**: Bei der Migration der Benutzenden bleibt der Produktzugriff bestehen. Wenn Sie während der Migration Ihres Kontos angemeldet sind, werden Sie abgemeldet und wenige Minuten nach der Migration aufgefordert, sich mit Adobe Identity erneut anzumelden.

* **Vorteile**: Authentifizierung von Marketo Engage und anderen Adobe-Produkten mithilfe einer einzigen Adobe-Identität – entweder mit Adobe ID oder Adobe Federated ID (SSO).

**Was Sie tun müssen:**

`1.` **Vorbereiten**: Für die Migration zu einer Adobe-Identität ist eine E-Mail-Bestätigung erforderlich.

I. Sie haben eine E-Mail mit einer Bestätigungsanfrage per E-Mail mit einem Link erhalten (bleibt 3 Tage gültig). Wenn Ihr Link abgelaufen ist, können Sie die Bestätigungs-E-Mail in Marketo Engage erneut senden, indem Sie auf das Symbol „Mein Profil“ klicken und dann zu **Mein Konto** > **Kontoeinstellungen** > **Bestätigung erneut senden** navigieren.

ii. Für eine erfolgreiche E-Mail-Bestätigung ist eine aktive Benutzersitzung erforderlich. Melden Sie sich zunächst mit der URL Ihres Identitätsanbieters (IdP) bei Ihrem Marketo Engage-Abonnement an.

`2.` **Onboarding**: Nachdem Ihr Benutzerkonto migriert wurde, erhalten Sie eine E-Mail von Adobe hinsichtlich der Änderungen bei Ihrer Anmeldemethode.

I. Akzeptieren Sie die neue Einladung, indem Sie auf die Schaltfläche „Einladung annehmen“ klicken und sich mit Adobe Identity anmelden.

ii. Melden Sie sich auf der Adobe-Anmeldeseite mit einer vorhandenen Adobe ID an.

iii. Sie müssen sich zunächst bei der Marketo Engage-Instanz anmelden, um zu einer zuvor mit Lesezeichen versehenen URL in der Domain engage-xx.marketo.com, zu der Sie navigieren wollen, zu gelangen.

`3.` **Kontakt**: Falls Sie Fragen haben oder Hilfe benötigen, nachdem Ihr Konto migriert wurde, oder falls Ihr Konto nicht migriert wurde und Sie den Zugriff auf Marketo Engage verloren haben, wenden Sie sich unter `[your internal contact email/phone]` an das Migrations-Team für Marketo Engage.

Wir danken Ihnen für Ihre Mitarbeit während des Übergangs. Vielen Dank für Ihr Verständnis und Ihr Engagement bezüglich der Sicherheit unserer Systeme.

Mit freundlichen Grüßen

`[Your Name]`

+++
