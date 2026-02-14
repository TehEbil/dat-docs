---
title: "CalculationFactor"
topic_id: "14061"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > ProcedureRelatedParameters > ProcedureRelatedParameter > CalculationFactor"
---

# CalculationFactor

Allgemeine Kalkulationsfaktoren

| factor | attribute | Beschreibung | type | mode | Mögliche Werte |
| --- | --- | --- | --- | --- | --- |
| CalculationFactor | selectedLacquerMethod | Ausgewähltes Lack-System | LacquerMethod |  | MANUFACTURER\_SPECIFIC  EURO\_LACQUER  AZT  FULLY\_MANUAL |
| CalculationFactor | isGlassCalculation | Mit getrennter Glaskalkulation | Boolean |  | true/false |
| CalculationFactor | vatRate | Mehrwertsteuer | Double |  | % [0 bis 99.9] |
| CalculationFactor | isGlassCalculationWithoutWork | Glaskalkulation ohne Arbeit | Boolean |  | true/false |
| CalculationFactor | showLongWorkStrings | Anzeige langer Arbeitstexte | Boolean |  | true/false |
| CalculationFactor | showAllIncludedWork | Sämtliche umfasste Arbeiten ausgeben | Boolean |  | true/false |
| CalculationFactor | biwOptimizationMode | Optimierung auf Rohbaukarosserie | BiwOptimizationMode |  | SUPPRESS = unterdrücken  AUTOMATIC = Standard Schwellenwert  FORCE = Niedrigem Schwellenwert |
| CalculationFactor | preDamageTotal | Vorschaden (EUR) | Price | ABSOLUTE |  |
| CalculationFactor | discount | Rabatt | Discount | ABSOLUTE/PERCENT | % [0 bis 100,00] |
| CalculationFactor | newForOld | NFA | Discount | ABSOLUTE/PERCENT | % [0 bis 100,00] |
| CalculationFactor | dataCurrency | Währung | String |  | EUR |
| CalculationFactor | timeUnit | Zeitmaß | TimeUnitSystem |  | HOUR /AW/ZE/AE |
| CalculationFactor | timeUnitsPerHour | Zeitmaß per STD | Integer |  |  |
| CalculationFactor | appreciation | Steuerneutrale Wertverbesserung    Die Eingabe bzw. Übergabe ist ausschließlich in der SilverDAT calculateExpert erlaubt.  In der SilverDAT myClaim (SilverDAT 3 Pro Netz) und SilverDAT calculatePRO ist der Import einer steuerneutralen Wertverbesserung aus der SilverDAT calculateExpert möglich.  In diesem Fall fließt die Wertverbesserung ohne Auswirkung oder Ausweis der Mehrwertsteuer ein.  Das Überschreiben dieses Wertes ist nicht gestattet. | Price | NETTO/BRUTTO/TaxNeutral |  |
| CalculationFactor | withoutValuesOfAdditionallyRequiredPositions | Preis/Arbeitszeit bei zugesteuerten Positionen nicht berücksichtigen | Boolean |  | true/false |
| CalculationFactor | crossSeries | Serienübergreifende Kalkulation | CrossSeriesState |  | YES/NO |
| CalculationFactor | wasteDisposalCostsPercValue | Angabe für Müllentsorgungskosten in Prozent für das Datenland Italien | Decimal | PERCENT |  |
| CalculationFactor | wasteDisposalCostsMaxValue | Angabe für den maximalen Wert der Müllentsorgungskosten in Euro für das Datenland Italien | Price | ABSOLUTE |  |
