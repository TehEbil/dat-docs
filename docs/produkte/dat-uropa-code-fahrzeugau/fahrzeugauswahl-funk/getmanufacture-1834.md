---
title: "getManufacturers"
topic_id: "1834"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getManufacturers"
---

# getManufacturers

Beschreibung

Funktion zur Auswahl des Herstellers in Abhängigkeit zur Fahrzeugart.

Die optionalen Parameter constructionTimeFrom und constructionTimeTo schränken den Bauzeitraum ein, in dem der Hersteller gültige Modelle haben soll, die
zurückgegeben werden. Ungültige Eingaben werden ignoriert.

constructionTimeFrom und constructionTimeTo können auch allein gesetzt werden. Dann ist die Logik wie folgt:

constructionTimeFrom = leer & constructionTimeTo != leer

-> Zeige alle Fahrzeuge bis "Bauzeit bis"

und

constructionTimeFrom != leer & constructionTimeTo = leer

-> Zeige alle Fahrzeuge ab "Bauzeit von"

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| Restriction | Enumeration | ALL / REPAIR / APPRAISAL | Alle / nur FI-DATEN / nur FB-Daten durchsuchen | X |
| vehicleType | Integer | [getVehicleTypes](getvehicletype-1904.md) | Fahrzeugart |  |
| constructionTimeFrom | Integer | [getConstructionPeriods](getconstructio-8152.md) oder 0 - 9999 | Bauzeit von |  |
| constructionTimeTo | Integer | [getConstructionPeriods](getconstructio-8152.md) oder 0 - 9999 | Bauzeit bis |  |

Rückgabe

Liste der vorhandenen Herstellerschlüssel und ihrer Kurzbezeichnungen analog zur übergebenen
Fahrzeugart und ggf. Bauzeitraum.

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
