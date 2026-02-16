---
title: "Ermittlung von Fahrzeuginformationen, DVN, Verbauungsbedingungen und/oder Preishistorie"
topic_id: "22533"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > PartsService > Ermittlung von Fahrzeuginformationen, DVN, Verbauungsbedingungen und/oder Preishistorie"
---

# Ermittlung von Fahrzeuginformationen, DVN, Verbauungsbedingungen und/oder Preishistorie

Die Funktion getSparePartsDetails() ermöglicht die Ermittlung von Fahrzeuginformationen (Untertyp und Ausstattungen),
DAT-interne Datenverarbeitungsnummer (DVN), Verbauungsbedingungen und/oder Preishistorie anhand von Fahrzeugart, Hersteller,
Haupttyp und Ersatzteilnummer (ETN). Um die Liste der Ergebnisse einzuschränken, werden Parameter wie withPriceHistory, withVehicleData, pageSize und pageNumber bereitgestellt. Das SortingCriterions Objekt dient der Sortierung der Ergebnismenge.

Parameter

| Name | Datentyp | Beschreibung | Kind - Elemente |
| --- | --- | --- | --- |
| locale | complexType, Locale | Landeinstellung, Datenland und Spracheinstellung |  |
| restriction | complexType, SparePartsRestrictionForETN | Für die Abfrage benötigte Daten zu Fahrzeug und Ersatzteilen | [sparePartNo | vehicleType | manufacturer | baseModel | subModel | constructionTime | equipment | manufacturerCode | vin]    sparePartNo (String[], Pflichtparameter): Liste der Ersatzteilnummern(max. 50 ETNs sind erlaubt)  vehicleType (Integer, Pflichtparameter): Fahrzeugart  manufacturer (Integer, Pflichtparameter): Hersteller  baseModel (Integer, optional): Haupttyp  subModel (Integer, optional): Untertyp  constructionTime (Integer, optional): Bauzeit in DAT-Verschlüsselung  equipment (Long[], optional): Ausstattung  manufacturerCode (String[], optional): Herstellercodes  vin (String, optional): Fahrzeugidentifikationsnummer |
| settings | complexType, optional, SparePartsSettings | Parameter für die Anpassung der Datenausgabemenge | [pageNumber | pageSize | withPriceHistory | withVehicleData | sortingCriterions | finisNumber]    pageNumber (Integer, optional): Seitennummer der Ergebnisliste (Offset)  pageSize (Integer, optional): Anzahl der Ergebnisse pro Seite (Der maximale Wert ist 100)  withPriceHistory (Boolean, optional): Auflistung der Preishistorie  withVehicleData (Boolean, optional): Auflistung der Fahrzeuge, an dem das Teil verbaut werden kann.  [sortingCriterions](../../silverdat-calculatepro-si/datentypen/sparepartssort-17188.md) (complexType, [SparePartsSortingcriterions](../../silverdat-calculatepro-si/datentypen/sparepartssort-17188.md), optional): Sortierung der Ergebnisliste  finisNumber (Boolean, optional): Steuerung, ob die FINIS-Ersatzteilenummer oder die Ford-Katalognummer in der Response zurückgegeben wird. |

Rückgabe

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| [sparePartsResultPerSparePartNumber](../../silverdat-calculatepro-si/datentypen/sparepartsresu-17205.md) | [SparePartsResultPerSparePartNumber](../../silverdat-calculatepro-si/datentypen/sparepartsresu-17205.md)[] | Enthält Ergebnisse über die Ersatzteilnummer |
