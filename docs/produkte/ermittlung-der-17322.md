---
title: "Ermittlung der Fahrzeuginformationen, Ersatzteilnummern, Verbauungsbedingungen und/oder Preishistorie"
topic_id: "17322"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > Ermittlung der Fahrzeuginformationen, Ersatzteilnummern, Verbauungsbedingungen und/oder Preishistorie"
---

# Ermittlung der Fahrzeuginformationen, Ersatzteilnummern, Verbauungsbedingungen und/oder Preishistorie

Die Funktion getSparePartsDetailsForDPN() ermöglicht die Ermittlung der Fahrzeuginformationen (Untertyp und Ausstattungen),
Ersatzteilnummern, Verbauungsbedingungen und/oder Preishistorie anhand von Fahrzeugart,
Hersteller, Haupttyp und DVNs. Um die Liste der Ergebnisse einzuschränken, werden
Parameter wie withPriceHistory, withVehicleData, pageSize und pageNumber bereitgestellt. Das SortingCriterions Objekt dient der Sortierung der Ergebnismenge.

Parameter

| Name | Datentyp | Beschreibung | Kind - Elemente |
| --- | --- | --- | --- |
| locale | complexType, Locale | Landeinstellung, Datenland und Spracheinstellung |  |
| restriction | complexType, SparePartsRestrictionForETN | Für die Abfrage benötigte Daten zu Fahrzeug und Ersatzteilen | [datProcessNo | vehicleType | manufacturer | baseModel | subModel | constructionTime | equipment | manufacturerCode | vin]    datProcessNo(Long[]): Liste der DVNs, die zu ermitteln sind (max. 50 DVNs sind erlaubt)  vehicleType (Integer, Pflichtparameter): Fahrzeugart  manufacturer (Integer, Pflichtparameter): Hersteller  baseModel (Integer, Pflichtparameter): Haupttyp  subModel (Integer, optional): Untertyp  constructionTime (Integer, optional): Bauzeit in DAT-Verschlüsselung  equipment (Long[], optional): Ausstattung  manufacturerCode (String[], optional): Herstellercodes  vin (String, optional): Fahrzeugidentifikationsnummer |
| settings | complexType, optional, SparePartsSettings | Parameter für die Anpassung der Datenausgabemenge | [pageNumber | pageSize | withPriceHistory | withVehicleData | sortingCriterions | finisNumber]    pageNumber (Integer, optional): Seitennummer der Ergebnisliste (Offset)  pageSize (Integer, optional): Anzahl der Ergebnisse pro Seite (Der maximale Wert ist 100)  withPriceHistory (Boolean, optional): Auflistung der Preishistorie  withVehicleData (Boolean, optional): Auflistung der Fahrzeuge, an dem das Teil verbaut werden kann.  [sortingCriterions](#showid/17188 "SparePartsSortingCriterions") (complexType, [SparePartsSortingcriterions](#showid/17188 "SparePartsSortingCriterions"), optional): Sortierung der Ergebnisliste  finisNumber (Boolean, optional): Steuerung, ob die FINIS-Ersatzteilenummer oder die Ford-Katalognummer in der Response zurückgegeben wird. |

Rückgabe

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| [sparePartsResultPerDPN](#showid/17219 "SparePartsResultPerDPN") | [SparePartsResultPerDPN[]](#showid/17219 "SparePartsResultPerDPN") | Ergebnisse der DAT-interne Datenverarbeitungsnummer (DVN) |
