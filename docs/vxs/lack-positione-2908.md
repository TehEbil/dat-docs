---
title: "Lack-Positionen (LacquerPosition(s))"
topic_id: "2908"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > Kalkulationsergebnisse CalcResult > Lack-Positionen (LacquerPosition(s))"
---

# Lack-Positionen (LacquerPosition(s))

Unter den in "[Kalkulationsergebnisse](#showid/1409 "Kalkulationsergebnisse CalcResult")" aufgeführten Elementen gibt es das Element <LacquerPositions>, das mehrere <LacquerPosition>-Elemente enthält. Diese enthalten Informationen über die für die Reparatur notwendigen
Lackarbeiten.

LacquerPosition (Lackierung - Standardposition):

| Element | Typ | Beschreibung |
| --- | --- | --- |
| DATProcessId | Integer | DAT-Datenverarbeitungsnummer (DVN) |
| DomusProcessId | String |  |
| Location | String |  |
| LabourPosId | String | Arbeitspositions-Nr. |
| Description | String | Beschreibung |
| Level | String | Lackstufe |
| LevelDescription | String | Lackstufenbezeichnung ["none" | "surface" | "minor" | "major" | "new"] |
| LevelManufacturer | String | Vom Hersteller angegebene Beschreibung für eine bestimmte Lackstufe. Wird nur für das Herstellerlacksystem angezeigt. |
| Material | Decimal | Materialkosten |
| MaterialPoints | Decimal | Materialpunkte |
| Duration | Decimal | Dauer (in Arbeitseinheiten) |
| ManualDuration | Decimal | Manuell eingegebene Dauer |
| ValueTotal | Decimal | Preis gesamt |
| ManualPosition | Boolean | Kennzeichen, ob manuelle Position |
| Includes | String | Beschreibung enthaltener Arbeiten (kann auch in Description enthalten sein) |
| AdditionalDesc | String | Zusätzliche Beschreibung |
| AmountDesc | String | Mengen/Typ-Beschreibung (z.B. Schraubengrößen, Kabellängen u.ä.) |
| CorrPerc | Decimal | Korrekturfaktor (Rabatte, Zuschläge) |
| ValueTotalCorrected | Decimal | Korrigierter Gesamtpreis |
| WageLevel1 | Decimal | Kosten pro Einheit in Reparaturstufe 1 (nur Frankreich) |
| WageLevel2 | Decimal | Kosten pro Einheit in Reparaturstufe 2 (nur Frankreich) |
| WageLevel3 | Decimal | Kosten pro Einheit in Reparaturstufe 3 (nur Frankreich) |
| WageLevel4 | Decimal | Kosten pro Einheit in Reparaturstufe 4 (nur Frankreich) |
| RequiredByProcessId | Integer |  |
| IsSpecific | Boolean |  |
| IncludedPositions | IncludedPosition | Die umfassten Positionen |
| AdditionalLacquerNumber | Integer |  |
| EffortDeductionPerc | Decimal |  |
| IndicatorAdditionalLacquer | String |  |
| Finish | String |  |
| Surface | Decimal |  |
| Scratches | Decimal |  |
| PriceOrigin | String |  |
| TimeOrigin | String |  |
| WorkNumber | String | Arbeitspositionsnummer |
| WorkNumberOrigin | String | Quelle/Art der Arbeitspositionsnummer |
| DATWorkNumber | String |  |
| LacquerPositionState | String | Lackierarbeitsangabe Status |
| LacquerPositionTimeState | String | Lackierarbeitszeitangabe Status |
| LacquerPositionMaterialState | String | Lackierarbeitsmaterialangabe Status |
| LacquerPositionPriceState | String | Lackierarbeitspreisangabe Status |
| MaterialType | Integer | Die Materialkennzeichnung der Lackierung, ob es sich bei dem zu lackierenden Teil um ein Metall- oder ein Kunststoffteil handelt. Mögliche Rückgabewerte:  "1" = Kunststoffteil  "2" = Blechteil" |
| Length | String | Länge des Ersatzteils. |
| Width | String | Breite des Ersatzteils. |
| <WorkIndication> | Integer, optional | Zeitangabe/Pauschale    ["0" | "1" | "3" | "4" | "6"]    0 = keine Eingabe  1 = Arbeitszeit  3 = Zeit-Aufschlag  4 = Zeit-Abschlag  6 = Pauschale (inkl. Material) |
| SparePartNumber | String, optional | Referenz zur originalen Ersatzteilnummer |
| ExternalId | String, optional | Dient als Referenz zwischen den Eingabepositionen (RepairPosition) und den Ergebnispositionen (LacquerPosition) |

LacquerWithPrepressPosition (Lackierung - Hagelschadenreparatur: Vordrücken zum Lackieren bzw. Vorziehen und Lackieren):

| Element | Typ | Beschreibung |
| --- | --- | --- |
| LacquerWithPrepressPosition | complexType, optional,  LacquerPosition | Lackposition nach Hagelreparaturweg "Vordrücken zum Lackieren" oder "Vorziehen und Lackieren" |

DentCivdPosition (Lackposition - Hagelschadenreparatur: Caravaning Industrie Verband Deutschland CIVD):

| Element | Typ | Beschreibung | Kind-Elemente |
| --- | --- | --- | --- |
| <DentCivdPosition> | complexType, optional,  LacquerPosition | Dellen-Lackposition bei der Hagelmethode CVID | [DATProcessId | Description | Duration | Material | ValueTotal | AmountDesc | Surface | DentsSize]    Neu:  DentsSize: Dellengröße in mm (nicht wie in der Oberfläche cm!)    DATProcessId: DAT Datenverarbeitungsnummer (DVN)  Description: Beschreibung (inkl. Einschlaggröße)  Duration: Arbeitszeit (Ausbeulen und Lackieren)  Material: Materialkosten (Lack- und Füll-/Hilfsmaterial)  ValueTotal: Preis gesamt  AmountDesc: Durchschnitt Anzahl Einschläge/m²  Surface: zu lackierende Gesamtfläche in m² ("bis"-Wert in Schritten, z.B. "bis 12 m²") |

SpotRepairPositions (Lackpositionen Spot Repair):

| Element | Typ | Beschreibung |
| --- | --- | --- |
| SpotRepairPosition | complexType, optional,  LacquerPosition | Spot Repair Lackposition |

OpelGoodwillLacquerPosition (Lackierung OPEL G+K)

| Element | Typ | Beschreibung |
| --- | --- | --- |
| <OpelGoodwillLacquerPosition> | LacquerPosition,  optional | Repräsentiert OPEL G+K Lack Position. Positionen werden in Abhängigkeit von PositionEntryTypeKey (OPELGOODWILL) und PositionExecutionFlag erzeugt. |
