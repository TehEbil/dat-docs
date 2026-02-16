---
title: "Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, DVNs und Preishistorie"
topic_id: "17163"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, DVNs und Preishistorie"
---

# Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, DVNs und Preishistorie

Die Funktion getSparePartsDetailsByVIN() ermöglicht die Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, DVNs und Preishistorie anhand von Fahrzeugidentifikationsnummer und Ersatzteilnummer. Hier
erfolgt eine automatische kostenpflichtige VIN-Abfrage. Diese Operation liefert das Ergebnis der VINAbfrage und die Ersatzteileinformationen.

Parameter

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| locale | complexType, Locale | Landeinstellung, Datenland und Spracheinstellung |
| vin | String | Fahrzeugidentifikationsnummer |
| sparePartNo | String[] | Liste der Ersatzteilnummern, die zu ermitteln sind (max. 50 ETNs sind erlaubt). |
| finisNumber | Boolean | Steuerung, ob die FINIS-Ersatzteilenummer oder die Ford-Katalognummer in der Response zurückgegeben wird. |

Rückgabe

| Name | Datentyp | Beschreibung | Kind - Elemente |
| --- | --- | --- | --- |
| [sparePartsResultPerSparePartNumber](../datentypen/sparepartsresu-17205.md) | [SparePartsResultPerSparePartNumber](../datentypen/sparepartsresu-17205.md) [] | Ergebnisse der Ersatzteilnummer (ohne Fahrzeuginformationen) |  |
| Dossier | complexType, Dossier | Liste Fahrzeugidentifikation nach DAT im VXS-Format | [Country | Language | Vehicle]    Country (String3): Landeskürzel für den Zielmarkt  Language (String5): Sprachkennzeichen in ISO-Kodierung  [Vehicle](../../../vxs/aktenzeichenvorgange-doss/fahrzeug-vehic-6692.md) ([Vehicle](../../../vxs/aktenzeichenvorgange-doss/fahrzeug-vehic-6692.md)): Fahrzeugdaten |
