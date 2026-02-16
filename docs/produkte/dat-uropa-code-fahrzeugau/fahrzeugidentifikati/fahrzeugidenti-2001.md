---
title: "Fahrzeugidentifikation Österreich - anhand des österreichischen Nationalcodes"
topic_id: "2001"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Fahrzeugidentifikation Österreich - anhand des österreichischen Nationalcodes"
---

# Fahrzeugidentifikation Österreich - anhand des österreichischen Nationalcodes

Beschreibung

Die Funktion getVehicleIdentificationByNationalCodeAustria liefert anhand des österreichischen-Nationalcodes (NatCode) die möglichen DAT €uropa-Codes® und deren Marktindizes. Aufgrund der Masse der Informationen erfolgt die Speicherung
im VXS-Format.

Diese Schnittstellenfunktion ist nur für das Datenland Österreich verfügbar.

Diese Operation führt eine vollständige Fahrzeugidentifizierung anhand des österreichischen-Nationalcodes
durch. Sie liefert eine Liste mit Elementen des folgenden Umfangs:

- DAT €uropa-Code®
- Fahrzeugartbenennung
- Herstellerbenennung
- Haupttypbenennung
- Untertypbenennung
- Benennungen der klassifizierenden Ausstattungen der Untertypvariante
- Liste der Marktindizes und deren Bezeichnungen

Optional kann eine Land-Sprach-Kombination gemäß ISO 639-1 und ISO 3166 ALPHA-2 übergeben
werden, um Benennungen in abweichender Sprache abzufragen.

Ebenfalls optional muss über den Filter für "FB", "FI" und "Alle" eingeschränkt werden
können. Sollte der Filter nicht übergeben werden ist "Alle" automatisch als Standard
heranzuziehen.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| nationalCode | String | NatCode | Gültiger NatCode | X |
| restriction | enumeration | ALL / REPAIR / APPRAISAL | alle / nur FI-Daten / nur FB-Daten durchsuchen |  |

Rückgabe

Es wird eine Liste möglicher Fahrzeugidentifikationen nach DAT im VXS-Format, Container
Vehicle, zurückgeliefert.

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
