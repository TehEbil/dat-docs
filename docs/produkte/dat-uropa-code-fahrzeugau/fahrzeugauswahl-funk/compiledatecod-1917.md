---
title: "compileDatECode"
topic_id: "1917"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > compileDatECode"
---

# compileDatECode

Beschreibung

Funktion zur Ermittlung des DAT €uropa-Code® in Abhängigkeit zum Basiscode (Fahrzeugart, Hersteller, Haupttyp, Untertyp) und der
gewählten klassifizierenden Ausstattung. Nachdem Fahrzeugart, Hersteller, Haupt- und
Untertyp sowie die für den jeweiligen Fahrzeugaufbau relevanten klassifizierenden
Ausstattungen bestimmt wurden, bildet sich der DAT €uropa-Code®. Dabei entsteht aus den einzelnen klassifizierenden Ausstattungen ein 4-stelliger
Code für die Untertypvariante als fünftes Element im DAT €uropa-Code®.

| Fahrzeugart | Hersteller | Haupttyp | Untertyp | Untertypvariante |
| --- | --- | --- | --- | --- |
| 2-stellig | 3-stellig | 3-stellig | 3-stellig | 4-stellig |
| 01 | 060 | 028 | 004 | 0008 |

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| restriction | Enumeration | ALL / REPAIR / APPRAISAL | Alle Daten / nur FI-Daten / nur FB-Daten durchsuchen | X |
| vehicleType | Integer | getVehicleTypes | Fahrzeugart | X |
| manufacturer | Integer | getManufacturers | Hersteller | X |
| baseModel | Integer | getBaseModels | Haupttyp | X |
| subModel | Integer | getSubModels | Untertyp | X |
| selectedOptions | Integer | s. [Klassifizierende Ausstattungen](../klassifizieren-1820.md) | Klassifizierende Ausstattung | X |

Rückgabe

1 gültiger DAT €uropa-Code®

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
