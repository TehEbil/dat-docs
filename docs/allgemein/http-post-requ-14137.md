---
title: "HTTP POST-Request (Beispiel)"
topic_id: "14137"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > Authentifizierung der SilverDAT Webservices > JSON Web Token Authentication (DAT-AuthorizationToken) > HTTP POST-Request an den AuthorizationManager tokenService > HTTP POST-Request (Beispiel)"
---

# HTTP POST-Request (Beispiel)

Das JSON-Objekt wird in einem HTTP POST-Request als HTTP Body "payload" übergeben.

```
{ 
    "action" : "generateToken",
    "customerNumber" : "1234567",
    "user" : "userName",
    "password" : "userPassword",
    "interfacePartnerNumber" : "1765432",
    "interfacePartnerSignature" : "xxxxxxxxxxxxxxxxxx",
    "productVariant" : "valuateNG.expert"
}
```

Der Parameter productVariant ist optional. Diesen bitte nur verwenden wenn es für das verwendete DAT Produkt erforderlich
ist.
