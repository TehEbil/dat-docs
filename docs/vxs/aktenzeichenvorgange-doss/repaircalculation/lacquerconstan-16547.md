---
title: "LacquerConstants"
topic_id: "16547"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > Kalkulationsergebnisse CalcResult > Summe Reparatur-Kalkulation (RepairCalculationSummary) > LacquerCostsSummary > LacquerMaterialSummary > LacquerConstants"
---

# LacquerConstants

###### LacquerConstants Unter den in"[Kalkulationsergebnisse](kalkulationser-1409.md)" aufgeführten Elementen gibt es das Element <LacquerConstants>, das mehrere <LacquerConstant>-Elemente enthält. Felder | Element | Typ | Beschreibung | Mögliche Werte | | --- | --- | --- | --- | | Id | String, optional | | | | Description | String, optional | | | | Price | Decimal, optional | | | | Parameter | String, optional | | | | Unit | String, optional | | | | ConstantType | Integer, optional | | | | ValueInPositions | Boolean, optional | Ist der Wert der Lackmaterial-Konstante in LacquerPositions bereits enthalten? Bspw. bei AZT oder Spot Repair wird der Material-Anteil in den Lackpositionen (LacquerPositions) ausgewiesen. Aus diesem Grund darf der Wert der entsprechenden LacquerConstants nicht noch einmal zu diesen addiert werden, um den Material-Gesamtwert <TotalSum> zu berechnen. ValueInPositions ist in diesem Fall true. Bei z.B. DAT Eurolack dagegen müssen die Konstanten zusätzlich addiert werden (ValueInPositions=false). | [true|false] | | ValueForInformation | Boolean, optional | Ist der Wert der Lackmaterial-Konstante nur zur Information? Bspw. bei dem für manche Länder verfügbaren Materialzuschlag für Mineral-/Perl-Effekt ist das Lackmaterial bereits in anderen Nodes unter <Material> enthalten und darf nicht zu diesen addiert werden um den Material-Gesamtwert <TotalSum> zu erhalten. In diesem Fall ist ValueForInformation dann "true". | [true|false] |
