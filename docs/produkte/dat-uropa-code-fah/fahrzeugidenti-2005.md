---
title: "Fahrzeugidentifikation Schweiz - anhand Kennzeichen, Stammnummer oder Typenscheinnummer"
topic_id: "2005"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Fahrzeugidentifikation Schweiz - anhand Kennzeichen, Stammnummer oder Typenscheinnummer"
---

# Fahrzeugidentifikation Schweiz - anhand Kennzeichen, Stammnummer oder Typenscheinnummer

Beschreibung

Die Funktion getVehicleIdentificationByCodeSwitzerland liefert anhand des Kennzeichens, der Stammnummer oder der Typenscheinnummer die möglichen
DAT €uropa-Codes® und deren Marktindizes. Aufgrund der Masse der Informationen erfolgt die Speicherung
im VXS-Format.

Diese Schnittstellenfunktion ist nur für das Datenland Schweiz verfügbar.

Diese Operation führt eine vollständige Fahrzeugidentifizierung anhand des Kennzeichens,
der Stammnummer oder der Typenscheinnummer durch. Sie liefert eine Liste mit Elementen
des folgenden Umfangs:

- DAT €uropa-Code®
- Fahrzeugartbenennung
- Herstellerbenennung
- Haupttypbenennung
- Untertypbenennung
- Benennungen der klassifizierenden Ausstattungen der Untertypvariante
- Liste der Marktindizes und deren Bezeichnungen

Es muss eine Land-Sprach-Kombination gemäß ISO 639-1 und ISO 3166 ALPHA-2 übergeben
werden, um Benennungen in abweichender Sprache abzufragen. Als Land sollte allerdings
immer „CH“ für Schweiz angegeben werden.

Ebenfalls optional muss über den Filter für "FB", "FI" und "Alle" eingeschränkt werden
können. Sollte der Filter nicht übergeben werden ist "Alle" automatisch als Standard
heranzuziehen.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| licencePlate | String |  | amtliches Kennzeichen (z.B. „BE 12345“) | X (\*) |
| baseNumber | String |  | Stammnummer 9 bzw. 12 stellig (z.B. "136.936.153" oder "136.936.153.123") | X (\*) |
| typeNoteNumber | String | genau 6 Stellen, die erste und die letzten drei Stellen als Ziffern, die zweite als Großbuchstabe, die dritte als Ziffer oder Großbuchstabe | Typenscheinnummer (z.B. „1LC582“) | X (\*) |
| restriction | enumeration | ALL / REPAIR / APPRAISAL | alle / nur FI-Daten / nur FB-Daten durchsuchen |  |

(\*) Es muss einer der Parameter licencePlate, baseNumber oder typeNoteNumber angegeben werden.

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
