---
title: "RepairCalculation"
topic_id: "1407"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation"
---

# RepairCalculation

Das Element <RepairCalculation> enthält die Kalkulationsergebnisse sowie alle Daten die zur Kalkulation benötigt
werden. Es befindet sich direkt unter dem [Dossier](#showid/1371 "Aktenzeichen/Vorgang (Dossier)") Element.

Die Kalkulationsergebnisse werden als in ein CalcResult Elemente abgelegt. Das CalcResultToUse gibt jeweils an welches Ergebnis gültig ist.

Felder:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| [Vehicle](#showid/6692 "Fahrzeug (Vehicle)") | [Vehicle](#showid/6692 "Fahrzeug (Vehicle)") | Das für die Kalkulation verwendete Fahrzeug.  Es ist eine Referenz auf das Vehicle Element im [Dossier](#showid/1371 "Aktenzeichen/Vorgang (Dossier)") daher muss es beim Import entweder null oder mit dem Vehicle im [Dossier](#showid/1371 "Aktenzeichen/Vorgang (Dossier)") identisch sein. |
| RepairWages | RepairWages | Lohnsätze |
| [RepairParameters](#showid/1415 "RepairParameters ") | [RepairParameters](#showid/1415 "RepairParameters ") | Kalkulationsparameter (alt) |
| [ProcedureRelatedParameters](#showid/14058 "ProcedureRelatedParameters") | [ProcedureRelatedParameters](#showid/14058 "ProcedureRelatedParameters") | Kalkulationsparameter (neu) |
| [RepairPositions](#showid/1417 "RepairPositions") | [RepairPositions](#showid/1417 "RepairPositions") | Enthält eine Liste mit Reparaturpositionen |
| CalcResultToUse | String | Beschreibt, welche Kalkulation verwendet wird. Das gilt für die folgenden Typen:  "common", "optimized", "glass", "italyCommon", "italyOptimized", "italyGlass","SPO","EXTERNAL", "DAT" |
| [CalcResultCommon](#showid/1409 "Kalkulationsergebnisse CalcResult") | [CalcResult](#showid/1409 "Kalkulationsergebnisse CalcResult") | Standardkalkulation  "common" --> VehicleRepairOnline  "DAT" -->myClaim  "EXTERNAL" --> eigene Kalkulation nur für myClaim |
| [CalcResultExtension](#showid/16426 "Kalkulationsergebnisse CalcResultExtension") | [CalcResult](#showid/1409 "Kalkulationsergebnisse CalcResult") | Reparaturkostenausweitungs-Kalkulation |
| [CalcResultGlass](#showid/1409 "Kalkulationsergebnisse CalcResult") | [CalcResult](#showid/1409 "Kalkulationsergebnisse CalcResult") | Glaskalkulation  "glass" |
| [CalcResultOptimized](#showid/1409 "Kalkulationsergebnisse CalcResult") | [CalcResult](#showid/1409 "Kalkulationsergebnisse CalcResult") | Optimierte Kalkulation Rohbaukarosserie  "optimized" |
| CalcResultItaly | CalcResultItaly | Standardkalkulation (nur für Italien)  "italyCommon" |
| CalcResultItalyOptimized | CalcResultItaly | Optimierte Berechnung mit Rohbaukarosserie (nur für Italien)  "italyOptimized" |
| CalcResultItalyGlass | CalcResultItaly | Glaskalkulation (nur für Italien)  "italyGlass" |
| CalcResultDomus |  |  |
| CalcResultDomusOptimized |  |  |
| CalcResultDomusGlass |  |  |
| [CalcResultCustomerRanking](#showid/1409 "Kalkulationsergebnisse CalcResult") | [CalcResult](#showid/1409 "Kalkulationsergebnisse CalcResult") |  |
| [CalcResultMaintenance](#showid/1409 "Kalkulationsergebnisse CalcResult") | [CalcResult](#showid/1409 "Kalkulationsergebnisse CalcResult") | Wartungskalkulation  "maintenance" |
| CalcResultsHistory |  | Kalkulationshistorie |
| CalcResultSPO | [CalcResult](#showid/1409 "Kalkulationsergebnisse CalcResult") | Spare Parts Optimization Calculation Ersatzteiloptimierungskalkulation |
| DiscountPositions | DiscountPositions |  |
| CalculationSummary | [CalculationSummary](#showid/2919 "Summe Reparatur-Kalkulation (RepairCalculationSummary) ") |  |
| SurchargeSettings | SurchargeSettings |  |
| SettingsParameters | complexType, optional,  [SettingsParameters](#showid/16545 "SettingsParameters") | Liste an Wertemengen, die folgende kalkulationsrelevante Einstellungen modelliert:  Ersatzteile-Einstellungen  Arbeit-Einstellungen  Lack-Einstellungen  Allgemeine Einstellungen |
