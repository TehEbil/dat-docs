---
title: "getVehicleData"
topic_id: "1987"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getVehicleData"
---

# getVehicleData

Beschreibung

Mit diesem Serviceaufruf lassen sich die Fahrzeugdaten zu einem DAT €uropa-Code® inklusive Marktindex, die Ausstattungen als Liste und die technischen Daten (siehe
hierzu auch die Techinfo der Vxs-Struktur) abrufen.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| Restriction | Enumeration | ALL / REPAIR / APPRAISAL | Alle Daten / nur FI-Daten / nur FB-Daten durchsuchen | X |
| DatECode | String | DAT €uropa-Code® | Gültiger DAT €uropa-Code® | X |
| container | String | Marktindex | Gültiger Marktindex |  |
| constructionTime | Integer | s. [date2ConstructionTime](date2construct-1807.md) | Bauzeit | X |

Wird der optionale Parameter "container" nicht übergeben, ist die Menge der ausgegebenen
technischen Daten erheblich kleiner. Deshalb: Wenn möglich, den Marktindex angeben.

Rückgabe

Fahrzeugdaten im VXS-Format, beginnend mit Element Vehicle[TechInfo]; zusätzlich auch noch alle möglichen KBA-Nummern.

Wichtiger Hinweis:

Um den größtmöglichen Umfang der technischen Daten zu erhalten muss, der optionale
Parameter container übergeben werden!

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
