---
title: "Arbeits-Positionen (LabourPosition(s))"
topic_id: "2958"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > Kalkulationsergebnisse CalcResult > Arbeits-Positionen (LabourPosition(s))"
---

# Arbeits-Positionen (LabourPosition(s))

Unter den in "[Kalkulationsergebnisse](kalkulationser-1409.md)" aufgeführten Elementen gibt es das Element <LabourPositions>, das mehrere <LabourPosition>- und <DentPosition>-Elemente enthält.

Diese enthalten Informationen über die für die Reparatur notwendigen Arbeiten.

LabourPosition (Arbeitslohn - Standardposition):

| Element | Typ | Beschreibung |
| --- | --- | --- |
| DATProcessId | Integer, optional | DAT-Datenverarbeitungsnummer (DVN) |
| RepairType | String, optional | Reparatur-Art |
| LabourPosId | String, optional | Arbeitspositions-Nr. |
| Description | String, optional | Beschreibung |
| WageType | String, optional | Arbeitsart |
| WageLevel | Integer, optional | Arbeitsstufe |
| Duration | Decimal, optional | Dauer (in Arbeitseinheiten) |
| ManualDuration | Boolean, optional | Manuell eingegebene Dauer (wird nicht ausgewertet) |
| ValueTotal | Decimal, optional | Lohn gesamt |
| ValueInPosition | Boolean, optional | Ist true, wenn alle Zuschläge (z.B. Zuschlag LM-Teil, Zuschlag Klebetechnik 30%) als separate Positionen aufgeführt werden, jedoch im Parameter ValueTotalCorrected der Hauptpositionen enthalten sind. |
| ManualPosition | Boolean, optional | Kennzeichen, ob manuelle Position |
| Includes | String, optional | Beschreibung enthaltener Arbeiten (kann auch in Description enthalten sein) |
| AdditionalDesc | String, optional | Zusätzliche Beschreibung |
| AmountDesc | String, optional | Mengen/Typ-Beschreibung (z.B. Schraubengrößen, Kabellängen u.ä.) |
| CorrPerc | Decimal, optional | Korrekturfaktor bei Positionsrabatten |
| ValueTotalCorrected | Decimal, optional | Korrigierter Gesamtwert |
| WageLevel1 – WageLevel4 | Decimal, optional | Gesamtlöhne für Arbeitsverteilung (Frankreich) |
| Amount | Integer, optional | Anzahl der Dellen |
| hasRequiredByPosition | Boolean, optional | [true | false] |
| RequiredByPosition | complexType, optional | Automatisch zugesteuerte Positionen (nicht umfasste Positionen) |
| InculdedPositions | complexType, optional  InculdedPosition | Die umfassten Positionen |
| Extended | Boolean, optional | Definiert die Positionen, die durch die Kalkulationslogik automatisch ergänzt wurden. |
| IncludedInCalculation | Boolean, optional | Ist false, wenn eine automatische ergänzte Position (Extended=true) nicht im Kalkulationsergebnis berücksichtigt wurde. Dies ist von der Einstellung "Preis/Arbeitszeit bei zugesteuerten Positionen nicht berücksichtigt". |
| Method | String, optional |  |
| HardshipAllowanceInd | Character, optional |  |
| optionalPositionIncluded | Boolean, optional |  |
| LabourPositionState | String, optional |  |
| LabourPositionPriceState | String, optional | Arbeitspreisangabe Status |
| LabourPositionTimeState | String, optional | Arbeitszeitangabe Status    P: Parkdellenposition ohne Lackierung  PL: Parkdellenpositionen mit Lackierung |
| size | Integer, optional |  |
| PriceOrigin | String, optional |  |
| TimeOrigin | String, optional |  |
| WorkNumber | String, optional | Arbeitspositionsnummer |
| WorkNumberOrigin | String, optional | Quelle/Art der Arbeitspositionsnummer |
| DATWorkNumber | String, optional |  |
| Length | Decimal, optional | Länge des Ersatzteils. |
| Width | Decimal, optional | Breite des Ersatzteils. |
| <WorkIndication> | Integer, optional | Zeitangabe/Pauschale    ["0" | "1" | "2" | "3" | "4" | "5" | "6"]    0 = keine Eingabe  1 = Arbeitszeit  2 = Lohnkosten Pauschal  3 = Zeit-Aufschlag  4 = Zeit-Abschlag  5 = Erschwerniszuschlag  6 = Pauschale (inkl. Material) |
| SparePartNumber | String, optional | Referenz zur originalen Ersatzteilnummer |
| ExternalId | String, optional | Dient als Referenz zwischen den Eingabepositionen (RepairPosition) und den Ergebnispositionen (LabourPosition) |
| ManualWageType | Boolean, optional | Manuelle Arbeitsposition |

DentPrepressPosition (Arbeitslohn - Hagelschadenreparatur: Vorziehen und Lackieren "Deutsche Kommission
für Lack und Karosserieinstandsetzung"):

| Element | Typ | Beschreibung |
| --- | --- | --- |
|  |  |  |

DentDtCommPosition (Arbeitslohn - Lackschadenfreie Reparatur Methode "Deutsche Kommission für Lack und
Karosserieinstandsetzung"):

| Element | Typ | Beschreibung |
| --- | --- | --- |
|  |  |  |

DentDtCommSumPosition (Arbeitslohn - Summe der Arbeitszeit nach Tabelle "Deutsche Kommission für Lack und
Karosserieinstandsetzung"):

| Element | Typ | Beschreibung |
| --- | --- | --- |
|  |  |  |

DentBvatPosition (Arbeitslohn - Lackschadenfreie Reparatur Methode und "Vordrücken und Lackieren" für
"Hagelschadenzentrum BVAT"):

| Element | Typ | Beschreibung |
| --- | --- | --- |
| DentsCalculationMethod | String, optional | press = Drücken  pre-press = Vordrücken und Lackieren  global = übergreifende Positionen wie Vorbereitungszeit |

OpelGoodwillLabourPosition (Arbeitslohn OPEL G+K)

| Element | Typ | Beschreibung |
| --- | --- | --- |
| OpelGoodwillLabourPosition | LabourPosition,  optional | Repräsentiert OPEL G+K Work Position. Positionen werden in Abhängigkeit von PositionEntryTypeKey erzeugt. |
