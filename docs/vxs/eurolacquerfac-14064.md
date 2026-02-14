---
title: "EuroLacquerFactor"
topic_id: "14064"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > ProcedureRelatedParameters > ProcedureRelatedParameter > EuroLacquerFactor"
---

# EuroLacquerFactor

Lackfaktoren Eurolack

|  |  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- | --- |
| factor | attribute | Beschreibung | type | mode | description | Mögliche Werte |
| EuroLacquerFactor | type | Lackart \* | String |  | bspw. Mineraleffekt (2-Schicht) | LACQUERID |
| EuroLacquerFactor | colorName | Farbbezeichnung | String |  |  |  |
| EuroLacquerFactor | colorCode | Farbcode | String |  |  |  |
| EuroLacquerFactor | addition | Farbtonangleich - Mischanlage | List |  |  | A |
| EuroLacquerFactor | addition | Farbtonangleich - Musterblech | List |  |  | B |
| EuroLacquerFactor | exemplarySheets | Anzahl Musterbleche \* | Integer |  |  |  |
|  |  |  |  |  |  |  |
|  | Lacklohn |  |  |  |  |  |
| EuroLacquerFactor | calculationType | Lack Kalkulationsmodus | LacquerCalculationMode |  |  | WAGE\_MATERIAL\_SEPARATELY = Lacklohn exkl. Lackmaterial WAGE\_INCLUSIVE\_MATERIAL = Lacklohn inkl. Lackmaterial |
| EuroLacquerFactor | wageMode | Lacklohn Modus | LacquerWageMode |  |  | PER\_TIME = Lohn (EUR/Stunde, AW, ZE, oder AE) \*  ABSOLUTE = Pauschaler Lohn (EUR) |
| EuroLacquerFactor | wage | Lacklohn (EUR/Stunde) \* | Price | PER\_HOUR /PER\_TIME\_SYSTEM |  |  |
| EuroLacquerFactor | wageFlatRate | Pauschaler Lacklohn (EUR) | Price | ABSOLUTE |  |  |
| EuroLacquerFactor | discountWage | Lacklohn - Rabatte | Discount | ABSOLUTE/PERCENT |  | % [0 bis 100,00] |
| EuroLacquerFactor | timeUnit | Zeitmaß | TimeUnitSystem |  |  | HOUR / AW / ZE / AE |
| EuroLacquerFactor | timeUnitsPerHour | Zeitmaß per STD | Integer |  |  |  |
|  |  |  |  |  |  |  |
|  | Lackmaterial |  |  |  |  |  |
| EuroLacquerFactor | materialPricePerTime | Lackmaterial für das Datenland Frankreich (EUR) | Double | PER\_HOUR /PER\_TIME\_SYSTEM |  |  |
| EuroLacquerFactor | materialMode | Lackmaterial Modus | LacquerMaterialMode |  |  | LACQUER\_METHOD  = Nach EURO Vorgabe  ABSOLUTE = Absolut (EUR)  PERCENT = Prozentual vom Lohn (%) |
| EuroLacquerFactor | materialPerPointCost | Materialkosten pro Materialpunkt | Price | ABSOLUTE |  |  |
| EuroLacquerFactor | materialIndex | Materialindex (%) \* | Double |  |  | % [50 bis 999,00] |
| EuroLacquerFactor | materialFlatRatePercent | Pauschale vom Lohn (%) \* | Double |  |  | % [-9999,99 bis 9999,99] |
| EuroLacquerFactor | materialFlatRateAbsolute | Pauschale Vorgabe (EUR) \* | Price | ABSOLUTE |  |  |
| EuroLacquerFactor | materialSpecialLacquer | Zuschlag Spezial-Lack (EUR) | Price | ABSOLUTE |  |  |
| EuroLacquerFactor | discountMaterial | Lackmaterial - Rabatte | Discount | ABSOLUTE/PERCENT |  | % [0 bis 100,00] |
| EuroLacquerFactor | materialPriceCategory | ID der Materialpreiskategorie nur für die Datenländer Polen und Tschechien | Integer |  |  |  |
| EuroLacquerFactor | materialPriceCategoryName | Name der Materialpreiskategorie, nur für die Datenländer Polen und Tschechien bspw. PM - Eurolack Premium [rodz. poj. 01, 02, 03] | String |  |  |  |
| EuroLacquerFactor | materialIndexPreparation | Prozentuale Angabe des Materialindexes für die Vorbereitung. Bitte beachten Sie, dass dieser Parameter nur in Verbindung mit dem gesamten Materialindex (<materialIndex>) angegeben werden kann. | Double |  |  |  |
| EuroLacquerFactor | materialIndexComponents | Prozentuale Angabe des Materialindexes für die Bauteile. Bitte beachten Sie, dass dieser Parameter nur in Verbindung mit dem gesamten Materialindex (<materialIndex>) angegeben werden kann. | Double |  |  |  |
| EuroLacquerFactor | isSurchargeForMatt | Angabe, ob ein Zuschlag für die Mattlackierung (Absetzfarbe) berücksichtigt wird. | Boolean |  |  |  |
| EuroLacquerFactor | isSurchargeForMattSmallParts | Angabe, ob ein Zuschlag für die Mattlackierung (Absetzfarbe) von Kleinteilen berücksichtigt wird. | Boolean |  |  |  |
|  |  |  |  |  |  |  |
|  | Lack inkl. Material |  |  |  |  |  |
| EuroLacquerFactor | wageInclMaterialMode | Lacklohn inkl. Material Modus | LacquerWageMode |  |  | PER\_TIME = Lohn inkl. Material (EUR/Stunde, AW, ZE oder AE) \*  ABSOLUTE = Pauschaler Lohn (EUR) |
| EuroLacquerFactor | wageInclMaterial | Lacklohn inkl. Material | Price | PER\_HOUR /PER\_TIME\_SYSTEM |  |  |
| EuroLacquerFactor | wageInclMaterialFlatRate | Pauschale Vorgabe (EUR) \* | Price | ABSOLUTE |  |  |
| EuroLacquerFactor | discountWageInclMaterial | Lacklohn inkl. Material - Rabatte | Discount | ABSOLUTE/PERCENT |  | % [0 bis 100,00] |
|  |  |  |  |  |  |  |
|  | Zusätzliche Aufschläge / Abschläge |  |  |  |  |  |
| EuroLacquerFactor | newForOld | Pauschaler Neu für Alt Abzug auf die gesamte Lackierung | Discount | ABSOLUTE/PERCENT |  | % [0 bis 100,00] |
| EuroLacquerFactor | preparationTimePercent | Vorbereitungszeit Blech (%) | Double |  |  | % [0 bis 100] |
| EuroLacquerFactor | preparationTimePlasticPercent | Vorbereitungszeit Kunststoff (%) | Double |  |  | % [0 bis 100] |
| EuroLacquerFactor | isReducedPreparationTime | Vorbereitung Einzelauftrag/Kleinteile | Boolean |  |  | true/false |
| EuroLacquerFactor | isFrameworkUse | Einsatz Gerüst | Boolean |  |  | true/false |
| EuroLacquerFactor | isSurchargeForSecondColor | Zuschlag für 2. Farbe | Boolean |  |  | true/false |
| EuroLacquerFactor | isLacquerPlasticWhenFitted | Kunststoffteile eingebaut lackieren | Boolean |  |  | true/false |
| EuroLacquerFactor | isApplyUndercoatLacquerWhenRemoved | Am Fahrzeug mit vorlackieren | Boolean |  |  | true/false |
| EuroLacquerFactor | isLacquerAssemblyWhenRemoved | Montageteile ausgebaut lackieren | Boolean |  |  | true/false |
| EuroLacquerFactor | disposalCostPercent | Entsorgungskosten (%) | Double |  |  | % [0 bis 5,00] |
| EuroLacquerFactor | maskingWorkGlassCount | Abdeckarbeit geklebte Scheiben | Integer |  |  | [1 bis 9] |
| EuroLacquerFactor | maskingWorkPlasticCount | Abdeckarbeit ausgebaute Kunststoffteile | Integer |  |  | [1 bis 10] |
| EuroLacquerFactor | matBlackWindowFrameCount | Anzahl mattschwarze Fensterrahmen | Integer |  |  | [1 bis 4] |
| EuroLacquerFactor | otherPreparationTimePercent | Sonstige Vorbereitungszeit    Der Reparaturparameter „sonstige Vorbereitung" wirkt auf die Positionen:  - Farbmischen (Arbeitszeit)  - Farbmuster (Arbeitszeit)  - Zuschlag Wasserbasislack (Arbeitszeit)  Nur für das Datenland Schweiz.  - Teil(e) ausgebaut vorlackieren (Arbeitszeit)  - Konstante Musterblech (Material)  - Konstante 2. Farbe (Material)  - Konstante ausgebaut vorlackieren. | Double | PERCENT |  | Defaultwert 100%  {0% -100%} |
