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
| factor | factor: definiert welche Faktorart angesprochen wird | [CalculationFactor: Allgemeine Kalkulationsfaktoren](calculationfac-14061.md)  [SparePartFactor: Ersatzteilfaktoren](sparepartfacto-14062.md)  [LabourCostFactor: Arbeitslohnfaktoren](labourcostfact-14063.md)  [EuroLacquerFactor: Lackfaktoren Eurolack](eurolacquerfac-14064.md)  [ManufacturerLacquerFactor: Lackfaktoren Herstellersystem](manufacturerla-14060.md)  [AztLacquerFactor: Lackfaktoren AZT](aztlacquerfact-14065.md)  [CzLacquerFactor: Lackfaktoren Centro Zaragoza](czlacquerfacto-14066.md)  [CesvimapLacquerFactor: Lackfaktoren Cesvimap](cesvimaplacque-14067.md)  [FullyManualLacquerFactor: Lackfaktoren Manuell](fullymanuallac-14068.md)  [DamageSegmentationFactor](damagesegmenta-22902.md): Schadensteilungfaktoren |
| mode | mode: steuert die Eigenschaften des Parameters | ABSOLUTE  PERCENT  PER\_HOUR  PER\_TIME\_SYSTEM |
| type | type: definiert den Typ des Parameters | BiwOptimizationMode  Boolean  Double  Date  Discount  Integer  lacquerMethod  Price  smallSparePartCalculationModel  String  TimeUnitSystem  LacquerCalculationMode  LacquerMaterialMode  LacquerWageMode  AztLacquerMode  List  OpelStandardRate |
| description | description: ist die Beschreibung | bspw. Mineraleffekt (2-Schicht) |

Der folgenden Parameter außerhalb der "Vorgangsbezogenen Daten" Maske wie PhantomCalculation muss weiterhin unter [RepairParameters](repairparamete-1415.md) wie folgt gesetzt werden:

```
<vxs:RepairParameters>
                        <vxs:PhantomCalculation>false</vxs:PhantomCalculation>
</vxs:RepairParameters>
```
