---
title: CRM-Synchronisierungsfehler protokollieren für einfache Fehlerbehebung
description: Erfahren Sie, wie Sie ein Protokoll mit CRM-Synchronisierungsfehlern verwenden, um CRM-Synchronisierungsprobleme zu untersuchen und für einen reibungslosen Betrieb zu sorgen.
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00Z
jira: KT-13875
thumbnail: KT-13875.jpeg
hide: false
exl-id: 3b7e6127-28fd-4dce-915d-5af9bcce984b
source-git-commit: 681d390ce5ab336a7e24cc63256659a492288517
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# CRM-Synchronisierungsfehler protokollieren für einfache Fehlerbehebung

Als Marketo Engage-Administrator sollte die Überprüfung, ob Ihre Instanz mit Ihrem CRM synchronisiert ist, ein wichtiger Teil Ihrer [täglichen Routine](https://nation.marketo.com/t5/champion-program-blogs/my-marketo-morning-routine-tips-for-driving-marketing-operation/ba-p/247508){target="_blank"} sein. Im [Benachrichtigungsabschnitt](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/notification-types.html){target="_blank"} (finden Sie ihn oben rechts in Ihrer Marketo Engage-Benutzeroberfläche) finden Sie Informationen zu häufigen Synchronisierungsproblemen. Es gibt jedoch einen Profi-Tipp, der Ihnen dabei helfen kann, den Zustand der Instanz auf übersichtliche Weise zu verwalten. Adobe Marketo Champion (2019-2022), Amy Goldfine empfiehlt Admin-Benutzern, ein Protokoll der CRM-Synchronisierungsfehler zu führen, um die Fehlerbehebung zu erleichtern.

![Screenshot der Registerkarte „Synchronisierungsfehler“](/help/tutorial-inherited-instance/_assets/Marketo_Engage_Admin_Salesforce_Sync_Errors_Tab.png)

## Warum sollten CRM-Synchronisierungsfehler aufgezeichnet werden?

Durch Protokollierung der CRM-Synchronisierungsfehler können Marketo Engage-Administratoren die Probleme und Trends mit den CRM-Administratoren überprüfen, um die Grundursache zu beheben. Gehen Sie wie folgt vor, um die CRM-Synchronisierungsprobleme für Ihre Instanz zu dokumentieren.

## Wie man ein Protokoll der CRM-Synchronisierungsfehler führt

Laden Sie zunächst die Vorlage [CRM-Synchronisierungsfehler-Protokoll](/help/tutorial-inherited-instance/_assets/downloads/Adobe-Marketo-Engage_CRM-Sync-Error-Log-Template.xlsx) herunter.

**Schritt 1:** Gehen Sie zum *[!UICONTROL Admin] Abschnitt* Marketo Engage. Klicken *[!UICONTROL unter]* Integration *[!DNL Salesforce]* auf, *[!DNL Microsoft Dynamics]* oder *[!DNL Veeva]*, je nachdem, welche [!DNL CRM] Sie verwenden, und klicken Sie dann auf die Registerkarte *[!UICONTROL Synchronisierungsfehler]*.

**Schritt 2:** Sie können [die Fehlerdatensätze als  [!DNL CSV]  über das Bedienfeld [!UICONTROL Filtern] exportieren](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.html#filter-sync-errors){target="_blank"}. Wenn Sie nur wenige Stunden haben, sollten Sie direkt von der Registerkarte *[!UICONTROL Synchronisierungsfehler]* kopieren und einfügen.

**Schritt 3:** Notieren Sie das Datum, an dem der Fehler aufgetreten ist.

**Schritt 4:** Geben Sie die Anzahl der von diesem Fehler betroffenen Personendatensätze ein. (Manchmal gibt Ihr CRM-System nur einen Fehler für eine Person aus. Manchmal gibt es viele Personen mit demselben Fehler auf einmal.)

**Schritt 5:** Notieren Sie die E-Mail-Adresse einer von dem Fehler betroffenen Person. Dies erleichtert Ihnen die Referenz und Diskussion der Fehler mit dem CRM-Administrator.

**Schritt 6:** Fügen Sie Links zum Personendatensatz in den [!DNL Marketo Engage]- und [!UICONTROL CRM-Lead/Kontakt]-Datensatz dieser Person ein.

**Schritt 7:** Fügen Sie den tatsächlichen Text des Fehlers in die letzte Spalte ein.

## Wie geht es weiter?

**Identifizieren von Fehler-Codes:** Um die Fehler-Codes zu verstehen, suchen Sie die Beschreibungen in der Entwicklerdokumentation [Tabelle „Fehler-Codes auf ](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes){target="_blank"}&quot; und finden Sie die typischen nächsten Schritte zur Behebung der Fehler.

## Autoren

**Amy Goldfine**\
Adobe Marketo Champion(2019-2022)
*Gründer, MarketingOpsAdvice.com*

![Amy Goldfine](/help/tutorial-inherited-instance/_assets/authors/Customer_Author_Amy_Goldfine.png){width="25%"}

**Amy Chiu**
*Adoption &amp; Retention Marketing Manager bei Adobe*

![Amy Chiu](/help/tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width="25%"}
