---
title: "Kalkulationsergebnisse CalcResult"
topic_id: "1409"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > Kalkulationsergebnisse CalcResult"
---

# Kalkulationsergebnisse CalcResult

Die Kalkulations-Ergebnis-Elemente befinden sich unter <RepairCalculation>. Sie bündeln die Elemente mit den eigentlichen Kalkulationsdaten im Typ calcResult.

Verfügbare Elemente

| Element | Typ | Beschreibung |
| --- | --- | --- |
| [MaterialPositions](material-posit-1465.md) | complexType, optional  [MaterialPosition](material-posit-1465.md) | Ersatzteile |
| [MaterialPositionsMaintenance](maintenanceint-1463.md) | complexType, optional  [MaterialPosition](material-posit-1465.md) | Wartungsersatzteile |
| [AdditionalCostsPositions](nebenkosten-po-2906.md) | complexType, optional  [AdditionalCostsPosition](nebenkosten-po-2906.md) | Nebenkosten |
| AdditionalCostsPositionsMaintenance | complexType, optional  [AdditionalCostsPosition](nebenkosten-po-2906.md) | Wartungsnebenkosten |
| [ExtensionPositions](reparaturauswe-16423.md) | complexType, optional,  [ExtensionPosition](reparaturauswe-16423.md) | Reparaturausweitungs-Positionen |
| [LabourPositions](arbeits-positi-2958.md) | complexType, optional  [LabourPosition](arbeits-positi-2958.md) | Arbeitspositionen |
| LabourPositionsMaintenance | complexType, optional  [LabourPosition](arbeits-positi-2958.md) | Wartungs-Arbeitspositionen |
| [LacquerPositions](lack-positione-2908.md) | complexType, optional  [LacquerPosition](lack-positione-2908.md) | Lackierungspositionen |
| [SurchargesDiscounts](surchargesdisc-15559.md) | complexType, optional  SurchargeDiscountPositions | Kalkulationspositionen weitere Auf- und Abschläge |
| [DiscountPositions](discountpositi-18557.md) | complexType, optional [DiscountPosition](discountpositi-18558.md) | Rabattpositionen |
| [DeductionsPositions](deductionsposi-18561.md) | complexType, optional [DeductiblePartsPosition](deductiblepart-18562.md) | Abzugspositionen (NFA, Wertverbesserung, Vorschaden) |
| DeductiblePartsPositions | complexType, optional DeductiblePartsPosition |  |
| [InspectionPositions](inspektion-pos-22883.md) | complexType, optional [InspectionPositions](inspektion-pos-22883.md) | Informationen über die kalkulierten HU/AU-Positionen |
| PriceDate | Date, optional | Preisstand |
| [RepairCalculationSummary](summe-reparatu-2919.md) | complexType, optional [CalculationSummary](summe-reparatu-2919.md) | Summierungen der Reparaturkalkulation |
| [DamageSegmentation](damagesegmenta-22904.md) | complexType, optional [DamageSegmentation](damagesegmenta-22904.md) | Beinhaltet mehrere Elemente DamageSegment, die Informationen pro Schaden enthalten |
| [MaterialProtocol](protokolle-mat-2904.md) | complexType, optional  [repairProtocol](protokolle-mat-2904.md) |  |
| [LabourProtocol](protokolle-mat-2904.md) | complexType, optional  [repairProtocol](protokolle-mat-2904.md) |  |
| [LacquerProtocol](protokolle-mat-2904.md) | complexType, optional  [repairProtocol](protokolle-mat-2904.md) |  |
| CalcProtocol | complexType, optional  [CalculationProtocol](calculationpro-16543.md) | Kalkulationsprotokoll |
| Legends | complexType, optional  Legends |  |
| CalcType | String, optional |  |
| BlanketCalculation |  |  |
| LacquerPriceVersion | String | Enthält Informationen zur Preisversion der Lackierung. |
| LacquerPriceDate | Date | Enthält Informationen zum Einsatzdatum der Lackierung. |
