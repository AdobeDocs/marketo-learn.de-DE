---
title: Fehler bei der CRM-Synchronisierung zur einfachen Fehlerbehebung
description: Erfahren Sie, wie Sie mithilfe eines Protokolls mit Fehlern bei der CRM-Synchronisierung Probleme bei der CRM-Synchronisierung untersuchen und diese reibungslos ausführen können.
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

# Fehler bei der CRM-Synchronisierung zur einfachen Fehlerbehebung

Als Marketo Engage-Administrator sollte die Überprüfung, ob Ihre Instanz mit Ihrem CRM-System synchronisiert ist, ein zentraler Bestandteil Ihrer [täglichen Routine](https://nation.marketo.com/t5/champion-program-blogs/my-marketo-morning-routine-tips-for-driving-marketing-operation/ba-p/247508){target="_blank"} sein. Im Abschnitt [Benachrichtigungen](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/notification-types.html){target="_blank"} (finden Sie ihn oben rechts auf der Marketo Engage-Oberfläche) finden und untersuchen Sie zwar häufige Synchronisierungsprobleme, es gibt jedoch einen prop-Tipp, der Ihnen bei der Organisation des Instanzstatus helfen könnte. Adobe Marketo Champion (2019-2022), Amy Goldfine empfiehlt Admin-Benutzern, ein Protokoll mit CRM-Synchronisierungsfehlern zu führen, um die Fehlerbehebung zu vereinfachen.

![Screenshot der Registerkarte &quot;Synchronisierungsfehler&quot;](/help/tutorial-inherited-instance/_assets/Marketo_Engage_Admin_Salesforce_Sync_Errors_Tab.png)

## Warum sollten Sie CRM-Synchronisierungsfehler aufzeichnen?

Durch Protokollierung der CRM-Synchronisierungsfehler können Marketo Engage-Administratoren die Probleme und Trends mit den CRM-Administratoren überprüfen, um die Grundursache zu beheben. Führen Sie die folgenden Schritte aus, um Probleme mit der CRM-Synchronisierung für Ihre Instanz zu dokumentieren.

## Protokollierung von CRM-Synchronisierungsfehlern

Laden Sie vor dem Start die Vorlage [CRM-Fehlerprotokoll-Vorlage](/help/tutorial-inherited-instance/_assets/downloads/Adobe-Marketo-Engage_CRM-Sync-Error-Log-Template.xlsx) herunter.

**Schritt 1:** Wechseln Sie zum Abschnitt *[!UICONTROL Admin]* im Marketo Engage. Klicken Sie unter *[!UICONTROL Integration]* auf *[!DNL Salesforce]*, *[!DNL Microsoft Dynamics]* oder *[!DNL Veeva]*, je nachdem, welchen [!DNL CRM] Sie verwenden, und dann auf die Registerkarte *[!UICONTROL Fehler synchronisieren]*.

**Schritt 2:** Sie können festlegen, dass die Fehlerdatensätze als  [!DNL CSV] -Datei über das Bedienfeld [!UICONTROL Filter]](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.html#filter-sync-errors){target="_blank"} exportiert werden. [ Wenn Sie nur wenige Stunden Zeit haben, können Sie direkt von der Registerkarte *[!UICONTROL Fehler synchronisieren]* kopieren und einfügen.

**Schritt 3:** Notieren Sie das Datum, an dem der Fehler aufgetreten ist.

**Schritt 4:** Geben Sie die Anzahl der von diesem Fehler betroffenen Datensätze ein. (Manchmal gibt Ihr CRM-System nur einen Fehler für eine Person aus. Manchmal wird es viele Personen mit demselben Fehler gleichzeitig geben.)

**Schritt 5:** Notieren Sie die E-Mail-Adresse einer vom Fehler betroffenen Person. Dadurch können Sie die Fehler einfach beim CRM-Administrator referenzieren und besprechen.

**Schritt 6:** Fügen Sie Links zum Personendatensatz in den Datensatz [!DNL Marketo Engage] und in den Datensatz [!UICONTROL CRM-Lead/Kontakt] dieser Person ein.

**Schritt 7:** Fügen Sie in der letzten Spalte den tatsächlichen Text des Fehlers ein.

## Wie geht es weiter?

**Fehlercodes identifizieren:** Um die Fehlercodes zu verstehen, suchen Sie die Beschreibungen in der Entwicklerdokumentation [Tabelle mit Fehlercodes auf Antwortebene](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes){target="_blank"} und suchen Sie nach typischen nächsten Schritten zur Behebung der Fehler.

## Autoren

**Amy Goldfine**\
Adobe Marketo Champion (2019-2022)
*Gründer, MarketingOpsAdvice.com*

![Amy Goldfine](/help/tutorial-inherited-instance/_assets/authors/Customer_Author_Amy_Goldfine.png){width="25%"}

**Amy Chiu**
*Adoption &amp; Retention Marketing Manager bei Adobe*

![Amy Chiu](/help/tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width="25%"}
