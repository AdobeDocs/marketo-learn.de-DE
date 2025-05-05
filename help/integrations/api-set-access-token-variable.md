---
title: Marketo-Anleitung zur API - Video zum Festlegen des Zugriffstokens in einer Variablen
description: Erfahren Sie, wie Sie die Postman-Anwendung einrichten und Variablen nutzen können, um Daten zur Wiederverwendbarkeit in der Variablen zu speichern.
feature: REST API
role: Admin, Developer
level: Experienced
doc-type: Technical Video
duration: 772
last-substantial-update: 2024-08-06T00:00:00Z
jira: KT-15548
exl-id: 4da86ed6-1072-4e0e-a648-16587badaeb3
source-git-commit: 3243c3047efa1bcb92581a58aafe17689ff945fd
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 24%

---

# API-Hilfe - Festlegen des Zugriffstokens in einer Variablen

Erfahren Sie, wie Sie die Postman-Anwendung einrichten und Variablen nutzen, um Daten in der Variablen zur späteren Wiederverwendung zu speichern. Außerdem lernen Sie, wie Sie Ihren ersten Marketo Engage-REST-API-Aufruf ausführen, um das Zugriffs-Token abzurufen.

>[!PREREQUISITES]
>
>Bevor Sie mit diesem Video beginnen, erstellen Sie einen Benutzernamen „Nur API“ mit einer API-Rolle und einen Launchpad-Service. Führen Sie die Schritte in den folgenden Artikeln aus:
>
>* [Erstellen einer Benutzerrolle nur für API](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user-role){target="_blank"}
>
>* [Nur API-Benutzer erstellen](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user){target="_blank"}
>
>* [Erstellen eines benutzerdefinierten Services zur Verwendung mit der REST-API](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api){target="_blank"}

**In diesem Video verwendete Verweise:**

* Marketo-Authentifizierungsendpunkt: `{{{}base_url{}}}/identity/oauth/token?grant_type=client_credentials&client_id={{{}client_id{}}}&client_secret={{{}client_secret{}}}`

* JS-Skript zum Abrufen von access_token aus dem Antworttext (befindet sich auf der Registerkarte Skripte: ):

```
var jsonData = pm.response.json();
pm.environment.set("access_token", jsonData.access_token);
```

* Dokumentation für [Marketo Engage-Entwickler](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/authentication){target="_blank"}

>[!VIDEO](https://video.tv.adobe.com/v/3453992/?learn=on&captions=ger)
