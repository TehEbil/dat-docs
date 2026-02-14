---
title: "Felderliste AV-Stammdaten"
topic_id: "2856"
breadcrumb: "Datenlieferungen > Satzbeschreibung DAT €uropa-Code > Beschreibung Zusatzelement 1 > Felderliste AV-Stammdaten"
---

# Felderliste AV-Stammdaten

| Feld | Beschreibung | DB-Feld | Datentyp | Bemerkungen |
| --- | --- | --- | --- | --- |
| FZA | Fahrzeugart | HHAV\_FZA | N, 2-stellig | PK |
| HST | Hersteller | HHAV\_HST | N, 3-stellig | PK |
| AV | Ausstattungsvariante (AV) | HHAV\_AV | N, 5-stellig | PK |
| AVB | AV-Benennung | HHAV\_BENN | C, 120 Zeichen |  |
| AVBl | AV-Langbenennung | HHAV\_BENN\_LANG | C, 600 Zeichen | nur manchmal vorhanden |
| AVKlf | Klassifizierung der Ausstattungsvariante | HHAV\_AV\_KLF | N, bis 5-stellig | Kann fehlen |
| AVGrp | AV-Gruppe | XMAG\_AG\_KUERZEL | C, 4 Zeichen | nur teilweise vorhanden |
| AVGrpB | AV-Gruppe-Benennung | XMAG\_BENN | C, 40 Zeichen | nur teilweise vorhanden |

PK (Primary Key) bedeutet: Teil der eindeutigen Identifizierung des Datensatzes.
