---
title: "AztLacquerFactor"
topic_id: "14065"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > ProcedureRelatedParameters > ProcedureRelatedParameter > AztLacquerFactor"
---

# AztLacquerFactor

Lackfaktoren AZT

|  |  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- | --- |
| factor | attribute | Beschreibung | type | mode | description | Mögliche Werte |
| AztLacquerFactor | type | Lackart \* | String |  | bspw. Mineraleffekt (2-Schicht) | LACQUERID |
| AztLacquerFactor | colorName | Farbbezeichnung | String |  |  |  |
| AztLacquerFactor | colorCode | Farbcode | String |  |  |  |
| AztLacquerFactor | fourLayerLacquerMode | AZT 4-Schicht Lack Modus | AztLacquerMode |  |  | WET\_IN\_WET = Nass in nass  DRY\_AND\_SAND = 1 mal trocknen und schleifen 2 mal trocknen und schleifen DRY\_AND\_SAND\_2\_TIMES = 2 mal trocknen und schleifen |
| AztLacquerFactor | threeLayerLacquerMode | AZT 3-Schicht Lack Modus | AztLacquerMode |  |  | WET\_IN\_WET = Nass in nass  DRY\_AND\_SAND = Trocknen und schleifen |
| AztLacquerFactor | addition | Farbtonangleich - Mischanlage | List |  |  | A |
| AztLacquerFactor | addition | Farbtonangleich - Musterblech | List |  |  | B |
| AztLacquerFactor | exemplarySheets | Anzahl Musterbleche \* | Integer |  |  |  |
| AztLacquerFactor | colourMixCounter | Anzahl von Farbmischungen \* | Integer |  |  |  |
|  |  |  |  |  |  |  |
|  | Lacklohn |  |  |  |  |  |
| AztLacquerFactor | calculationType | Lack Kalkulationsmodus | LacquerCalculationMode |  |  | WAGE\_MATERIAL\_SEPARATELY = Lacklohn exkl. Lackmaterial  WAGE\_INCLUSIVE\_MATERIAL = Lacklohn inkl. Lackmaterial |
| AztLacquerFactor | wage | Lacklohn (EUR) | Price | PER\_HOUR /PER\_TIME\_SYSTEM |  |  |
| AztLacquerFactor | wageMode | Lacklohn Modus | LacquerWageMode |  |  | PER\_TIME = Lohn (EUR/Stunde, AW, ZE, oder AE) \*  ABSOLUTE = Pauschaler Lohn (EUR) |
| AztLacquerFactor | wageFlatRate | Pauschaler Lohn (EUR) | Price | ABSOLUTE |  |  |
| AztLacquerFactor | discountWage | Lacklohn - Rabatte | Discount | ABSOLUTE/PERCENT |  | PERCENT [0 bis 100,00] |
|  |  |  |  |  |  |  |
|  | Lackmaterial |  |  |  |  |  |
| AztLacquerFactor | materialPricePerTime | Lackmaterial für das Datenland Frankreich (EUR) | Double | PER\_HOUR /PER\_TIME\_SYSTEM |  |  |
| AztLacquerFactor | materialMode | Lackmaterial Modus | LacquerMaterialMode |  |  | LACQUER\_METHOD = Nach AZT Vorgabe  ABSOLUTE = Absolut (EUR)  PERCENT = Prozentual vom Lohn (%) |
| AztLacquerFactor | materialIndex | Materialindex (%) \* | Double |  |  | % [50 bis 999,00] |
| AztLacquerFactor | materialFlatRatePercent | Pauschale vom Lohn (%) \* | Double |  |  | % [-9999,99 bis 9999,99] |
| AztLacquerFactor | materialFlatRateAbsolute | Pauschale Vorgabe (EUR) \* | Price | ABSOLUTE |  |  |
| AztLacquerFactor | materialSpecialLacquer | Zuschlag Spezial-Lack (EUR) | Price | ABSOLUTE |  |  |
| AztLacquerFactor | discountMaterial | Rabatt Material | Discount | ABSOLUTE/PERCENT |  | PERCENT [0 bis 100,00] |
|  |  |  |  |  |  |  |
|  | Lack inkl. Material |  |  |  |  |  |
| AztLacquerFactor | wageInclMaterialMode | Lacklohn inkl. Material Modus | LacquerWageMode |  |  | PER\_TIME = Lohn inkl. Material (EUR/Stunde, AW, ZE oder AE) \*  ABSOLUTE = Pauschaler Lohn (EUR) |
| AztLacquerFactor | wageInclMaterial | Lacklohn inkl. Material | Price | PER\_HOUR /PER\_TIME\_SYSTEM |  |  |
| AztLacquerFactor | wageInclMaterialFlatRate | Pauschale Vorgabe (EUR) \* | Price | ABSOLUTE |  |  |
| AztLacquerFactor | discountWageInclMaterial | Lacklohn inkl. Material - Rabatt | Discount | ABSOLUTE/PERCENT |  | PERCENT [0 bis 100,00] |
|  |  |  |  |  |  |  |
|  | Zusätzliche Aufschläge / Abschläge |  |  |  |  |  |
| AztLacquerFactor | newForOld | Pauschaler Neu für Alt Abzug auf die gesamte Lackierung | Discount | ABSOLUTE/PERCENT |  | PERCENT [0 bis 100,00] |
| AztLacquerFactor | preparationTimePercent | Vorbereitungszeit Blech (%) | Double |  |  | PERCENT [0 bis 100,00] |
| AztLacquerFactor | preparationTimePlasticPercent | Vorbereitungszeit Kunststoff (%) | Double |  |  | PERCENT [0 bis 100,00] |
| AztLacquerFactor | isSurchargeForSecondColor | Zuschlag für 2. Farbe | Boolean |  |  | true/false |
| AztLacquerFactor | isLacquerPlasticWhenFitted | Kunststoffteile eingebaut lackieren | Boolean |  |  | true/false |
| AztLacquerFactor | isApplyUndercoatLacquerWhenRemoved | Am Fahrzeug mit vorlackieren | Boolean |  |  | true/false |
| AztLacquerFactor | isLacquerAssemblyWhenRemoved | Montageteile ausgebaut lackieren | Boolean |  |  | true/false |
| AztLacquerFactor | disposalCostPercent | Entsorgungskosten (%) | Double |  |  | PERCENT [0 bis 5,00] |
| AztLacquerFactor | maskingWorkPlasticCount | Abdeckarbeit ausgebaute Kunststoffteile | Integer |  |  | [1 bis 10] |
| AztLacquerFactor | matBlackWindowFrameCount | Anzahl mattschwarze Fensterrahmen | Integer |  |  | [1 bis 4] |
| AztLacquerFactor | otherPreparationTimePercent | Sonstige Vorbereitungszeit    Der Reparaturparameter „sonstige Vorbereitung" wirkt auf die Positionen:  - Farbmischen (Arbeitszeit)  - Farbmuster (Arbeitszeit)  - Zuschlag 2 Farben Lackierung (Arbeitszeit)  - Musterblech (Material)  - Zuschlag 2 Farbenlackierung (Material) | Double | PERCENT |  | Defaultwert 100%  {0% -100%} |
