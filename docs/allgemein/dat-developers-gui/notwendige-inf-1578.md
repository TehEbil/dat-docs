---
title: "Notwendige Informationen"
topic_id: "1578"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > Authentifizierung der SilverDAT Webservices > Notwendige Informationen"
---

# Notwendige Informationen

Untenstehende Parameter werden für die Authentifizierung benötigt.

Diese Informationen werden bei der Erzeugung des DAT-AuthorizationToken verwendet.

| Name | Datentyp | mögliche Werte | Beschreibung | Pflicht |
| --- | --- | --- | --- | --- |
| customerNumber | String | 1234567 | Gültige Kundennr. mit Lizenz zum Produkt | X |
| customerLogin | String | myuser | Gültiger Benutzername zur o.g. Kundennr. | X |
| customerPassword | String | password | Persönliches Kennwort des Benutzers. | X |
| interfacePartnerNumber | String | 1234567 | Gültige Kundennr. des Schnittstellenpartners mit Lizenz zum Produkt | X |
| interfacePartnerSignature | String | AF4662380.... | Generierter SHA256 hash für den Schnittstellenpartner. (Kann NICHT selbst erzeugt werden, wird von DAT zur Verfügung gestellt) | X |
| productVariant | String | valuateNG.expert | calculateExpert | Die Übergabe der Produktvariante ist ausschließlich bei den Produkten SilverDAT valuateExpert und SilverDAT calculateExpert zwingend notwendig. |  |

Mit dem DAT-AuhorizationToken und dem optionalen Parameter DAT-ProductVariant können danach die Schnittstellenfunktionen aufgerufen werden.

| Name | Datentyp | mögliche Werte | Beschreibung | Pflicht |
| --- | --- | --- | --- | --- |
| DAT-AuthorizationToken | String | 670a8f439c... | Generierter SHA256 hash für den Benutzer. | X |
| DAT-ProductVariant | String | valuateNG.expert | Produktvariante |  |
