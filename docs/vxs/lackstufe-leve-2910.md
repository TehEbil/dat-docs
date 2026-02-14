---
title: "Lackstufe Level"
topic_id: "2910"
breadcrumb: "Datenaustauschformat VXS > Wertelisten > Lackstufe Level"
---

# Lackstufe Level

| Wert | Beschreibung |
| --- | --- |
| 1 | Oberflächenlackierung |
| 2 | Reparaturlackierung bis 50 Prozent |
| 3 | Reparaturlackierung über 50 Prozent |
| 4 | Neuteillackierung |
| 5 | Lackstufe 5 (speziell bei Kunststoffteilen) |
| 0 | keine Lackierung (Lackunterdrückung für Einzelposition; nur in DATRKADV) |
| \* | alle Lackstufen (nur bei Bedingungs-Lackstufen) |
| # | alle Lackstufen kleiner/gleich der vorgegebenen Lackstufe (nur bei Bedingungs-Lackstufen) |
| A | Lackstufe wird ersetzt durch Reparaturcode A (nur bei Umfasst- und Umfasst-Nicht-Bedingungs-Lackstufen, wird ersetzt durch eignes RC-Feld) |
| E | Lackstufe wird ersetzt durch Reparaturcode E (nur bei Umfasst-Nicht-Bedingungs-Lackstufen, wird ersetzt durch eigenes RC-Feld) |
| Z | Lackstufe wird ersetzt durch Reparaturcode Z (nur bei Umfasst-Nicht-Bedingungs-Lackstufen, wird ersetzt durch eigenes RC-Feld) |
| Blank | Keine Lackstufe hinterlegt (wenn das entsprechende Feld NULL-fähig ist, statt Blank NULL) |

Eurolack

| DAT-Lackstufe (Level) | Lackstufenbezeichnung (WorkNumber) (DLFP-Text) | |
| --- | --- | --- |
|  | Metallteil | Kunststoffteil |
| 1 | OBERFLÄCHE | OBERFLÄCHE-K |
| 2 | INSTANDSETZUNG | INSTANDSETZUNG |
| 3 | INSTANDSETZUNG | NEUTEIL-K-V |
| 4 | NEUTEIL-M/-S/-P | NEUTEIL-K-R |
| 5 | -- | NEUTEIL-K-N |

AZT

| DAT-Lackstufe (Level) | Lackstufenbezeichnung (WorkNumber) | |
| --- | --- | --- |
|  | Metallteil | Kunststoffteil |
| 1 | OBERFLÄCHE ST.II | OBERFLÄCHE K2 |
| 2 | REP.-LACK ST.III | REP.-LACK K3 |
| 3 | REP.-LACK ST.IV | NEUTEIL K1R |
| 4 | NEUTEIL ST.I-M/-S | NEUTEIL K1G |
| 5 | -- | NEUTEIL K1N |

Herstellerlack

| DAT-Lackstufe (Level) | Lackstufenbezeichnung (WorkNumber) |
| --- | --- |
|  | Metallteil und Kunststoffteil |
| 1 | je nach Hersteller Text aus DLWE |
| 2 | je nach Hersteller Text aus DLWE |
| 3 | je nach Hersteller Text aus DLWE |
| 4 | je nach Hersteller Text aus DLWE |
| 5 | je nach Hersteller Text aus DLWE |
