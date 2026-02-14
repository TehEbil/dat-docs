---
title: "Fahrzeugidentifikation anhand Typcode Toyota"
topic_id: "9153"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Fahrzeugidentifikation anhand Typcode Toyota"
---

# Fahrzeugidentifikation anhand Typcode Toyota

Beschreibung

Die Funktion getVehicleIdentificationByTypecodeToyota liefert anhand des Toyota-Typcodes, Produktionsdatum und Ausstattungscodes (PPO-Codes) alle DAT €uropa-Code®, (DAT) Containers und AV. Aufgrund der Masse der Informationen erfolgt die Ausgabe
im VXS-Format.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| typeCode | String | Toyota-Typcode |  | X |
| manufacturer | enumeration | TOYOTA / LEXUS | Toyota oder Lexus | X |
| productionDate | Date | Datumswerte | Produktionsdatum | X |
| equipmentCode | String | ein oder mehrere Ausstattungscodes (PPO-Codes) | (optional) |  |
| colorCode | String | ein oder mehrere Farbcodes | (optional) |  |
| coverage | enumeration | ALL / WITH\_MANUFACTURER\_TEXTS /WITH\_PRICE\_LIST\_TIME | Optional kann über den Parameter coverage die zusätzliche Ausgabe der Herstellertexte und/oder der Preislisten-Bauzeit gesteuert werden. |  |
| restriction | enumeration | ALL / REPAIR / APPRAISAL | alle / nur FI-Daten / nur FB-Daten durchsuchen |  |

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
