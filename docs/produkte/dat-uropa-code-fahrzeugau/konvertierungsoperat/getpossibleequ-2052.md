---
title: "getPossibleEquipmentN"
topic_id: "2052"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Konvertierungsoperationen > getPossibleEquipmentN"
---

# getPossibleEquipmentN

Diese Schnittstellenfunktion ist veraltet, bitte nutzen Sie getPossibleEquipment aus
dem VehicleSelectionSerice.

Beschreibung

Ermittelt anhand des übergebenen DAT €uropa-Code® nebst Marktindex die verfügbaren Ausstattungsvarianten.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| datECode | String | DAT €uropa-Code® | Gültiger DAT €uropa-Code® | X |
| container | String | Marktindex | Gültiger Marktindex | X |
| constructionTime | Integer | DAT-Notation Bauzeit | Bauzeit | X |

Rückgabe

Zurückgegeben werden folgende Werte:

| Name | Beschreibung |
| --- | --- |
| DatEquipmentId | DAT Ausstattungs-Nummer (AV-Code) |
| Description | Beschreibung |
| EquipmentGroup | Kürzel der Ausstattungsgruppe |
| EquipmentClass | Klassifizierungsnummer, falls vorhanden |
| OriginalPrice | Preis der Ausstattung |
| ContainedEquipmentPositions | Inhalt eines Ausstattungspaketes |

WSDL

https://<HOST>/<PRODUKT>/<PROTOKOLL>/<SERVICE>?wsdl

Serviceaufruf

https://<HOST>/<PRODUKT>/<PROTOKOLL>/<SERVICE>

Die Schnittstellenfunktionen der DAT €uropa-Code® Fahrzeugauswahl sind sowohl im gleichnamigen Produkt, als auch in allen anderen Produkten
enthalten.

Produkte

| Name | ProductVariant | <HOST> | <PRODUKT> | <PROTOKOLL> | <SERVICE> |
| --- | --- | --- | --- | --- | --- |
| DAT €uropa-Code Fahrzeugauswahl |  | www.datgroup.com | DATECodeSelection | services | ConversionFunctionsService |
| SilverDAT calculatePro |  | www.datgroup.com | VehicleRepairOnline | services | ConversionFunctionsService |
| SilverDAT calculateExpert | calculateExpert | www.datgroup.com | VehicleRepairOnline | services | ConversionFunctionsService |
| SilverDAT valuateFinance |  | www.datgroup.com | FinanceLine | soap | ConversionFunctionsService |
| SilverDAT valuateExpert | valuateNG.expert | www.datgroup.com | valuateNG | soap | ConversionFunctionsService |
| SilverDAT 3 Pro | DAT | www.datgroup.com | myClaim | soap/v2 | ConversionFunctionsService |
| SilverDAT 3 myclaim | abhängig vom jeweiligen Netz | www.datgroup.com | myClaim | soap/v2 | ConversionFunctionsService |
