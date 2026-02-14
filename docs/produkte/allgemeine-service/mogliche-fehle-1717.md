---
title: "Mögliche Fehlercodes createOrUpdateUser"
topic_id: "1717"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Customer Service > Customer Service Schnittstellenoperationen > Benutzer anlegen oder ändern: createOrUpdateUser > Mögliche Fehlercodes createOrUpdateUser"
---

# Mögliche Fehlercodes createOrUpdateUser

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| Server.authorizationFailed | Server.authorizationFailed | Der Fehler kann eintreten, wenn falsche Autorisierungsdaten eingegeben wurden bspw. customerNumber, customerLogin, customerSignature, interfacePartnerNumber oder interfacePartnerSignature.  Oder: Der Benutzer hat keine Lizenz für das erforderliche Produkt. |
| Server.requireCode | Server.requireCode | Wenn mindestens ein Feld fehlt:  externalCustomerID |
| Server.internalError | Server.internalError | Interner Fehler im SOAP- Service. |
| Server.emailNotValid | The eMail is not valid! Example: max.mustermann@dat.de | Dieser Fehler tritt auf, wenn eine ungültige eMail eingetragen wird. |
| Server.CustomerCountryError | Please enter a valid customer country code! | Tritt auf, wenn beim Parameter CustomerCountry ein ungültiger Wert eingetragen wird. |
