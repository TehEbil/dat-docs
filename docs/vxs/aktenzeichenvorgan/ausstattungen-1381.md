---
title: "Ausstattungen (Equipment, …Equipment, EquipmentPosition)"
topic_id: "1381"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Fahrzeug (Vehicle) > Ausstattungen (Equipment, …Equipment, EquipmentPosition)"
---

# Ausstattungen (Equipment, …Equipment, EquipmentPosition)

<Equipment> ist ein Unter-Element von <Vehicle> und <UpperBody> und enthält Informationen zu den Ausstattungen. <Equipment> selbst enthält allgemeine Angaben wie z.B. Fahrzeugfarbe und Polsterung.

Die auswählbaren Ausstattungen befinden sich in mehreren <EquipmentPosition>-Elementen, die in verschiedenen <...Equipment>-Elementen unter <Equipment> zusammengefasst sind (z.B. <SeriesEquipment> für die Serienausstattung).

Elemente in Equipment:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| SpecialEditionPackage | String | Sondermodellpaket |
| (Dat)ColorType | String | Farbe |
| (Dat)Color | String | Farbe Fahrzeug (Freitext) |
| (Dat)ColorVariant | String | Farbvariante |
| (Dat)LacquerType | String | Lackart |
| (Dat)CushionTypeName | String | Art des Sitzbezugs (Freitext) |
| (Dat)CushionType | String | Art des Sitzbezugs (Auswahl) |
| (Dat)CushionColorType | String | Farbe des Sitzbezugs (Auswahl) |
| (Dat)CushionColor | String | Farbe des Sitzbezugs (Freitext) |
| (Dat)EquipmentValue | Decimal | Ausstattungswert |
| (Dat)EquipmentValueGross | Decimal | Ausstattungswert ink.l MwSt. |
| (Dat)OriginalEquipmentValue | Decimal | Ausstattungs-Neuwert |
| (Dat)OriginalEquipmentValueGross | Decimal | Ausstattungs-Neuwert inkl. MwSt. |
| EquipmentValueType | String |  |
| SpecialEditionPackageId | Integer | Nummer des Sondermodellpaketes |
| SpecialEditionPackageNameN | String | Name des Sondermodellpaketes |
| SpecialEditionPackageDetails1 | String | Details des Sondermodellpaketes Teil 1 |
| SpecialEditionPackageDetails2 | String | Details des Sondermodellpaketes Teil 2 |
| SeriesEquipment |  | Serienausstattung; s. EquipmentPosition |
| DeselectedSeriesEquipment |  | abgewählte Serienausstattung; s. EquipmentPosition |
| SpecialModelEquipment |  | Sondermodellpaket; s. EquipmentPosition |
| SpecialEquipment |  | Sonderausstattung; s. EquipmentPosition |
| FreeSpecialEquipment |  | kostenlose Sonderausstattung; s. EquipmentPosition |
| AdditionalEquipment |  | Zusatzausstattung; s. EquipmentPosition |
| FlatRateEquipment |  | Pauschalausstattung (Restwertprognose); s. EquipmentPosition |

Elemente für Ausstattungspositionen: (Gruppierung, Daten in EquipmentPosition-Elementen)

| Element | Beschreibung |
| --- | --- |
| SeriesEquipment | Serienausstattung |
| DeselectedSeriesEquipment | abgewählte Serienausstattung |
| FreeSpecialEquipment | kostenlose Sonderausstattung |
| SpecialEquipment | Sonderausstattung |
| AdditionalEquipment | Zusatzausstattung |
| FlatRateEquipment | Pauschalausstattung (Restwertprognose) |
| SpecialModelEquipment | Sondermodellpaket |
| DenialCaseEquipment | ausgesteuerte Ausstattungen |
| SeriesOrSpecialEquipment | Ausstattungen, die Serienausstattung oder Sonderausstattung sein können. Dieses Element wird nur in den Methoden getExistingEquipmentN und getPossibleEquipmentN verwendet! |

Attribute von EquipmentPosition:

| Attribut | Typ | Beschreibung |
| --- | --- | --- |
| origin | string | "dat" – wenn die Ausstattung von DAT stammt,  "vin" – wenn die Ausstattung über eine VIN-Abfrage eingebracht wurde |

Elemente in EquipmentPosition:

| Element | Typ | Beschreibung | Status |
| --- | --- | --- | --- |
| AddedByLogicCheck | fieldBoolean | true, falls die betreffende Ausstattungsposition durch Logikprüfungen hinzugefügt wurden; ansonsten false | Dieses Feld kann nur bei Calculate-Anwendungsfällen auf true stehen, denn nur dort kann es vorkommen, dass eine Ausstattung aufgrund der Logikprüfungen hinzukommt. |
| InstallDate | date | Einbaudatum |  |
| (Dat)AgeInMonths | integer | Zusatzausstattungen | noch nicht aktiv |
| Deselected | boolean | Zusatzausstattungen | Für die Anwendungen der Schadenskalkulation kann hiermit der Ausdruck einer Ausstattung unterdrückt werden. |
| DatEquipmentId | integer | Nummer der Ausstattungsvariante (auch für ausgesteuerte Ausstattungsvarianten) | Rückgabe in calculatePro und valuateFinance |
| DatEquipmentIdReason | integer | gibt die Ausstattungsvariante wieder, die die Aussteuerung verursacht | Rückgabe in calculatePro |
| DatEquipmentIdReason2 | integer | gibt die Ausstattungsvariante wieder, die die Aussteuerung verursacht | Rückgabe in calculatePro |
| ValuationControlType | string | Behandlung bei Bewertung; bei no valuation wird der Wert der Ausstattung nicht berücksichtigt. |  |
| Description | string | Beschreibung der Ausstattungsvariante | Rückgabe in calculatePro und valuateFinance |
| FootnoteType | string | Verwendung der Fußnote |  |
| (Dat)FootnotePerc | decimal | Auf-/Abwertung in Prozent |  |
| (Dat)DecreaseType | string | Restwert/Fußnote/manuell |  |
| OriginalPrice | decimal | Neuwert ohne MwSt. (DAT) |  |
| OriginalPriceUser | decimal | Neuwert ohne MwSt. (Benutzer) |  |
| OriginalPriceGross | decimal | Neuwert inkl. MwSt. (DAT) |  |
| OriginalPriceGrossUser | decimal | Neuwert inkl. MwSt. (Benutzer) |  |
| (Dat)ResidualValue | decimal | Restwert ohne MwSt. |  |
| (Dat)ResidualValueGross | decimal | Restwert inkl. MwSt. |  |
| Amount | integer | Menge |  |
| ManualEntry | boolean | Zusatzausstattungen | noch nicht aktiv |
| ManualAgeEntry | boolean | Zusatzausstattungen | noch nicht aktiv |
| EquipmentGroup | string | Ausstattungsvarianten-Gruppe |  |
| EquipmentType | string | Beziehung zu Glaskalkulation, Motor-AV |  |
| EquipmentClass | long | Klasse der Ausstattung |  |
| ContainedEquipmentPositions |  | s. EquipmentPosition; kann wiederum EquipmentPosition enthalten. |  |
| ConstructionTimeFrom | integer | Bauzeit, ab der die Fahrzeuginformationen gelten (für Kalkulationsprüfung) |  |
