---
title: "Wichtige Änderungen und Erweiterungen des Lacksystems DAT-Eurolack"
topic_id: "32034"
breadcrumb: "Technische Informationen > Ausgabe Nr. 95 Februar 2026 > Reparaturkostenkalkulation > SilverDAT calculatePro/SilverDAT calculateItalia > Erweiterungen > Wichtige Änderungen und Erweiterungen des Lacksystems DAT-Eurolack"
---

# Wichtige Änderungen und Erweiterungen des Lacksystems DAT-Eurolack

Voraussichtlich im zweiten Quartal 2026 erfolgen wichtige Änderungen und Erweiterungen
am Lacksystem DAT-Eurolack. Eine wesentliche Änderung betrifft die Kalkulation: Das
Lackmaterial wird künftig nicht mehr auf Basis des Preises pro Materialpunkt, sondern
pro Quadratdezimeter berechnet. Im Zuge dieser Änderungen und Erweiterungen werden
folgende Punkte umgesetzt:

Änderungen

Das Attribut <materialIndex> unter dem EuroLacquerFactor im ProcedureRelatedParameter wird um zwei zusätzliche Attribute erweitert: <materialIndexPreparation> und <materialIndexComponents> (siehe Abschnitt Erweiterungen). Der gesamte Materialindex erhöht den gesamten Materialpreis
inklusive Materialindex Vorbereitung und Materialindex Bauteile. Beachten Sie, dass
die drei einzelnen Materialindizes separat betrachtet werden müssen. Wird der gesamten
Materialindex erhöht, sind die Materialindizes Vorbereitung und Bauteile gesperrt.

<RepairCalculation><ProcedureRelatedParameters>

| attribute | factor | type | mode | Beschreibung |
| --- | --- | --- | --- | --- |
| <materialIndex> | EuroLacquerFactor | Double |  | Prozentuale Angabe des gesamten Materialindexes. Bitte beachten Sie, dass dieses Attribut dem bisherigen Materialindex entspricht; zusätzlich wurden die Attribute Materialindex Vorbereitung und Materialindex Bauteile eingeführt. |

Erweiterungen

Der ProcedureRelatedParameter wird unter den EuroLacquerFactor um folgende Elemente erweitert:

<RepairCalculation><ProcedureRelatedParameters>

| attribute | factor | type | mode | Beschreibung | Mögliche Werte |
| --- | --- | --- | --- | --- | --- |
| <materialIndexPreparation> | EuroLacquerFactor | Double |  | Prozentuale Angabe des Materialindexes für die Vorbereitung. |  |
| <materialIndexComponents> | EuroLacquerFactor | Double |  | Prozentuale Angabe des Materialindexes für die Bauteile. |  |
| <isSurchargeForMatt> | EuroLacquerFactor | Boolean |  | Angabe, ob ein Zuschlag für die Mattlackierung (Absetzfarbe) berücksichtigt wird. |  |
| <isSurchargeForMattSmallParts> | EuroLacquerFactor | Boolean |  | Angabe, ob ein Zuschlag für die Mattlackierung (Absetzfarbe) von Kleinteilen berücksichtigt wird. |  |
| <lacquerTechnique> | EuroLacquerFactor | LacquerTechnique |  | Angabe für die Lackierung der 3-/4-Schicht. Hier wird eingegeben, ob die Lackiertechnik „Nass in nass“ oder "Trocken und schleifen" angewendet wurde. | {WET\_IN\_WET | DRY\_AND\_SAND}    WET\_IN\_WET: Nass in nass  DRY\_AND\_SAND: Trocken und schleifen |

Der Parameter RepairPosition wird um folgende Elemente erweitert:

<RepairCalculation><RepairPositions><RepairPosition>

| Element | Typ | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| <LacquerStoneChipProtection> | Boolean, optional | [true | false]    true: Der Steinschlagschutz wird für das Fahrzeug berücksichtigt.    false: Der Steinschlagschutz wird für das Fahrzeug nicht berücksichtigt. | Angabe, ob der Steinschlagschutz für das Fahrzeug berücksichtigt wird oder nicht. Bitte beachten Sie, dass dieses Element nur für die Reparaturcodes „Lackieren (L)" und „Montageteil demontiert lackieren (M)" gilt. |
| <LacquerCorrosionProtection> | Boolean, optional | [true | false]    true: Der Korrosionsschutz wird für das Fahrzeug berücksichtigt.    false: Der Korrosionsschutz wird für das Fahrzeug nicht berücksichtigt. | Angabe, ob der Korrosionsschutz für das Fahrzeug berücksichtigt wird oder nicht. Bitte beachten Sie, dass dieses Element nur für die Reparaturcodes „Lackieren (L)" und „Montageteil demontiert lackieren (M)" gilt. |
| <LacquerHardshipAllowance> | Boolean, optional | [true | false]    true: Der Erschwerniszuschlag für Instandsetzung wird für das Fahrzeug berücksichtigt.    false: Der Erschwerniszuschlag für Instandsetzung wird für das Fahrzeug nicht berücksichtigt. | Angabe, ob der Erschwerniszuschlag für Instandsetzung für das Fahrzeug berücksichtigt wird oder nicht. Bitte beachten Sie, dass dieses Element nur für die Reparaturcodes „Lackieren (L)" und „Montageteil demontiert lackieren (M)" und für die Lackstufen 2 und 3 gilt. |
| <LacquerPrePaintingComponents> | Boolean, optional | [true | false]    true: Das Bauteil ausgebaut zum Vorlackieren wird berücksichtigt.    false: Das Bauteil ausgebaut zum Vorlackieren wird nicht berücksichtigt. | Angabe, ob das Bauteil ausgebaut zum Vorlackieren berücksichtigt wird oder nicht. Bitte beachten Sie, dass dieses Element nur für die Reparaturcodes „Lackieren (L)" und „Montageteil demontiert lackieren (M)" gilt. |

Der Node CalcResultCommon wird mit folgenden Elementen erweitert:

<RepairCalculation><CalcResultCommon>

| Element | Typ | Beschreibung |
| --- | --- | --- |
| <LacquerPriceVersion> | String | Enthält Informationen zur Preisversion der Lackierung. |
| <LacquerPriceDate> | Date | Enthält Informationen zum Einsatzdatum der Lackierung. |

Bitte beachten Sie, dass die oben erwähnte Schnittstellenerweiterung alle Kalkulationsarten
mit dem Datentyp calcResult betreffen wird.

Das Beispiel bezieht sich auf die Kalkulationsart CalcResultCommon für eine Standardkalkulation.

Allerdings sind weitere Kalkulationsarten wie bspw.

- CalcResultGlass (Glaskalkulation)
- CalcResultOptimized (Optimierte Kalkulation)
- CalcResultExtension (Reparaturkostenausweitungs-Kalkulation)
- CalcResultMaintenance (Wartungskalkulation)
- CalcResultSPO (Ersatzteiloptimierungskalkulation)

von den Erweiterungen betroffen.

Weitere Informationen finden Sie in unserem Kompendium unter: ProcedureRelatedParameter, RepairPosition und [CalcResult](#showid/1409 "Kalkulationsergebnisse CalcResult").
