---
title: "getPossibleEquipment"
topic_id: "31540"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getPossibleEquipment"
---

# getPossibleEquipment

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
| DAT €uropa-Code Fahrzeugauswahl |  | www.datgroup.com | DATECodeSelection | services | VehicleSelectionService |
| SilverDAT calculatePro |  | www.datgroup.com | VehicleRepairOnline | services | VehicleSelectionService |
| SilverDAT calculateExpert | calculateExpert | www.datgroup.com | VehicleRepairOnline | services | VehicleSelectionService |
| SilverDAT valuateFinance |  | www.datgroup.com | FinanceLine | soap | VehicleSelectionService |
| SilverDAT valuateExpert | valuateNG.expert | www.datgroup.com | valuateNG | soap | VehicleSelectionService |
| SilverDAT 3 Pro | DAT | www.datgroup.com | myClaim | soap/v2 | VehicleSelectionService |
| SilverDAT 3 myclaim | abhängig vom jeweiligen Netz | www.datgroup.com | myClaim | soap/v2 | VehicleSelectionService |
