---
title: "RepairCalculation"
topic_id: "1407"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation"
---

# RepairCalculation

Das Element <RepairCalculation> enthält die Kalkulationsergebnisse sowie alle Daten die zur Kalkulation benötigt
werden. Es befindet sich direkt unter dem [Dossier](../aktenzeichenvorgang/index.md) Element.

Die Kalkulationsergebnisse werden als in ein CalcResult Elemente abgelegt. Das CalcResultToUse gibt jeweils an welches Ergebnis gültig ist.

Felder:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| [Vehicle](../fahrzeug-vehicle/index.md) | [Vehicle](../fahrzeug-vehicle/index.md) | Das für die Kalkulation verwendete Fahrzeug.  Es ist eine Referenz auf das Vehicle Element im [Dossier](../aktenzeichenvorgang/index.md) daher muss es beim Import entweder null oder mit dem Vehicle im [Dossier](../aktenzeichenvorgang/index.md) identisch sein. |
| RepairWages | RepairWages | Lohnsätze |
| [RepairParameters](repairparamete-1415.md) | [RepairParameters](repairparamete-1415.md) | Kalkulationsparameter (alt) |
| [ProcedureRelatedParameters](procedurerelat-14058.md) | [ProcedureRelatedParameters](procedurerelat-14058.md) | Kalkulationsparameter (neu) |
| [RepairPositions](repairposition-1417.md) | [RepairPositions](repairposition-1417.md) | Enthält eine Liste mit Reparaturpositionen |
| CalcResultToUse | String | Beschreibt, welche Kalkulation verwendet wird. Das gilt für die folgenden Typen:  "common", "optimized", "glass", "italyCommon", "italyOptimized", "italyGlass","SPO","EXTERNAL", "DAT" |
| [CalcResultCommon](kalkulationser-1409.md) | [CalcResult](kalkulationser-1409.md) | Standardkalkulation  "common" --> VehicleRepairOnline  "DAT" -->myClaim  "EXTERNAL" --> eigene Kalkulation nur für myClaim |
| [CalcResultExtension](kalkulationser-16426.md) | [CalcResult](kalkulationser-1409.md) | Reparaturkostenausweitungs-Kalkulation |
| [CalcResultGlass](kalkulationser-1409.md) | [CalcResult](kalkulationser-1409.md) | Glaskalkulation  "glass" |
| [CalcResultOptimized](kalkulationser-1409.md) | [CalcResult](kalkulationser-1409.md) | Optimierte Kalkulation Rohbaukarosserie  "optimized" |
| CalcResultItaly | CalcResultItaly | Standardkalkulation (nur für Italien)  "italyCommon" |
| CalcResultItalyOptimized | CalcResultItaly | Optimierte Berechnung mit Rohbaukarosserie (nur für Italien)  "italyOptimized" |
| CalcResultItalyGlass | CalcResultItaly | Glaskalkulation (nur für Italien)  "italyGlass" |
| CalcResultDomus |  |  |
| CalcResultDomusOptimized |  |  |
| CalcResultDomusGlass |  |  |
| [CalcResultCustomerRanking](kalkulationser-1409.md) | [CalcResult](kalkulationser-1409.md) |  |
| [CalcResultMaintenance](kalkulationser-1409.md) | [CalcResult](kalkulationser-1409.md) | Wartungskalkulation  "maintenance" |
| CalcResultsHistory |  | Kalkulationshistorie |
| CalcResultSPO | [CalcResult](kalkulationser-1409.md) | Spare Parts Optimization Calculation Ersatzteiloptimierungskalkulation |
| DiscountPositions | DiscountPositions |  |
| CalculationSummary | [CalculationSummary](summe-reparatu-2919.md) |  |
| SurchargeSettings | SurchargeSettings |  |
| SettingsParameters | complexType, optional,  [SettingsParameters](settingsparame-16545.md) | Liste an Wertemengen, die folgende kalkulationsrelevante Einstellungen modelliert:  Ersatzteile-Einstellungen  Arbeit-Einstellungen  Lack-Einstellungen  Allgemeine Einstellungen |

