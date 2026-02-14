---
title: "JSON Web Token Authentication (DAT-AuthorizationToken)"
topic_id: "14087"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > Authentifizierung der SilverDAT Webservices > JSON Web Token Authentication (DAT-AuthorizationToken)"
---

# JSON Web Token Authentication (DAT-AuthorizationToken)

Für die Authentifizierung mittels DAT-AuthorizationToken muss zuerst über DAT-Webservices das DAT-AuthorizationToken unter Angabe der Authentifizierungsparameter erzeugt werden.

Beim eigentlichen Aufruf der gewünschten DAT-Webservice-Funktion werden die Informationen

- DAT-AuthorizationToken
- DAT-ProductVariant (optional)

angegeben.

Wichtig:

Die Angabe des Parameters DAT-ProductVariant übersteuert den bei Erzeugung des DAT-AuthorizationToken angegebenen Wert für productVariant.

Gültigkeit des DAT-AuthorizationToken

Das DAT-AuthorizationToken hat eine Gültigkeit von 30 Minuten.

Erzeugung des DAT-AuthorizationToken

Zur Erzeugung des DAT-AuthorizationToken stehen folgende Möglichkeiten zur Verfügung

- SOAP-Request "generateToken" an den [AuthenticationService der jeweiligen Anwendung](#showid/14126 "SOAP-Request generateToken")
- Http POST-Request an den [AuthorizationManager tokenService](#showid/14131 "HTTP POST-Request an den AuthorizationManager tokenService")

Verwendung des DAT-AuthorizationToken

Bei Aufruf der Produktservice-Funktion werden die Informationen

- DAT-AuthorizationToken
- DAT-ProductVariant (optional)

als HTTP-Header angegeben:

Wichtig:

Die Angabe des Parameters DAT-ProductVariant übersteuert den bei Erzeugung des DAT-AuthorizationToken angegebenen Wert für productVariant.
