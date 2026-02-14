---
title: "CzLacquerFactor"
topic_id: "14066"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > ProcedureRelatedParameters > ProcedureRelatedParameter > CzLacquerFactor"
---

# CzLacquerFactor

Lackfaktoren Centro Zaragoza

|  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- |
| factor | attribute | Beschreibung | type | mode | Mögliche Werte |
| CzLacquerFactor | calculationType | Lack Kalkulationsmodus | LacquerCalculationMode |  | WAGE\_MATERIAL\_SEPARATELY = Lacklohn exkl. Lackmaterial WAGE\_INCLUSIVE\_MATERIAL = Lacklohn inkl. Lackmaterial |
| CzLacquerFactor | isCalculationWithoutConstant | Berechnung ohne Konstanten | Boolean |  | true/false |
| CzLacquerFactor | type | Lackart | String |  | LACQUERID |
| CzLacquerFactor | wage | Lacklohn | Price | PER\_HOUR /PER\_TIME\_SYSTEM |  |
| CzLacquerFactor | wageMode | Lacklohn Modus | LacquerWageMode |  | PER\_TIME = Lacklohn (EUR/Stunde oder UT) \* |
| CzLacquerFactor | materialMode | Lackmaterial Modus | LacquerMaterialMode |  | LACQUER\_METHOD = Nach Cz Vorgabe |
| CzLacquerFactor | isMultiColoured | Fahrzeug mehrfarbig | Boolean |  | true/false |
| CzLacquerFactor | colourCount | Anzahl Farben | Integer |  | [2 bis 9] |
| CzLacquerFactor | isDiscountCombined | Kombirabatt auf Lackieren | Boolean |  | true/false |
| CzLacquerFactor | discountWageInclMaterial | Rabatt Lohn und Material | Discount | ABSOLUTE/PERCENT | % [0 bis 100,00] |
| CzLacquerFactor | isDiscountSparePart | Rabatt Ersatzteile | Boolean |  | true/false |
| CzLacquerFactor | discountMaterial | Rabatt Material \* | Discount | ABSOLUTE/PERCENT | % [0 bis 100,00] |
| CzLacquerFactor | discountWage | Rabatt Lohn \* | Discount | ABSOLUTE/PERCENT | % [0 bis 100,00] |
