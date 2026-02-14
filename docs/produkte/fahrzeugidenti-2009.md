---
title: "Fahrzeugidentifikation Italien - anhand Kennzeichenabfrage"
topic_id: "2009"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Fahrzeugidentifikation Italien - anhand Kennzeichenabfrage"
---

# Fahrzeugidentifikation Italien - anhand Kennzeichenabfrage

Beschreibung

Die Funktion getVinByLicencePlateItaly ermittelt anhand des Kennzeichens die VIN-Nummer, das Erstzulassungsdatum und weitere
Daten des Fahrzeugs.

Diese Schnittstellenfunktion ist nur für das Datenland Italien verfügbar.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| licencePlate | String |  | amtliches Kennzeichen (z.B. „AB12345“) | X |

Rückgabe

| Name | Datentyp | Beschreibung | (italienisch) |
| --- | --- | --- | --- |
| vin | String | Fahrgestellnummer | telaio |
| licencePlate | String | amtliches Kennzeichen | targa |
| initialRegistration | Date | Erstzulassungsdatum | data prima immatricolazione |
| modelPermissionNumber | String | Zulassungsnummer des Modells | codice omologazione |
| engineCode | String | Motorcode | codice motore |
| lastRevisionDate | Date | Datum der letzten Untersuchung | data ultima revisione |

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
