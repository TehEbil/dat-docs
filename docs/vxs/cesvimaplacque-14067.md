---
title: "CesvimapLacquerFactor"
topic_id: "14067"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > ProcedureRelatedParameters > ProcedureRelatedParameter > CesvimapLacquerFactor"
---

# CesvimapLacquerFactor

Lackfaktoren Cesvimap

|  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- |
| factor | attribute | Beschreibung | type | mode | Mögliche Werte |
| CesvimapLacquerFactor | calculationType | Lack Kalkulationsmodus | LacquerCalculationMode |  | WAGE\_MATERIAL\_SEPARATELY = Lacklohn exkl. Lackmaterial WAGE\_INCLUSIVE\_MATERIAL = Lacklohn inkl. Lackmaterial |
| CesvimapLacquerFactor | isCalculationWithoutConstant | Berechnung ohne Konstanten | Boolean |  | true/false |
| CesvimapLacquerFactor | wage | Lacklohn | Price | PER\_HOUR /PER\_TIME\_SYSTEM |  |
| CesvimapLacquerFactor | wageMode | Lacklohn Modus | LacquerWageMode |  | PER\_TIME = Lacklohn (EUR/Stunde oder UT) \* |
| CesvimapLacquerFactor | materialMode | Lackmaterial Modus | LacquerMaterialMode |  | LACQUER\_METHOD = Nach Cesvimap Vorgabe |
| CesvimapLacquerFactor | type | Lackart | String |  | LACQUERID |
| CesvimapLacquerFactor | isScratchResistant | Kratzfeste Klarlacke | Boolean |  | true/false |
| CesvimapLacquerFactor | isDiscountCombined | Kombirabatt auf Lackieren | Boolean |  | true/false |
| CesvimapLacquerFactor | discountWageInclMaterial | Rabatt Lohn und Material | Discount | ABSOLUTE/PERCENT | % [0 bis 100,00] |
| CesvimapLacquerFactor | isDiscountSparePart | Rabatt Ersatzteile | Boolean |  | true/false |
| CesvimapLacquerFactor | discountMaterial | Rabatt Material \* | Discount | ABSOLUTE/PERCENT | % [0 bis 100,00] |
| CesvimapLacquerFactor | discountWage | Rabatt Lohn \* | Discount | ABSOLUTE/PERCENT | % [0 bis 100,00] |
