---
title: "Wichtige Abkündigungen des Lacksystems DAT-Eurolack"
topic_id: "31554"
breadcrumb: "Technische Informationen > Ausgabe Nr. 94 Dezember 2025 > Reparaturkostenkalkulation > SilverDAT calculatePro/SilverDAT calculateItalia > Abkündigungen > Wichtige Abkündigungen des Lacksystems DAT-Eurolack"
---

# Wichtige Abkündigungen des Lacksystems DAT-Eurolack

Im zweiten Quartal 2026 erfolgen wichtige Abkündigungen am Lacksystem DAT-Eurolack.
Im Zuge dieser Abkündigungen werden folgende Elemente nach Einhaltung der 6-monatigen
Abkündigungsfrist endgültig aus der Schnittstelle entfernt:

In <ProcedureRelatedParameter> unter EuroLacquerFactor entfallen folgende Attribute:

<RepairCalculation><ProcedureRelatedParameters>

| attribute | factor | type | mode | Beschreibung |
| --- | --- | --- | --- | --- |
| <materialPerPointCost> | EuroLacquerFactor | Price | ABSOLUTE | Materialkosten pro Materialpunkt |
| <isLacquerPlasticWhenFitted> | EuroLacquerFactor | Boolean |  | Kunststoffteile eingebaut lackieren |

Unter <RepairPosition> entfällt folgender Parameter:

<RepairCalculation><RepairPositions><RepairPosition>

| Element | Typ | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| <LacquerScratchProofFinishTime> | Decimal, optional |  | Lackfinish kratzfeste Klarlacke |

Unter <LacquerPosition> entfällt folgender Parameter:

<RepairCalculation><CalcResultCommon><LacquerPositions><LacquerPosition>

| Element | Typ | Beschreibung |
| --- | --- | --- |
| <MaterialPoints> | Decimal | Materialpunkte |

Bitte beachten Sie, dass die oben erwähnte Schnittstellenabkündigung alle Kalkulationsarten
mit dem Datentyp calcResult betreffen wird.

Das Beispiel bezieht sich auf die Kalkulationsart CalcResultCommon für eine Standardkalkulation.

Allerdings sind weitere Kalkulationsarten wie bspw.

- CalcResultGlass (Glaskalkulation)
- CalcResultOptimized (Optimierte Kalkulation)
- CalcResultExtension (Reparaturkostenausweitungs-Kalkulation)
- CalcResultMaintenance (Wartungskalkulation)
- CalcResultSPO (Ersatzteiloptimierungskalkulation)

von den Erweiterungen betroffen.

Bitte berücksichtigen Sie die aufgeführten Abkündigungen in Ihrer eigenen Implementierung.
Führen Sie, wenn nötig, rechtzeitig entsprechende Anpassungen durch!
