---
title: "Anmerkung zum REST Service"
topic_id: "16892"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Börsendaten via webScan REST-API abrufen > Anmerkung zum REST Service"
---

# Anmerkung zum REST Service

- Method: POST HTTP/1.1
- Content-Type: application/json
- Accept: application/json
- Current Version: v1
- Endpoint: https://www.dat.de/FinanceLine/rest/{Version}/marketData/{Funktionsname}/
- Authentifizierung: Authentifizierungstoken im Header
- Body: JSON String

Versionierung:

Hinweis: Die URL beinhaltet einen Versionierungsstring. Änderungen werden dabei frühzeitig
im Newsletter angekündigt.

Authentifizierung:

Die Authentifizierung findet mittels eines Authentifizierungstokens im Header der
POST Anfrage statt. Zum generieren des Tokens lesen Sie bitte den Bereich [Authentifizierung der SilverDAT](../../../allgemein/dat-developers-guide/authentifizierung-de/index.md) Webservices.

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
