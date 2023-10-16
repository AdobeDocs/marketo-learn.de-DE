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
source-git-commit: 4dc6aeed353fdd8bac960603af22b060ae2d7f00
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---


# Fehler bei der CRM-Synchronisierung zur einfachen Fehlerbehebung

Als Marketo Engage-Administrator sollte die Überprüfung, ob Ihre Instanz mit Ihrem CRM-System synchronisiert ist, ein wichtiger Teil Ihrer [tägliche Routine](https://nation.marketo.com/t5/champion-program-blogs/my-marketo-morning-routine-tips-for-driving-marketing-operation/ba-p/247508){target="_blank"}. While the [Notifications section](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/notification-types.html){target="_blank"} (finden Sie es in der oberen rechten Ecke Ihrer Marketo Engage-Oberfläche), wo Sie häufige Synchronisierungsprobleme finden und untersuchen werden. Es gibt einen prop-Tipp, der Ihnen bei der Organisation des Instanzstatus helfen könnte.  Adobe Marketo Champion (2022), empfiehlt Amy Goldfine, dass Admin-Benutzer ein Protokoll mit CRM-Synchronisierungsfehlern aufbewahren, um die Fehlerbehebung zu vereinfachen.

![Screenshot der Registerkarte &quot;Synchronisierungsfehler&quot;](/help/tutorial-inherited-instance/_assets/Marketo_Engage_Admin_Salesforce_Sync_Errors_Tab.png)

## Warum sollten Sie CRM-Synchronisierungsfehler aufzeichnen?

Durch Protokollierung der CRM-Synchronisierungsfehler können Marketo Engage-Administratoren die Probleme und Trends mit den CRM-Administratoren überprüfen, um die Grundursache zu beheben. Führen Sie die folgenden Schritte aus, um Probleme mit der CRM-Synchronisierung für Ihre Instanz zu dokumentieren.

## Protokollierung von CRM-Synchronisierungsfehlern

Laden Sie vor dem Einstieg die [CRM-Synchronisierungs-Fehlerprotokollvorlage](/help/tutorial-inherited-instance/_assets/downloads/Adobe-Marketo-Engage_CRM-Sync-Error-Log-Template.xlsx).

**Schritt 1:** Navigieren Sie zu *[!UICONTROL Admin] Abschnitt* in Marketo Engage. under *[!UICONTROL Integration]* klicken *[!DNL Salesforce]*, *[!DNL Microsoft Dynamics]* oder *[!DNL Veeva]*, abhängig von [!DNL CRM] Sie verwenden dann die *[!UICONTROL Synchronisierungsfehler]* Registerkarte.

**Schritt 2:** Sie können zwischen [Exportieren Sie die Fehlerdatensätze als [!DNL CSV] Datei über die [!UICONTROL Filter] panel](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.html#filter-sync-errors){target="_blank"}. Wenn Sie nur wenige Stunden Zeit haben, kopieren und einfügen Sie direkt aus dem *[!UICONTROL Synchronisierungsfehler]* -Tab wäre der richtige Weg.

**Schritt 3:** Notieren Sie das Datum, an dem der Fehler aufgetreten ist.

**Schritt 4:** Geben Sie die Anzahl der von diesem Fehler betroffenen Datensätze an. (Manchmal gibt Ihr CRM-System nur einen Fehler für eine Person aus. Manchmal wird es viele Personen mit demselben Fehler gleichzeitig geben.)

**Schritt 5:** Notieren Sie die E-Mail-Adresse einer Person, die von dem Fehler betroffen ist. Dadurch können Sie die Fehler einfach beim CRM-Administrator referenzieren und besprechen.

**Schritt 6:** Fügen Sie Links zum Personendatensatz in [!DNL Marketo Engage] und [!UICONTROL CRM-Lead/Kontakt] Aufzeichnungen dieser Person.

**Schritt 7:** Fügen Sie in der letzten Spalte den tatsächlichen Text des Fehlers ein.

## Wie geht es weiter?

**Identifizieren Sie Fehlercodes:** Die Fehlercodes finden Sie in den Beschreibungen in der Entwicklerdokumentation [Tabelle mit Fehlercodes auf Antwortebene](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes){target="_blank"} und finden Sie die typischen nächsten Schritte zur Behebung der Fehler.

## Autoren

**Amy Goldfine**\
Adobe Marketo Champion(2022)
*Senior Manager, Marketing Operations, Iterable*

![Amy Goldfine](/help/tutorial-inherited-instance/_assets/authors/Customer_Author_Amy_Goldfine.png){width="25%"}

**Amy Chiu**
*Adoption &amp; Retention Marketing Manager unter Adobe*

![Amy Chiu](/help/tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width="25%"}

