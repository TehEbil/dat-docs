---
title: "getEquipmentLineOptions"
topic_id: "6382"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getEquipmentLineOptions"
---

# getEquipmentLineOptions

Beschreibung

Funktion zur Auswahl der verfügbaren Ausstattungslinie-Ausstattungsvarianten in Abhängigkeit
vom Basiscode (Fahrzeugart, Hersteller, Haupttyp, Untertyp) und (optional) bereits
gewählten Ausstattungsvarianten.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| restriction | Enumeration | ALL / REPAIR / APPRAISAL | Alle Daten / nur FI-Daten / nur FB-Daten durchsuchen | X |
| vehicleType | Integer | getVehicleTypes | Fahrzeugart | X |
| manufacturer | Integer | getManufacturers | Hersteller | X |
| baseModel | Integer | getBaseModels | Haupttyp | X |
| subModel | Integer | getSubModels | Untertyp | X |
| AvailableOptions | Integer |  | Bereits gewählte klassifizierende Ausstattungen, die die Ausstattungsmenge weiter einschränken. |  |

Rückgabe

Liste der verfügbaren Ausstattungslinie-Ausstattungsvarianten und ihren Bezeichnungen
entsprechend des übergebenen Basiscodes (Fahrzeugart, Hersteller, Haupttyp, Untertyp)
und der (optional) bereits gewählten Ausstattungsvarianten.

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
