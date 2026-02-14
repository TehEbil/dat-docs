---
title: "SparePartsCostsSummary"
topic_id: "15105"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > Kalkulationsergebnisse CalcResult > Summe Reparatur-Kalkulation (RepairCalculationSummary) > SparePartsCostsSummary"
---

# SparePartsCostsSummary

Felder:

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| AllSum | Decimal, optional |  |
| ProcurementCosts | Decimal, optional |  |
| ProcurementCostsFromParts | Decimal, optional | Der Aufschlag für Beschaffungskosten (für das Datenland Österreich) |
| ProcurementCostsFromPartsPercentage | Decimal, optional | Der prozentuale Aufschlag für Beschaffungskosten (für das Datenland Österreich) |
| ConsumablesSurcharge | Decimal, optional | Der Aufschlag für Klein- bzw. Verbrauchsmaterial |
| ConsumablesSurchargePercentage | Decimal, optional | Der prozentuale Aufschlag für Klein- bzw. Verbrauchsmaterial |
| SurchargeDeduction | Decimal, optional |  |
| DisposalCostsSpareParts | Decimal, optional | Der Aufschlag für Entsorgungskosten (für das Datenland Österreich) |
| DisposalCostsSparePartsPercentage | Decimal, optional | Der prozentuale Aufschlag für Entsorgungskosten (für das Datenland Österreich) |
| SmallMaterialsLumpSum | Decimal, optional | Kleinmaterialpauschale (von Summe Arbeitslohn Sanfte Instandsetzung)  2% für Deutschland (landesspezifisch) |
| TotalSum | Decimal, optional |  |
| SparePartsTotalWear | Decimal, optional | Summe des Verschleißes aller Ersatzteile, nur für Datenland Russland |
| SparePartsTotalPartsWear | Decimal, optional | Summe aller Ersatzteile mit Verschleiß und ohne Kleinersatzteile, nur für Datenland Russland |
| SparePartsTotalTotalWear | Decimal, optional | Summe aller Ersatzteile mit Verschleiß und mit kleinen Ersatzteilen, nur für Datenland Russland |

Der Parameter DentAdhesiveMaterial wurde von SparePartsCostsSummary nach <RepairCalculation><CalcResultCommon><AdditionalCostsPositions><AdditionalCostsPosition>
verschoben.
