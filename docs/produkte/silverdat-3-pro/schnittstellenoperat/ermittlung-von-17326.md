---
title: "Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, Ersatzteilnummer und Preishistorie"
topic_id: "17326"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, Ersatzteilnummer und Preishistorie"
---

# Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, Ersatzteilnummer und Preishistorie

Die Funktion getSparePartsDetailsForDPNByVIN() ermöglicht die Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, Ersatzteilnummer und Preishistorie anhand von Fahrzeugidentifikationsnummer
und DVNs. Hier erfolgt eine automatische kostenpflichtige VIN-Abfrage.

Diese Operation liefert das Ergebnis der VIN-Abfrage und die Ersatzteileinformationen für die abgefragten DVNs.

Parameter

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| locale | complexType, Locale | Landeinstellung, Datenland und Spracheinstellung |
| vin | String | Fahrzeugidentifikationsnummer |
| datProcessNo | Long[] | Liste der DVNs, die zu ermitteln sind (max. 50 DVNs sind erlaubt). |
| finisNumber | Boolean | Steuerung, ob die FINIS-Ersatzteilenummer oder die Ford-Katalognummer in der Response zurückgegeben wird. |

Rückgabe

| Name | Datentyp | Beschreibung | Kind - Elemente |
| --- | --- | --- | --- |
| [sparePartsResultPerDPN](../../silverdat-calculatepro-si/datentypen/sparepartsresu-17219.md) | [SparePartsResultPerDPN[]](../../silverdat-calculatepro-si/datentypen/sparepartsresu-17219.md) | Ergebnisse der DAT-interne Datenverarbeitungsnummer (DVN), ohne Fahrzeuginformationen |  |
| Dossier | complexType, Dossier | Liste Fahrzeugidentifikation nach DAT im VXS-Format | [Country | Language | Vehicle]    Country (String3): Landeskürzel für den Zielmarkt  Language (String5): Sprachkennzeichen in ISO-Kodierung  [Vehicle](../../../vxs/aktenzeichenvorgange-doss/fahrzeug-vehicle/index.md) ([Vehicle](../../../vxs/aktenzeichenvorgange-doss/fahrzeug-vehicle/index.md)): Fahrzeugdaten |
