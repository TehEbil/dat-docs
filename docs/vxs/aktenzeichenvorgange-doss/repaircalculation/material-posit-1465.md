---
title: "Material-Positionen (MaterialPosition(s))"
topic_id: "1465"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > Kalkulationsergebnisse CalcResult > Material-Positionen (MaterialPosition(s))"
---

# Material-Positionen (MaterialPosition(s))

Unter den in "[Kalkulationsergebnisse](kalkulationser-1409.md)" aufgeführten Elementen gibt es das Element <MaterialPositions>, das mehrere <MaterialPosition>-Elemente enthält. Diese enthalten Informationen über die für die Reparatur verwendeten
Ersatzteile.

Felder

| Element | Typ | Beschreibung |
| --- | --- | --- |
| DATProcessId | Integer, optional | DAT-Verarbeitungsnummer (DVN) |
| PartNumber | String, optional | Ersatzteilnummer / Reparaturart |
| Description | String, optional | Beschreibung |
| Amount | Decimal, optional | Menge |
| ValuePerUnit | Decimal, optional | Preis pro Einheit (nicht immer gefüllt) |
| ValueTotal | Decimal, optional | Preis gesamt |
| ManualPosition | Boolean, optional | Manuelle Position? |
| PartNoValidForOrder | Boolean, optional | Ersatzteilnummer gültig für Bestellung? |
| LastUPE | Boolean, optional | Letzte UPE? |
| Includes | String, optional | Beschreibung enthaltener Teile (kann auch in Description enthalten sein) |
| AdditionalDesc | String, optional | Zusätzliche Beschreibung |
| AmountDesc | String, optional | Mengen/Typ-Beschreibung (z.B. Schraubengrößen, Kabellängen u.ä.) |
| CorrPerc | Decimal, optional | Korrekturfaktor bei Positionsrabatten |
| ValueTotalCorrected | Decimal, optional | Korrigierter Gesamtwert |
| FootNote | String, optional | Fußnote / Zusatzinformation |
| Extended | Boolean, optional | Extended = true definiert die Positionen, die durch die Kalkulationslogik zusätzlich erfasst wurden. |
| IncludedInCalculation | Boolean, optional | Falls true, ist die Position im Kalkulationsergebnis berücksichtigt. |
| PartOrigin | String, optional | Die Herkunft eines Ersatzteils. Rückgabewerte:  "OE" = Originalteil mit Herstellerpreis  "EX" = Austauschteil  "NA" = Information nicht verfügbar (Default, keine weitere Aussage über die Herkunft des Ersatzteils möglich) |
| Predefined | Boolean, optional | Vordefinierte Ersatzteilposition |
| Manufacturer | String, optional | Ersatzteilhersteller |
| WearRus | complexType, optional, MTPLWearRus | Verschleißwert, nur für Datenland Russland |
| Dimension | String, optional | Dimension |
| ExternalId | String, optional | Dient als Referenz zwischen den Eingabepositionen (RepairPosition) und den Ergebnispositionen (MaterialPosition) |
| ManualPrice | Boolean, optional | Manuelle Preiseingabe |
| AmountState | String, optional | Quelle / Art der Menge |
| PartUnitPriceState | String, optional | Quelle / Art des Preises |
