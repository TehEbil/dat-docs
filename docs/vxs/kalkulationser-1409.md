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
| [MaterialPositions](#showid/1465 "Material-Positionen (MaterialPosition(s))") | complexType, optional  [MaterialPosition](#showid/1465 "Material-Positionen (MaterialPosition(s))") | Ersatzteile |
| [MaterialPositionsMaintenance](#showid/1463 "MaintenanceIntervals (MaintenancePosition)") | complexType, optional  [MaterialPosition](#showid/1465 "Material-Positionen (MaterialPosition(s))") | Wartungsersatzteile |
| [AdditionalCostsPositions](#showid/2906 "Nebenkosten-Positionen (AdditionalCostsPosition(s))") | complexType, optional  [AdditionalCostsPosition](#showid/2906 "Nebenkosten-Positionen (AdditionalCostsPosition(s))") | Nebenkosten |
| AdditionalCostsPositionsMaintenance | complexType, optional  [AdditionalCostsPosition](#showid/2906 "Nebenkosten-Positionen (AdditionalCostsPosition(s))") | Wartungsnebenkosten |
| [ExtensionPositions](#showid/16423 "Reparaturausweitungs-Positionen") | complexType, optional,  [ExtensionPosition](#showid/16423 "Reparaturausweitungs-Positionen") | Reparaturausweitungs-Positionen |
| [LabourPositions](#showid/2958 "Arbeits-Positionen (LabourPosition(s))") | complexType, optional  [LabourPosition](#showid/2958 "Arbeits-Positionen (LabourPosition(s))") | Arbeitspositionen |
| LabourPositionsMaintenance | complexType, optional  [LabourPosition](#showid/2958 "Arbeits-Positionen (LabourPosition(s))") | Wartungs-Arbeitspositionen |
| [LacquerPositions](#showid/2908 "Lack-Positionen (LacquerPosition(s))") | complexType, optional  [LacquerPosition](#showid/2908 "Lack-Positionen (LacquerPosition(s))") | Lackierungspositionen |
| [SurchargesDiscounts](#showid/15559 "SurchargesDiscounts (Veraltet!)") | complexType, optional  SurchargeDiscountPositions | Kalkulationspositionen weitere Auf- und Abschläge |
| [DiscountPositions](#showid/18557 "DiscountPositions") | complexType, optional [DiscountPosition](#showid/18558 "DiscountPosition") | Rabattpositionen |
| [DeductionsPositions](#showid/18561 "DeductionsPositions") | complexType, optional [DeductiblePartsPosition](#showid/18562 "DeductiblePartsPosition") | Abzugspositionen (NFA, Wertverbesserung, Vorschaden) |
| DeductiblePartsPositions | complexType, optional DeductiblePartsPosition |  |
| [InspectionPositions](#showid/22883 "Inspektion-Positionen (InspectionPosition(s))") | complexType, optional [InspectionPositions](#showid/22883 "Inspektion-Positionen (InspectionPosition(s))") | Informationen über die kalkulierten HU/AU-Positionen |
| PriceDate | Date, optional | Preisstand |
| [RepairCalculationSummary](#showid/2919 "Summe Reparatur-Kalkulation (RepairCalculationSummary) ") | complexType, optional [CalculationSummary](#showid/2919 "Summe Reparatur-Kalkulation (RepairCalculationSummary) ") | Summierungen der Reparaturkalkulation |
| [DamageSegmentation](#showid/22904 "DamageSegmentation") | complexType, optional [DamageSegmentation](#showid/22904 "DamageSegmentation") | Beinhaltet mehrere Elemente DamageSegment, die Informationen pro Schaden enthalten |
| [MaterialProtocol](#showid/2904 "Protokolle MaterialProtocol LabourProtocol LacquerProtocol") | complexType, optional  [repairProtocol](#showid/2904 "Protokolle MaterialProtocol LabourProtocol LacquerProtocol") |  |
| [LabourProtocol](#showid/2904 "Protokolle MaterialProtocol LabourProtocol LacquerProtocol") | complexType, optional  [repairProtocol](#showid/2904 "Protokolle MaterialProtocol LabourProtocol LacquerProtocol") |  |
| [LacquerProtocol](#showid/2904 "Protokolle MaterialProtocol LabourProtocol LacquerProtocol") | complexType, optional  [repairProtocol](#showid/2904 "Protokolle MaterialProtocol LabourProtocol LacquerProtocol") |  |
| CalcProtocol | complexType, optional  [CalculationProtocol](#showid/16543 "CalculationProtocol") | Kalkulationsprotokoll |
| Legends | complexType, optional  Legends |  |
| CalcType | String, optional |  |
| BlanketCalculation |  |  |
| LacquerPriceVersion | String | Enthält Informationen zur Preisversion der Lackierung. |
| LacquerPriceDate | Date | Enthält Informationen zum Einsatzdatum der Lackierung. |
