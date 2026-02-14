---
title: "Fahrzeugidentifikation Niederlande - anhand Kennzeichenabfrage"
topic_id: "16795"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Fahrzeugidentifikation Niederlande - anhand Kennzeichenabfrage"
---

# Fahrzeugidentifikation Niederlande - anhand Kennzeichenabfrage

Beschreibung

Die Funktion getVinByLicencePlateNetherlands ermittelt anhand des Kennzeichens die VIN-Nummer des Fahrzeugs.

Diese Schnittstellenfunktion ist nur für das Datenland Niederlande verfügbar.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| licencePlate | String |  | amtliches Kennzeichen (z.B. „AB12345“) | X |

Rückgabe

| Name | Datentyp | Beschreibung |  |
| --- | --- | --- | --- |
| vin | String | Fahrgestellnummer |  |
| licencePlate | String | amtliches Kennzeichen |  |

WSDL

https://<HOST>/<PRODUKT>/<PROTOKOLL>/<SERVICE>?wsdl

Serviceaufruf

https://<HOST>/<PRODUKT>/<PROTOKOLL>/<SERVICE>

Die Schnittstellenfunktionen der DAT €uropa-Code® Fahrzeugauswahl sind sowohl im gleichnamigen Produkt, als auch in allen anderen Produkten
enthalten.

Produkte

| Name | ProductVariant | <HOST> | <PRODUKT> | <PROTOKOLL> | <SERVICE> |
| --- | --- | --- | --- | --- | --- |
| DAT €uropa-Code Fahrzeugauswahl |  | www.datgroup.com | DATECodeSelection | services | VehicleIdentificationService |
| SilverDAT calculatePro |  | www.datgroup.com | VehicleRepairOnline | services | VehicleIdentificationService |
| SilverDAT calculateExpert | calculateExpert | www.datgroup.com | VehicleRepairOnline | services | VehicleIdentificationService |
| SilverDAT valuateFinance |  | www.datgroup.com | FinanceLine | soap | VehicleIdentificationService |
| SilverDAT valuateExpert | valuateNG.expert | www.datgroup.com | valuateNG | soap | VehicleIdentificationService |
| SilverDAT 3 Pro | DAT | www.datgroup.com | myClaim | soap/v2 | VehicleIdentificationService |
| SilverDAT 3 myclaim | abhängig vom jeweiligen Netz | www.datgroup.com | myClaim | soap/v2 | VehicleIdentificationService |
