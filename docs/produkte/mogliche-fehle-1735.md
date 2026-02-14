---
title: "Mögliche Fehlercodes updateCustomer"
topic_id: "1735"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Customer Service > Customer Service Schnittstellenoperationen > Kundendaten ändern: updateCustomer > Mögliche Fehlercodes updateCustomer"
---

# Mögliche Fehlercodes updateCustomer

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| Server.authorizationFailed | Server.authorizationFailed | Der Fehler kann eintreten, wenn falsche Autorisierungsdaten eingegeben wurden bspw. customerNumber, customerLogin, customerSignature, interfacePartnerNumber oder interfacePartnerSignature.  Oder: Der Benutzer hat keine Lizenz für das erforderliche Produkt. |
| Server.requireCode | Server.requireCode | Wenn mindestens ein Feld fehlt: externalCustomerID |
| Server.internalError | Server.internalError | Interner Fehler im SOAP- Service. |
| Server.valueNotFound | Server.valueNotFound | Die angegebene externalCustomerID wurde in der DAT- Datenbank nicht gefunden. |
