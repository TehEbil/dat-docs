---
title: "ProcedureRelatedParameter"
topic_id: "14059"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > ProcedureRelatedParameters > ProcedureRelatedParameter"
---

# ProcedureRelatedParameter

ProcedureRelatedParameters fungiert als parentNode und kann mit beliebig vielen ProcedureRelatedParameter bestückt werden. Die Struktur des ProcedureRelatedParameter Objektes ist immer gleich und hat eine Vielzahl an Attributen.

| Element | Typ | Beschreibung | Wertebereich |
| --- | --- | --- | --- |
| <ProcedureRelatedParameter> | complexType,  optional |  |  |
| attribute | attribute: definiert die Art/Bedeutung des Kalkulationsparameters |  |
| factor | factor: definiert welche Faktorart angesprochen wird | [CalculationFactor: Allgemeine Kalkulationsfaktoren](#showid/14061 "CalculationFactor")  [SparePartFactor: Ersatzteilfaktoren](#showid/14062 "SparePartFactor")  [LabourCostFactor: Arbeitslohnfaktoren](#showid/14063 "LabourCostFactor")  [EuroLacquerFactor: Lackfaktoren Eurolack](#showid/14064 "EuroLacquerFactor")  [ManufacturerLacquerFactor: Lackfaktoren Herstellersystem](#showid/14060 "ManufacturerLacquerFactor")  [AztLacquerFactor: Lackfaktoren AZT](#showid/14065 "AztLacquerFactor")  [CzLacquerFactor: Lackfaktoren Centro Zaragoza](#showid/14066 "CzLacquerFactor")  [CesvimapLacquerFactor: Lackfaktoren Cesvimap](#showid/14067 "CesvimapLacquerFactor")  [FullyManualLacquerFactor: Lackfaktoren Manuell](#showid/14068 "FullyManualLacquerFactor")  [DamageSegmentationFactor](#showid/22902 "DamageSegmentationFactor"): Schadensteilungfaktoren |
| mode | mode: steuert die Eigenschaften des Parameters | ABSOLUTE  PERCENT  PER\_HOUR  PER\_TIME\_SYSTEM |
| type | type: definiert den Typ des Parameters | BiwOptimizationMode  Boolean  Double  Date  Discount  Integer  lacquerMethod  Price  smallSparePartCalculationModel  String  TimeUnitSystem  LacquerCalculationMode  LacquerMaterialMode  LacquerWageMode  AztLacquerMode  List  OpelStandardRate |
| description | description: ist die Beschreibung | bspw. Mineraleffekt (2-Schicht) |

Der folgenden Parameter außerhalb der "Vorgangsbezogenen Daten" Maske wie PhantomCalculation muss weiterhin unter [RepairParameters](#showid/1415 "RepairParameters ") wie folgt gesetzt werden:

```
<vxs:RepairParameters>
                        <vxs:PhantomCalculation>false</vxs:PhantomCalculation>
</vxs:RepairParameters>
```
