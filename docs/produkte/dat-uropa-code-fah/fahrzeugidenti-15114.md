---
title: "Fahrzeugidentifikation anhand Typcode"
topic_id: "15114"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Fahrzeugidentifikation anhand Typcode"
---

# Fahrzeugidentifikation anhand Typcode

Beschreibung

Die Funktion getVehicleIdentificationByTypecode liefert anhand der Typcodes, Produktionsdatum und Ausstattungscodes (PPO-Codes) alle DAT €uropa-Code®, (DAT) Containers und AV. Aufgrund der Menge der Informationen erfolgt die Ausgabe
im VXS-Format.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| typeCode | String | Typcode | Typcode des Fahrzeuges | X |
| manufacturerKey | Integer | Herstellerschlüssel | DAT Schlüsselnummer des Herstellers | X |
| productionDate | Date | Datumswerte | Produktionsdatum | X |
| equipmentCodes | String | ein oder mehrere Ausstattungscodes (PPO-Codes) | (optional)  Wird für Hersteller 860 oder 487 (Toyota oder Lexus) nicht berücksichtigt! |  |
| colorCode | String | ein oder mehrere Farbcodes | (optional)  Wird für Hersteller 860 oder 487 (Toyota oder Lexus) nicht berücksichtigt! |  |
| coverage | enumeration | ALL / WITH\_MANUFACTURER\_TEXTS /WITH\_PRICE\_LIST\_TIME | Optional kann über den Parameter coverage die zusätzliche Ausgabe der Herstellertexte und/oder der Preislisten-Bauzeit gesteuert werden. |  |
| restriction | enumeration | ALL / REPAIR / APPRAISAL | alle / nur FI-Daten / nur FB-Daten durchsuchen |  |

Hinweis zu Parameter colorCode

Hier finden nur solche Angaben Berücksichtigung, bei denen der String aus drei Bestandteilen
besteht, die durch ein |-Zeichen (Pipe-Zeichen) voneinander getrennt sind, also z.B.
„A1|XXX|Freitext“.

Beim ersten Bestandteil („A1“) handelt es sich um die Color-ID, gültig sind hierfür:

- „A1“ (Bedeutung: Außenfarbe 1)
- „A2“ (Bedeutung: Außenfarbe 2)
- „I1“ (Bedeutung: Innenfarbe 1)
- „I2“ (Bedeutung: Innenfarbe 2)
- „PF“ (Bedeutung: Polsterfarbe)
- „PM“ (Bedeutung: Polstermaterial)

Beim zweiten Bestandteil („XXX“) handelt es sich um den ColorCode, also der Farbcode aus Sicht des Herstellers.

Beim dritten Bestandteil handelt es sich um einen Langtext der Farbe aus Sicht des
Herstellers.

Rückgabe

Es wird eine Liste möglicher Fahrzeugidentifikationen nach DAT im VXS-Format, beginnend
mit Element Dossier, zurückgeliefert. Zusätzlich werden noch alle möglichen KBA-Nummern zurückgegeben. Im Element Vehicle befindet sich das Element VINResult, darin sind die Informationen vom Hersteller enthalten.

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
