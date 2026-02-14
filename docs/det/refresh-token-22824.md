---
title: "Refresh Token"
topic_id: "22824"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Funktionsreferenz > Anmeldung > Refresh Token"
---

# Refresh Token

| Funktionsname | Methode | Beschreibung | Ergebnis |
| --- | --- | --- | --- |
| refresh | POST | Erneuert den Zugangsschlüssel. | JSON-Web-Token |

Die Funktion erwartet keine Parameter im Request Body. Allerdings muss der Cookie
refreshToken, der von der Funktion login gesetzt wurde, im HTTP-Header übergeben werden. Ein Web-Browser tut dies beim Aufruf
automatisch (bei AJAX-Aufrufen muss die Option withCredentials = true gesetzt werden).

Der Refresh-Token verfügt über eine wesentlich längere Gültigkeitsdauer, als der Berechtigungs-Token
(accessToken). Dennoch läuft er irgendwann (üblicherweise nach einigen Stunden) ab. Ein neuer
Token kann nur mittels einer neuen Anmeldung über die Funktion login abgefragt werden.

Die Funktion liefert ein JSON-Objekt zurück. Das ausgegebene Objekt hat die folgenden
Eigenschaften:

| Rückgabewert | Typ | Beschreibung |
| --- | --- | --- |
| accessToken | String | Base64-kodierter und signierter Datensatz mit zeitlich beschränkter Gültigkeit. Wird zur Berechtigung anderen Funktionen im HTTP-Header unter "DAT-AuthorizationToken" übergeben. |
