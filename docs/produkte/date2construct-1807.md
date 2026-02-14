---
title: "date2ConstructionTime"
topic_id: "1807"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Konvertierungsoperationen > date2ConstructionTime"
---

# date2ConstructionTime

Beschreibung

Ermittelt aus einem Datum die DAT-kodierte Angabe für eine Bauzeit. Zum Umgang mit
Angaben zu Bauzeit gibt es die Operation date2ConstructionTime. Sie konvertiert aus einem Datum das Format in Angabe für Bauzeit bei der DAT. Die
Übergabe des Datums erfolgt in amerikanischer Schreibweise: YYYY-MM-DD.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| Date | Date | Datumswerte |  | X |

Rückgabe

Zurückgegeben wird die aus dem übergebenen Datum übersetzte DAT-kodierte Angabe Bauzeit.

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
