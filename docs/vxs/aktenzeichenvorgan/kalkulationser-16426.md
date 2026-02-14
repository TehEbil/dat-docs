---
title: "Kalkulationsergebnisse CalcResultExtension"
topic_id: "16426"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > Kalkulationsergebnisse CalcResultExtension"
---

# Kalkulationsergebnisse CalcResultExtension

Die Kalkulations-Ergebnis-Elemente befinden sich unter <RepairCalculation>. Sie bündeln die Elemente mit den eigentlichen Kalkulationsdaten im Typ calcResult.

Verfügbare Elemente:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| [MaterialPositions](material-posit-1465.md) | complexType, optional  [MaterialPosition](material-posit-1465.md) | Ersatzteile |
| [MaterialPositionsMaintenance](maintenanceint-1463.md) | complexType, optional  [MaterialPosition](material-posit-1465.md) | Wartungsersatzteile |
| [AdditionalCostsPositions](nebenkosten-po-2906.md) | complexType, optional  [AdditionalCostsPosition](nebenkosten-po-2906.md) | Nebenkosten |
| AdditionalCostsPositionsMaintenance | complexType, optional  [AdditionalCostsPosition](nebenkosten-po-2906.md) | Wartungsnebenkosten |
| [LabourPositions](arbeits-positi-2958.md) | complexType, optional  [LabourPosition](arbeits-positi-2958.md) | Arbeitspositionen |
| LabourPositionsMaintenance | complexType, optional  [LabourPosition](arbeits-positi-2958.md) | Wartungs-Arbeitspositionen |
| [LacquerPositions](lack-positione-2908.md) | complexType, optional  [LacquerPosition](lack-positione-2908.md) | Lackierungspositionen |
| [SurchargesDiscounts](surchargesdisc-15559.md) | complexType, optional  SurchargeDiscountPositions | Kalkulationspositionen weitere Auf- und Abschläge |
| [DiscountPositions](discountpositi-18557.md) | complexType, optional [DiscountPosition](discountpositi-18558.md) | Rabattpositionen |
| [DeductionsPositions](deductionsposi-18561.md) | complexType, optional [DeductiblePartsPosition](deductiblepart-18562.md) | Abzugspositionen (NFA, Wertverbesserung, Vorschaden) |
| DeductiblePartsPositions | complexType, optional DeductiblePartsPosition |  |
| PriceDate | Date, optional | Preisstand |
| [RepairCalculationSummary](summe-reparatu-2919.md) | complexType, optional [CalculationSummary](summe-reparatu-2919.md) | Summierungen der Reparaturkalkulation |
| [MaterialProtocol](protokolle-mat-2904.md) | complexType, optional  [repairProtocol](protokolle-mat-2904.md) |  |
| [LabourProtocol](protokolle-mat-2904.md) | complexType, optional  [repairProtocol](protokolle-mat-2904.md) |  |
| [LacquerProtocol](protokolle-mat-2904.md) | complexType, optional  [repairProtocol](protokolle-mat-2904.md) |  |
| CalcProtocol | complexType, optional  CalculationProtocol | Kalkulationsprotokoll |
| Legends | complexType, optional  Legends |  |
| CalcType | String, optional |  |
| BlanketCalculation |  |  |
