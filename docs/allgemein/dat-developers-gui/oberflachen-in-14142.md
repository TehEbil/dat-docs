---
title: "Oberflächen-Integration"
topic_id: "14142"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > Authentifizierung der SilverDAT Webservices > JSON Web Token Authentication (DAT-AuthorizationToken) > Oberflächen-Integration"
---

# Oberflächen-Integration

Nachfolgend ein Beispiel für die Oberflächenintragtion mit JavaScript, bei erfolgreicher
Token-Erzeugung wird im Beispiel die Funktion "initExternal" ausgeführt:

```
$.ajax( {
   url: 'https://www.dat.de/AuthorizationManager/service--/endpoint/tokenService',
   data: {
      payload: JSON.stringify({
         action: "generateToken",
         customerNumber: "1234567",
         user: "userName",
         password: "userPassword",
         interfacePartnerNumber: "1765432",
         interfacePartnerSignature: "xxxxxxxxxxxxxxxxxx",
         productVariant: "valuateNG.expert"
      })
   },
   type: 'POST',
   error: function (error) { alert(error); },
   success: initExternal
});
```

Der Parameter productVariant ist optional. Diesen bitte nur verwenden wenn es für das verwendete DAT Produkt erforderlich
ist.
