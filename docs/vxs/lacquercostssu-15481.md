---
title: "LacquerCostsSummary"
topic_id: "15481"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > Kalkulationsergebnisse CalcResult > Summe Reparatur-Kalkulation (RepairCalculationSummary) > LacquerCostsSummary"
---

# LacquerCostsSummary

Felder

| Parameter | Typ | Beschreibung | Mögliche Werte |
| --- | --- | --- | --- |
| DiscountTotalFlat | complexType, optional | Pauschaler Rabatt auf die Lackierungskosten |  |
| TotalFlat | Decimal, optional | Pauschale Gesamtsumme |  |
| WageAndMaterial | complexType, optional  detailBlockSummary | Summenblock Lohn und Material kombiniert |  |
| Wage | complexType, optional,  detailBlockSummary | Lacklohn konventionelle Lackierung  Type: LACQUER WORK  Units: Anzahl Arbeitseinheiten  PricePerUnit: Preis pro Arbeitseinheit  Price: Gesamtpreis Lacklohn für konventionelle Lackierung | [Type | Units | PricePerUnit | Price] |
| SpotRepairWage | complexType, optional,  detailBlockSummary | Spot Repair Lohn  Type: LACQUER WORK SPOTS  Units: Anzahl Arbeitseinheiten  PricePerUnit: Preis pro Arbeitseinheit  Price: Gesamtpreis Spot Repair Lacklohn | [Type | Units | PricePerUnit | Price] |
| TotalWages | Decimal, optional | Gesamtsumme Lacklohn |  |
| TotalTimeUnits | Decimal, optional | Gesamtsumme Arbeitseinheiten der Lackierungskosten |  |
| DentsCivdWage | complexType, optional,  detailBlockSummary | Summenblock Lacklohn: Hagelschadenreparatur CIVD: Instandsetzen    Type: HAIL CIVD WORK  Units: Anzahl Arbeitseinheiten  PricePerUnit: Preis pro Arbeitseinheit  Price: Gesamtpreis Lacklohn Hagelschadenreparatur CIVD: Instandsetzen | [Type | Units | PricePerUnit | Price] |
| DentsCivdMaterial | complexType, optional  detailBlockSummary | Summenblock Lackmaterial: Hagelschadenreparatur CIVD: Materialkosten    Type: HAIL CIVD MATERIAL  Units: Anzahl Arbeitseinheiten  PricePerUnit: Preis pro Arbeitseinheit  Price: Gesamtpreis Lackmaterial Hagelschadenreparatur CIVD: Materialkosten | [Type | Units | PricePerUnit | Price] |
| Material | complexType, optional  [LacquerMaterialSummary](#showid/15519 "LacquerMaterialSummary") | Summenblock Material |  |
| TotalSum | Decimal | Gesamtsumme Lackmaterial und Lacklohn |  |
