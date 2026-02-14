---
title: "getVehicleRimImages"
topic_id: "7523"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugbilder Funktionen > getVehicleRimImages"
---

# getVehicleRimImages

Beschreibung

Die Funktion getVehicleRimImages liefert die Felgengrafiken zu einem DAT €uropa-Code® in Abhängigkeit von Restriktion, Bauzeit Land und Container.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| datECode | String | DAT €uropa-Code® | Gültiger DAT €uropa-Code® (11 oder 15 Stellen) | X |
| constructionTime | Integer | Bauzeit | Gültige DAT-Bauzeit (4 Stellen) |  |
| container | String | Container | Gültiger Container (5 Stellen) |  |
| restriction | Enumeration | ALL / REPAIR / APPRAISAL |  | X |

Rückgabe

Liste der vorhandenen Felgengrafiken mit Name, AV-Nummer und Binärdaten des Bildes
als Base64-Format kodierten String.

WSDL

https://<HOST>/<PRODUKT>/<PROTOKOLL>/<SERVICE>?wsdl

Serviceaufruf

https://<HOST>/<PRODUKT>/<PROTOKOLL>/<SERVICE>

Die Schnittstellenfunktionen der DAT €uropa-Code® Fahrzeugauswahl sind sowohl im gleichnamigen Produkt, als auch in allen anderen Produkten
enthalten.

Produkte

| Name | ProductVariant | <HOST> | <PRODUKT> | <PROTOKOLL> | <SERVICE> |
| --- | --- | --- | --- | --- | --- |
| DAT €uropa-Code Fahrzeugauswahl |  | www.datgroup.com | DATECodeSelection | services | VehicleImagery |
| SilverDAT calculatePro |  | www.datgroup.com | VehicleRepairOnline | services | VehicleImagery |
| SilverDAT calculateExpert | calculateExpert | www.datgroup.com | VehicleRepairOnline | services | VehicleImagery |
| SilverDAT valuateFinance |  | www.datgroup.com | FinanceLine | soap | VehicleImagery |
| SilverDAT valuateExpert | valuateNG.expert | www.datgroup.com | valuateNG | soap | VehicleImagery |
| SilverDAT 3 Pro | DAT | www.datgroup.com | myClaim | soap/v2 | VehicleImagery |
| SilverDAT 3 myclaim | abhängig vom jeweiligen Netz | www.datgroup.com | myClaim | soap/v2 | VehicleImagery |
