---
title: "getHgvPlatformManufacturers"
topic_id: "10790"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getHgvPlatformManufacturers"
---

# getHgvPlatformManufacturers

Beschreibung

Funktion zur Auswahl des Lkw-Aufbau-Herstellers in Abhängigkeit zur Lkw-Aufbauart.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| restriction | Enumeration | ALL / REPAIR / APPRAISAL | Alle / nur FI-DATEN / nur FB-Daten durchsuchen | X |
| hgvPlatformType | Integer |  | Lkw-Aufbauart | X |

Rückgabe

Liste der vorhandenen Herstellerschlüssel und ihrer Kurzbezeichnungen analog zur übergebenen
Fahrzeugart.

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
