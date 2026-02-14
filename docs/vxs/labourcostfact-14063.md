---
title: "LabourCostFactor"
topic_id: "14063"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > ProcedureRelatedParameters > ProcedureRelatedParameter > LabourCostFactor"
---

# LabourCostFactor

Arbeitslohnfaktoren

|  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- |
| factor | attribute | Beschreibung | type | mode | Mögliche Werte |
| LabourCostFactor | mechanicWage1 | Mechanik1 | Price | PER\_HOUR / PER\_TIME\_SYSTEM |  |
| LabourCostFactor | mechanicWage2 | Mechanik2 | Price | PER\_HOUR / PER\_TIME\_SYSTEM |  |
| LabourCostFactor | mechanicWage3 | Mechanik3 | Price | PER\_HOUR / PER\_TIME\_SYSTEM |  |
| LabourCostFactor | bodyWage1 | Karosserie1 | Price | PER\_HOUR / PER\_TIME\_SYSTEM |  |
| LabourCostFactor | bodyWage2 | Karosserie2 | Price | PER\_HOUR / PER\_TIME\_SYSTEM |  |
| LabourCostFactor | bodyWage3 | Karosserie3 | Price | PER\_HOUR / PER\_TIME\_SYSTEM |  |
| LabourCostFactor | electricWage1 | Elektrik1 | Price | PER\_HOUR / PER\_TIME\_SYSTEM |  |
| LabourCostFactor | electricWage2 | Elektrik2 | Price | PER\_HOUR / PER\_TIME\_SYSTEM |  |
| LabourCostFactor | electricWage3 | Elektrik3 | Price | PER\_HOUR / PER\_TIME\_SYSTEM |  |
| LabourCostFactor | dentWage | Dellen drücken | Price | PER\_HOUR / PER\_TIME\_SYSTEM |  |
| LabourCostFactor | dentsCountInProtocol | Dellenanzahl und Größe nur im Protokoll | Boolean |  | true/false |
| LabourCostFactor | discount | Rabatt | Discount | ABSOLUTE/PERCENT | % [0 bis 100,00] |
| LabourCostFactor | discountBiw | Rabatt Optimierung auf RBK | Discount | ABSOLUTE/PERCENT | % [0 bis 100,00] |
| LabourCostFactor | timeUnit | Zeitmaß | TimeUnitSystem |  | HOUR /AW/ZE/AE |
| LabourCostFactor | timeUnitsPerHour | Zeitmaß per STD | Integer |  |  |
| LabourCostFactor | labourLumpSum | Arbeitslohn pauschal (EUR) | Price | ABSOLUTE |  |
| LabourCostFactor | preparationAndSetupTimePercent | Vorbereitungs-/Rüstzeit (%), nur in Abhängigkeit vom ausgewählten Fahrzeug sichtbar. Nur bei den Herstellern Nissan (Pkw), Jaguar (Pkw), Mazda (Pkw), Land Rover (Pkw) und Nissan(Transporter) verfügbar. | Double | PERCENT | Defaultwert 100%  {0% -100%} |
