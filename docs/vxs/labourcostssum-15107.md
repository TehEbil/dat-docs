---
title: "LabourCostsSummary"
topic_id: "15107"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > Kalkulationsergebnisse CalcResult > Summe Reparatur-Kalkulation (RepairCalculationSummary) > LabourCostsSummary"
---

# LabourCostsSummary

Felder

| Parameter | Typ | Beschreibung | Mögliche Werte |
| --- | --- | --- | --- |
| AllSum | Decimal, optional |  |  |
| Bodywork | complexType, optional  detailBlockSummary | Summenblock Karosseriearbeit |  |
| Electric | complexType, optional  detailBlockSummary | Summenblock für Elektrikarbeit |  |
| Mechanic | complexType, optional,  detailBlockSummary | Summenblock für Mechanikarbeit |  |
| Works | [Work[]](#showid/22593 "Work") | Zusammensetzung der unterschiedlichen Arbeitslöhne: Karosserie | Elektrik | Mechanik |  |
| OpelGoodWill | complexType, optional,  detailBlockSummary | Bezieht sich auf die Zusammenfassung von OPEL G+K Arbeitspositionen. |  |
| DentsPress | complexType, optional  detailBlockSummary | Summenblock Hagelreparaturmethode Drücken |  |
| DentsPrePress | complexType, optional  detailBlockSummary | Summenblock Hagelreparaturmethode Vordrücken / Vorziehen und Lackieren |  |
| DentsGlobal | complexType, optional,  detailBlockSummary | Summenblock Hagelreparatur für übergreifende Hagelpositionen |  |
| DentsFlat | complexType, optional,  detailBlockSummary | Summenblock pauschale Lohnkosten der Hagelreparatur | [Type | Price]    Type: FLAT PRICE HAIL DAMAGE  Price: Lohnkosten Pauschal |
| ParkingDents | complexType, optional,  detailBlockSummary | Summenblock Arbeitslohn: Parkdellenreparatur: Lackschadenfrei    Type: PARKING DENTS  Units: Anzahl Arbeitseinheiten  PricePerUnit: Preis pro Arbeitseinheit  Price: Gesamtpreis Lacklohn Parkdellenreparatur: Lackschadenfrei | [Type | Units | PricePerUnit | Price] |
| ParkingDentsLacquerDeduction | complexType, optional,  detailBlockSummary | Summenblock Arbeitslohn: Parkdellenreparatur: 40% Abzug bei Lackierung (auf alle Parkdellen-Positionen mit Lackierung)    Type: PARKING DENTS LACQUER DEDUCTION  Units: Anzahl Arbeitseinheiten  PricePerUnit: Preis pro Arbeitseinheit  Discount: Abzug (derzeit "40%")  Price: Gesamt-Abzug (negativer Wert) | [Type | Units | PricePerUnit | Discount | Price] |
| TotalSum | Decimal, optional |  |  |
| Discount | complexType, optional,  Discount |  |  |
| Wages | complexType, optional,  DetailBlockSummaryWages |  |  |
