---
title: "ManufacturerLacquerFactor"
topic_id: "14060"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > ProcedureRelatedParameters > ProcedureRelatedParameter > ManufacturerLacquerFactor"
---

# ManufacturerLacquerFactor

Lackfaktoren Herstellersystem

| factor | attribute | Beschreibung | type | mode | description | Mögliche Werte |
| --- | --- | --- | --- | --- | --- | --- |
| ManufacturerLacquerFactor | type | Lackart \* | String |  | bspw. Mineraleffekt (2-Schicht) | LACQUERID |
| ManufacturerLacquerFactor | colorName | Farbbezeichnung | String |  |  |  |
| ManufacturerLacquerFactor | colorCode | Farbcode | String |  |  |  |
| ManufacturerLacquerFactor | calculationType | Kalkulationstyp | LacquerCalculationMode |  |  | WAGE\_MATERIAL\_SEPARATELY = Lacklohn exkl. Lackmaterial WAGE\_INCLUSIVE\_MATERIAL = Lacklohn inkl. Lackmaterial |
| ManufacturerLacquerFactor | addition | Farbtonangleich - Musterblech | List |  |  | B |
| ManufacturerLacquerFactor | exemplarySheets | Anzahl Musterbleche \* | Integer |  |  |  |
|  |  |  |  |  |  |  |
|  | Lacklohn |  |  |  |  |  |
| ManufacturerLacquerFactor | wage | Lacklohn(EUR) \* | Price | PER\_HOUR / PER\_TIME\_SYSTEM |  |  |
| ManufacturerLacquerFactor | wageMode | Lacklohn Modus | LacquerWageMode |  |  | PER\_TIME = Lohn (EUR/Stunde, AW, ZE, oder AE) \*  ABSOLUTE = Pauschaler Lohn (EUR) |
| ManufacturerLacquerFactor | timeUnit | Zeitmaß | TimeUnitSystem |  |  | HOUR / AW / ZE / AE |
| ManufacturerLacquerFactor | timeUnitsPerHour | Zeitmaß per STD | Integer |  |  |  |
| ManufacturerLacquerFactor | wageFlatRate | Pauschaler Lohn (EUR) \* | Price | ABSOLUTE |  |  |
| ManufacturerLacquerFactor | discountWage | Rabatt | Discount | ABSOLUTE/PERCENT |  | PERCENT [0 bis 100,00] |
|  |  |  |  |  |  |  |
|  | Lackmaterial |  |  |  |  |  |
| ManufacturerLacquerFactor | materialPricePerTime | Lackmaterial für das Datenland Frankreich (EUR) | Double | PER\_HOUR /PER\_TIME\_SYSTEM |  |  |
| ManufacturerLacquerFactor | materialMode | Lackmaterial Modus | LacquerMaterialMode |  |  | LACQUER\_METHOD = Nach HST Vorgabe (EUR/QDM)  ABSOLUTE = Absolut (EUR)  PERCENT = Prozentual vom Lohn (%) |
| ManufacturerLacquerFactor | materialFlatRatePercent | Material prozentual vom Lohn (%) \* | Double |  |  |  |
| ManufacturerLacquerFactor | materialFlatRateAbsolute | Material Absolut (EUR) \* | Price | ABSOLUTE |  |  |
| ManufacturerLacquerFactor | discountMaterial | Rabatt Material | Discount | ABSOLUTE/PERCENT |  | PERCENT [0 bis 100,00] |
| ManufacturerLacquerFactor | discountMaterialBiw | Rabatt Material Optimierung auf RBK | Discount | ABSOLUTE/PERCENT |  | PERCENT [0 bis 100,00] |
|  |  |  |  |  |  |  |
|  | Lackmaterial - Mercedes - Benz |  |  |  |  |  |
| ManufacturerLacquerFactor | materialManufConstantPrice | Materialkonstante | Price | ABSOLUTE |  |  |
| ManufacturerLacquerFactor | materialManufSt1Price | ST.2 | Price | ABSOLUTE |  |  |
| ManufacturerLacquerFactor | materialManufSt2Price | ST.3 | Price | ABSOLUTE |  |  |
| ManufacturerLacquerFactor | materialManufSt3Price | ST.1-M | Price | ABSOLUTE |  |  |
| ManufacturerLacquerFactor | materialManufSt4Price | ST.1-E | Price | ABSOLUTE |  |  |
| ManufacturerLacquerFactor | materialManufSt5Price | ST.1-J | Price | ABSOLUTE |  |  |
|  |  |  |  |  |  |  |
|  | Lackmaterial - BMW |  |  |  |  |  |
| ManufacturerLacquerFactor | materialManufSurfacePercent | Flächenabhängige Variable (%) | Double |  |  |  |
| ManufacturerLacquerFactor | materialManufSt1Price | ST.1 | Price | ABSOLUTE |  |  |
| ManufacturerLacquerFactor | materialManufSt2Price | ST.3 | Price | ABSOLUTE |  |  |
| ManufacturerLacquerFactor | materialManufSt3Price | ST.2 | Price | ABSOLUTE |  |  |
|  |  |  |  |  |  |  |
|  | Lackmaterial - VW Gruppe |  |  |  |  |  |
| ManufacturerLacquerFactor | materialManufSt1Price | 1-Schicht | Price | ABSOLUTE |  |  |
| ManufacturerLacquerFactor | materialManufSt2Price | 2-Schicht | Price | ABSOLUTE |  |  |
| ManufacturerLacquerFactor | materialManufSt3Price | 3-Schicht | Price | ABSOLUTE |  |  |
|  |  |  |  |  |  |  |
|  | Lackmaterial - OPEL |  |  |  |  |  |
| ManufacturerLacquerFactor | materialOpelManufStxPrice | Materialpreis für Garantie-und Kulanzanträge | Price | PER\_TIME\_SYSTEM |  |  |
| ManufacturerLacquerFactor | materialMode | Materialmodus für Garantie-und Kulanzanträge | LacquerMaterialMode |  |  | GUARANTEE\_GOODWILL\_SYSTEM |
| ManufacturerLacquerFactor | materialOpelStandardRate |  | OpelStandardRate |  |  | ST2\_RULE1 / ST2\_RULE2 |
| ManufacturerLacquerFactor | materialManufSt1Price | 1-Schicht | Price | ABSOLUTE |  |  |
| ManufacturerLacquerFactor | materialManufSt2Price | 2-Schicht | Price | ABSOLUTE |  |  |
| ManufacturerLacquerFactor | materialManufSt3Price | 3-Schicht | Price | ABSOLUTE |  |  |
|  |  |  |  |  |  |  |
|  | Lackmaterial - FORD |  |  |  |  |  |
| ManufacturerLacquerFactor | materialManufSt1Price | 1-Schicht | Price | ABSOLUTE |  |  |
| ManufacturerLacquerFactor | materialManufSt2Price | 2-Schicht | Price | ABSOLUTE |  |  |
| ManufacturerLacquerFactor | materialManufSt3Price | 3-Schicht | Price | ABSOLUTE |  |  |
|  |  |  |  |  |  |  |
|  | Lack inkl. Material |  |  |  |  |  |
| ManufacturerLacquerFactor | wageInclMaterialMode | Lacklohn inkl. Material Modus | LacquerWageMode |  |  | PER\_TIME = Lohn inkl. Material (EUR/Stunde, AW, ZE oder AE) \*  ABSOLUTE = Pauschaler Lohn (EUR) |
| ManufacturerLacquerFactor | wageInclMaterial | Lacklohn inkl. Material | Price | PER\_HOUR /PER\_TIME\_SYSTEM |  |  |
| ManufacturerLacquerFactor | wageInclMaterialFlatRate | Pauschale Vorgabe (EUR) \* | Price | ABSOLUTE |  |  |
| ManufacturerLacquerFactor | discountWageInclMaterial | Rabatt | Discount | ABSOLUTE/PERCENT |  | PERCENT [0 bis 100,00] |
| ManufacturerLacquerFactor | discountWageInclMaterialBiw | Rabatt (Lohn ink. Material) Optimierung auf RBK | Discount | ABSOLUTE/PERCENT |  | PERCENT [0 bis 100,00] |
|  |  |  |  |  |  |  |
|  | Zusätzliche Aufschläge / Abschläge |  |  |  |  |  |
| ManufacturerLacquerFactor | newForOld | Pauschaler Neu für Alt Abzug auf die gesamte Lackierung | Discount | ABSOLUTE/PERCENT |  | PERCENT [0 bis 100,00] |
| ManufacturerLacquerFactor | preparationTimePercent | Vorbereitungszeit Blech (%) | Double |  |  | PERCENT [0 bis 100,00] |
| ManufacturerLacquerFactor | surchargeIncreaseWorkarea | Zusatz-Vorbereitungszeit für die Hersteller VW und Audi | Boolean |  |  | true/false |
| ManufacturerLacquerFactor | isLacquerAssemblyWhenRemoved | Montageteile ausgebaut lackieren | Boolean |  |  | true/false |
| ManufacturerLacquerFactor | isSurchargeForSecondColor | Zuschlag für 2. Farbe | Boolean |  |  | true/false |
| ManufacturerLacquerFactor | isSurchargeForMatt | Zuschlag für Mattlackierung für Audi und Volkswagen | Boolean |  |  | true/false |
| ManufacturerLacquerFactor | isSurchargeForMattSettlingColor | Angabe, ob ein Zuschlag für die Mattlackierung (Absetzfarbe) berücksichtigt wird. Bitte beachten Sie, dass der Parameter nur für die Hersteller Volkswagen und Audi vorgesehen sind. | Boolean |  |  | true/false |
