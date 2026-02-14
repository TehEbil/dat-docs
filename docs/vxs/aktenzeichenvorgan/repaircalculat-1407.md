---
title: "RepairCalculation"
topic_id: "1407"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation"
---

# RepairCalculation

Das Element <RepairCalculation> enthält die Kalkulationsergebnisse sowie alle Daten die zur Kalkulation benötigt
werden. Es befindet sich direkt unter dem [Dossier](aktenzeichenvo-1371.md) Element.

Die Kalkulationsergebnisse werden als in ein CalcResult Elemente abgelegt. Das CalcResultToUse gibt jeweils an welches Ergebnis gültig ist.

Felder:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| [Vehicle](fahrzeug-vehic-6692.md) | [Vehicle](fahrzeug-vehic-6692.md) | Das für die Kalkulation verwendete Fahrzeug.  Es ist eine Referenz auf das Vehicle Element im [Dossier](aktenzeichenvo-1371.md) daher muss es beim Import entweder null oder mit dem Vehicle im [Dossier](aktenzeichenvo-1371.md) identisch sein. |
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
