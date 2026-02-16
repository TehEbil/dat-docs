---
title: "Mögliche Fehlercodes createCustomer"
topic_id: "1734"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Customer Service > Customer Service Schnittstellenoperationen > Neuen Kunden anlegen oder deaktivierten Kunden reaktivieren: createCustomer > Mögliche Fehlercodes createCustomer"
---

# Mögliche Fehlercodes createCustomer

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| Server.authorizationFailed | Server.authorizationFailed | Der Fehler kann eintreten, wenn  falsche Autorisierungsdaten eingegeben wurden, beispielsweise:   - customerNumber - customerLogin - customerSignature - interfacePartnerNumber - interfacePartnerSignature   oder der Benutzer hat keine Lizenz für das erforderliche Produkt. |
| Server.requireCode | Server.requireCode | Wenn mindestens ein Feld fehlt:  Kundendaten: "name1", "street", "zip", "city", "country", "customerEmail", "externalCustomerID", "filterName". |
| Server.internalError | Server.internalError | Interner Fehler im SOAP- Service. |
| Server.internalError | Cannot initialize credentials. The license is not valid or user limit reached | Die übergebenen Parameter können nicht genutzt werden. Bitte prüfen Sie, ob Sie das Recht haben, neue Kunden anzulegen oder ob das Userlimit für diese Kundennummer erreicht ist. |
| Server.emailNotValid | The E-Mail is not valid! Example: max.mustermann@dat.de | Dieser Fehler tritt auf, wenn eine ungültige E-Mail eingetragen wird. |
| Server.CustomerCountryError | Please enter a valid customer country code! | Tritt auf, wenn im Feld beim "customerCountry" ein ungültiger Wert eingetragen wird. |
