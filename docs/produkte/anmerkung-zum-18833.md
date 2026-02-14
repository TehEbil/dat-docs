---
title: "Anmerkung zum REST Service"
topic_id: "18833"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Börsendaten via webScan REST-API abrufen > Anmerkung zum REST Service"
---

# Anmerkung zum REST Service

- Method: POST HTTP/1.1
- Content-Type: application/json
- Accept: application/json
- Current Version: v1
- Endpoint: https://www.dat.de/myClaim/rest/marketData/{Funktionsname}/
- Authentifizierung: Authentifizierungstoken im Header
- Body: JSON String

Authentifizierung:

Die Authentifizierung findet mittels eines Authentifizierungstokens im Header der
POST Anfrage statt. Zum generieren des Tokens lesen Sie bitte den Bereich [Authentifizierung der SilverDAT](#showid/1294 "Authentifizierung der SilverDAT Webservices") Webservices.

Übergabeformat:

| Header Element | Value |
| --- | --- |
| Dat-AuthorizationToken | eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.ey......DaR70 |

Die Übergabe der Funktionsparameter erfolgt grundsätzlich in der Form eines JSON Strings
und befindet sich immer unter dem Element "data":

```
{
  "data": {
    Funktionsparameter
  }
}
```

Rückgabeformat

Die Antwort der webScan Anfrage erfolgt als JSON String mit folgender Struktur:

```
{
  "data": {
    "marketData": {
      ...
    }
  }
}
```
