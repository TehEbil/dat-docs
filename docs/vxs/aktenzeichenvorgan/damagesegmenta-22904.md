---
title: "DamageSegmentation"
topic_id: "22904"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > Kalkulationsergebnisse CalcResult > DamageSegmentation"
---

# DamageSegmentation

Unter den in "[Kalkulationsergebnisse](kalkulationser-1409.md)" aufgeführten Elementen gibt es das Element <DamageSegmentation>, das mehrere <DamageSegment>-Elemente enthält. Diese enthalten Informationen pro Schaden.

Felder

| Element | Typ | Beschreibung |
| --- | --- | --- |
| DamageNumber | Integer | Enthält die laufende Nummer des Schadens |
| DamageName | String | Enthält die Bezeichnung des Schadens |
| calcResult | complexType, calcResult | Enthält das Kalkulationergebnis für diesen Schaden |
