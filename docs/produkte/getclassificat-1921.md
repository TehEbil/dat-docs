---
title: "getClassificationGroups"
topic_id: "1921"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getClassificationGroups"
---

# getClassificationGroups

Beschreibung

Dieser Service ermittelt Fahrzeugart, Hersteller, Haupt- und Untertyp und die damit
verbundenen Ausstattungsgruppen.

Die zur Untertypvariante notwendigen klassifizierenden AV (Pflicht- und optionale
Felder) unterscheiden NICHT nach Fahrzeugart, sondern nach dem Fahrzeugaufbau bzw.
der Fahrzeugklasse. Da die Fahrzeugart PKW gleich 3 Fahrzeugarten umfasst, nämlich
PKW, Geländewagen/SUV und Kleintransporter/Transporter, kann mit dieser Funktion die
Klassifizierungsgruppe zur genaueren Definition der Fahrzeugart geholt werden.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| restriction | Enumeration | ALL / REPAIR / APPRAISAL | Alle Daten / nur FI-Daten / nur FB-Daten durchsuchen | X |
| vehicleType | Integer | getVehicleTypes | Fahrzeugart | X |
| manufacturer | Integer | getManufacturers | Hersteller | X |
| baseModel | Integer | getBaseModels | Haupttyp | X |
| subModel | Integer | getSubModels | Untertyp | X |

Rückgabe

Liste der Klassifizierungsgruppen

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
