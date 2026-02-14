---
title: "getHgvPlatformSubModelData"
topic_id: "10802"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getHgvPlatformSubModelData"
---

# getHgvPlatformSubModelData

Beschreibung

Mit diesem Serviceaufruf lassen sich die Daten zu einem Lkw-Aufbau-Untertyp abrufen
(siehe hierzu auch das UpperBody-Element der Vxs-Struktur).

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| restriction | Enumeration | ALL / REPAIR / APPRAISAL | Alle / nur FI-DATEN / nur FB-Daten durchsuchen | X |
| hgvPlatformType | Integer |  | Lkw-Aufbauart | X |
| manufacturer | Integer |  | Lkw-Aufbau-Hersteller | X |
| baseModel | Integer |  |  | X |
| subModel | Integer |  |  | X |

Rückgabe

Lkw-Aufbau-Daten im VXS-Format, beginnend mit Element UpperBody.

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
