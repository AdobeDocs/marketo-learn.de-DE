---
title: Marketo-Anleitung zur API - Video zum Festlegen des Zugriffstokens in einer Variablen
description: Erfahren Sie, wie Sie die Postman-Anwendung einrichten und Variablen nutzen können, um Daten zur Wiederverwendbarkeit in der Variablen zu speichern.
feature: REST API
role: Admin, Developer
level: Experienced
doc-type: Technical Video
duration: 772
last-substantial-update: 2024-08-06T00:00:00.000Z
jira: KT-15548
exl-id: 4da86ed6-1072-4e0e-a648-16587badaeb3
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: dca84292-69e9-4116-a575-667d31fa060d
    internal-label: APIs
subfeature_v2:
  - id: cf1396d8-ab85-4e93-b35d-d9b573024abf
    internal-label: REST APIs
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
source-git-commit: 4768ecb20d4d9c70452ae084256928261f3a80eb
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 27%
---
# API-Hilfe – Festlegen des Zugriffstokens in einer Variablen

Erfahren Sie, wie Sie die Postman-Anwendung einrichten und Variablen nutzen, um Daten in der Variablen zur späteren Wiederverwendung zu speichern. Erfahren Sie außerdem, wie Sie Ihren ersten Marketo Engage-REST-API-Aufruf ausführen, um das Zugriffstoken zu erhalten.

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

* [Marketo Engage Developers-Dokumentation](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/authentication){target="_blank"}

>[!VIDEO](https://video.tv.adobe.com/v/3429275/?learn=on)
