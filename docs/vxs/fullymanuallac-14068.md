---
title: "FullyManualLacquerFactor"
topic_id: "14068"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > ProcedureRelatedParameters > ProcedureRelatedParameter > FullyManualLacquerFactor"
---

# FullyManualLacquerFactor

Lackfaktoren Manuell

|  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- |
| factor | attribute | Beschreibung | type | mode | Mögliche Werte |
| FullyManualLacquerFactor | calculationType | Lack Kalkulationsmodus | LacquerCalculationMode |  | WAGE\_MATERIAL\_SEPARATELY = Lacklohn exkl. Lackmaterial WAGE\_INCLUSIVE\_MATERIAL = Lacklohn inkl. Lackmaterial |
| FullyManualLacquerFactor | isCalculationWithoutConstant | Berechnung ohne Konstanten | Boolean |  | true/false |
| FullyManualLacquerFactor | wage | Lacklohn | Price | PER\_HOUR /PER\_TIME\_SYSTEM |  |
| FullyManualLacquerFactor | wageMode | Lacklohn Modus | LacquerWageMode |  | PER\_TIME = Lacklohn (EUR/Stunde oder UT) \* |
| FullyManualLacquerFactor | materialMode | Lackmaterial Modus | LacquerMaterialMode |  | LACQUER\_METHOD = Nach FManual Vorgabe |
| FullyManualLacquerFactor | type | Lackart | String |  | LACQUERID |
| FullyManualLacquerFactor | isDiscountCombined | Kombirabatt auf Lackieren | Boolean |  | true/false |
| FullyManualLacquerFactor | discountWageInclMaterial | Rabatt Lohn und Material | Discount | ABSOLUTE/PERCENT | % [0 bis 100,00] |
| FullyManualLacquerFactor | isDiscountSparePart | Rabatt Ersatzteile | Boolean |  | true/false |
| FullyManualLacquerFactor | discountMaterial | Rabatt Material \* | Discount | ABSOLUTE/PERCENT | % [0 bis 100,00] |
| FullyManualLacquerFactor | discountWage | Rabatt Lohn \* | Discount | ABSOLUTE/PERCENT | % [0 bis 100,00] |