- [arbeits-positi-2958](arbeits-positi-2958.md)
- [auftragsbezoge-2921](auftragsbezoge-2921.md)
- [ausstattungen-1379](ausstattungen-1379.md)
- [auxiliarycosts-15531](auxiliarycosts-15531.md)
- [aztlacquerfact-14065](aztlacquerfact-14065.md)
- [calculationfac-14061](calculationfac-14061.md)
- [calculationpro-16543](calculationpro-16543.md)
- [cesvimaplacque-14067](cesvimaplacque-14067.md)
- [czlacquerfacto-14066](czlacquerfacto-14066.md)
- [damagesegmenta-22902](damagesegmenta-22902.md)
- [damagesegmenta-22904](damagesegmenta-22904.md)
- [deductiblepart-18562](deductiblepart-18562.md)
- [deductionsposi-18561](deductionsposi-18561.md)
- [deductionssumm-15112](deductionssumm-15112.md)
- [dentpositionsp-16560](dentpositionsp-16560.md)
- [discountpositi-18557](discountpositi-18557.md)
- [discountpositi-18558](discountpositi-18558.md)
- [eurolacquerfac-14064](eurolacquerfac-14064.md)
- [fahrzeug-3696](fahrzeug-3696.md)
- [fullymanuallac-14068](fullymanuallac-14068.md)
- [iflmaterialdat-17427](iflmaterialdat-17427.md)
- [iflworkdata-17426](iflworkdata-17426.md)
- [inspectioncost-22886](inspectioncost-22886.md)
- [inspektion-pos-22883](inspektion-pos-22883.md)
- [kalkulationser-1409](kalkulationser-1409.md)
- [kalkulationser-16426](kalkulationser-16426.md)
- [labourcostfact-14063](labourcostfact-14063.md)
- [labourcostssum-15107](labourcostssum-15107.md)
- [lack-positione-2908](lack-positione-2908.md)
- [lacquerconstan-16547](lacquerconstan-16547.md)
- [lacquercostssu-15481](lacquercostssu-15481.md)
- [lacquermateria-15519](lacquermateria-15519.md)
- [manufacturerla-14060](manufacturerla-14060.md)
- [material-posit-1465](material-posit-1465.md)
- [mtplwearrus-16506](mtplwearrus-16506.md)
- [nebenkosten-po-2906](nebenkosten-po-2906.md)
- [parkingdentpos-15552](parkingdentpos-15552.md)
- [parkingdentpos-15553](parkingdentpos-15553.md)
- [positionswithm-16562](positionswithm-16562.md)
- [pricecorrectio-16564](pricecorrectio-16564.md)
- [procedurerelat-14058](procedurerelat-14058.md)
- [procedurerelat-14059](procedurerelat-14059.md)
- [protocolentrie-16556](protocolentrie-16556.md)
- [protocolentrie-16558](protocolentrie-16558.md)
- [protocolhints-16549](protocolhints-16549.md)
- [protocolhints-16566](protocolhints-16566.md)
- [protokolle-mat-2904](protokolle-mat-2904.md)
- [repairparamete-1415](repairparamete-1415.md)
- [repairposition-1417](repairposition-1417.md)
- [repairposition-1419](repairposition-1419.md)
- [reparaturauswe-16423](reparaturauswe-16423.md)
- [settingsparame-16545](settingsparame-16545.md)
- [settingsparame-16550](settingsparame-16550.md)
- [settingsparame-16551](settingsparame-16551.md)
- [settingsparame-16552](settingsparame-16552.md)
- [settingsparame-16553](settingsparame-16553.md)
- [settingsparame-16554](settingsparame-16554.md)
- [sparepartfacto-14062](sparepartfacto-14062.md)
- [sparepartscost-15105](sparepartscost-15105.md)
- [summe-reparatu-2919](summe-reparatu-2919.md)
- [surchargedisco-15560](surchargedisco-15560.md)
- [surchargesdisc-15556](surchargesdisc-15556.md)
- [surchargesdisc-15559](surchargesdisc-15559.md)
- [vxs-beispiel-14080](vxs-beispiel-14080.md)
- [weitere-repara-2960](weitere-repara-2960.md)
- [work-22593](work-22593.md)
