---
title: "Nebenkosten-Positionen (AdditionalCostsPosition(s))"
topic_id: "2906"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > Kalkulationsergebnisse CalcResult > Nebenkosten-Positionen (AdditionalCostsPosition(s))"
---

# Nebenkosten-Positionen (AdditionalCostsPosition(s))

Unter den in "[Kalkulationsergebnisse](#showid/1409 "Kalkulationsergebnisse CalcResult")" aufgeführten Elementen gibt es das Element <AdditionalCostsPositions>, das mehrere <AdditionalCostsPosition>-Elemente enthält. Diese enthalten Informationen über Nebenkosten der Reparatur.

Felder:

| Element | Typ | Beschreibung | Mögliche Werte |
| --- | --- | --- | --- |
| DATProcessId | Integer | DAT-Vorgangsnummer |  |
| Description | String | Beschreibung |  |
| ValueTotal | Decimal | Preis gesamt |  |
| ManualPosition | Boolean | Manuelle Position |  |
| ValuePerUnit | Decimal | Ersatzteilpreis |  |
| QuantityUnit | String | Einheit Material | ["" | CCM | DOSE| KART | KG | LFM | LTR | PAAR | PACK | QCM | QDM | QM | SATZ | STCK]    "": keine Angabe  CCM: Kubikzentimeter  DOSE: Dose(n)  KART: Kartuschen  KG: Kilogramm  LFM: Lfd. Meter  LTR: Liter  PAAR: Paar  PACK: Packungen  QCM: Quadratzentimeter  QDM: Quadratdezimeter  QM: Quadratmeter  SATZ: Satz  STCK: Stück |
| Amount | Decimal | Anzahl der Ersatzteile |  |
| PartNumber | String | Ersatzteilnummer |  |
| PartNumberOrigin | String | Quelle/Art der Ersatzteilnummer |  |
| ExternalId | String | Dient als Referenz zwischen den Eingabepositionen (RepairPosition) und den Ergebnispositionen (AdditionalCostsPosition) |  |
