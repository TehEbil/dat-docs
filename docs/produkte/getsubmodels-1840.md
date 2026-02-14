---
title: "getSubModels"
topic_id: "1840"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getSubModels"
---

# getSubModels

Beschreibung

Funktion zur Auswahl des Untertyps in Abhängigkeit von Fahrzeugart, Hersteller und
Haupttyp.

Die optionalen Parameter constructionTimeFrom und constructionTimeTo schränken den Bauzeitraum ein, in dem der Untertyp gültige Modelle haben soll, die
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
| vehicleType | Integer | [getVehicleTypes](#showid/1904 "getVehicleTypes") | Fahrzeugart | X |
| Manufacturer | Integer | [getManufacturers](#showid/1834 "getManufacturers") | Hersteller | X |
| BaseModel | Integer | [getBaseModels](#showid/1838 "getBaseModelsN") | Haupttyp | X |
| constructionTimeFrom | Integer | [getConstructionPeriods](#showid/8152 "getConstructionPeriodsN") oder 0 - 9999 | Bauzeit von |  |
| constructionTimeTo | Integer | [getConstructionPeriods](#showid/8152 "getConstructionPeriodsN") oder 0 - 9999 | Bauzeit bis |  |

Rückgabe

Liste der vorhandenen Untertypen und ihren Bezeichnungen analog zur übergebenen Fahrzeugart,
Hersteller und Haupttyp und ggf. Bauzeitraum.

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
