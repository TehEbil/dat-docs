---
title: "getBaseModelsN"
topic_id: "1838"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getBaseModelsN"
---

# getBaseModelsN

Mit der Schnittstellenfunktion getBaseModelsN wurde die alte Funktion getBaseModels um einen zusätzlichen Parameter (withRepairIncomplete) erweitert. Die alte Schnittstellenfunktion ist hiermit abgekündigt und wird voraussichtlich
Anfang 2020 abgeschaltet!

Beschreibung

Funktion zur Auswahl des Haupttyps in Abhängigkeit zu Fahrzeugart und Hersteller.

Die optionalen Parameter constructionTimeFrom und constructionTimeTo schränken den Bauzeitraum ein, in dem der Haupttyp gültige Modelle haben soll, die
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
| vehicleType | Integer | [getVehicleTypes](getvehicletype-1904.md) | Fahrzeugart | X |
| Manufacturer | Integer | [getManufacturers](getmanufacture-1834.md) | Hersteller | X |
| withRepairIncomplete | Boolean | true, false oder null | Falls true und falls Restriction == "REPAIR", wird das Ergebnis zusätzlich auch solche Haupttypen enthalten, deren Datenstand noch unvollständig ist (lediglich die Ersatzteildaten sind vorhanden). |  |
| constructionTimeFrom | Integer | [getConstructionPeriodsN](getconstructio-8152.md) oder 0 - 9999 | Bauzeit von |  |
| constructionTimeTo | Integer | [getConstructionPeriodsN](getconstructio-8152.md) oder 0 - 9999 | Bauzeit bis |  |

Rückgabe

Liste der vorhandenen Haupttypen und ihrer Bezeichnungen analog zur übergebenen Fahrzeugart./Herstellerschlüssel
und ggf. Bauzeitraum.

Im Falle von unvollständigen Haupttypen werden zusätzlich zu Nummer und Name auch
folgende Attribute zurückgegeben:

- Attribut "repairIncomplete" mit Inhalt true
- Attribute "alternativeBaseType" mit Inhalt: die Nummer desjenigen Haupttyps, den die DAT als Ersatzhaupttyp vorschlägt.

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
