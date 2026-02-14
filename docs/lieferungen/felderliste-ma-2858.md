---
title: "Felderliste Marktindex"
topic_id: "2858"
breadcrumb: "Datenlieferungen > Satzbeschreibung DAT €uropa-Code > Beschreibung Zusatzelement 1 > Felderliste Marktindex"
---

# Felderliste Marktindex

| Feld | Beschreibung | DB-Feld | Datentyp | Bemerkungen |
| --- | --- | --- | --- | --- |
| DATECode | DAT €uropa-Code® | HTUV\_FZA + HTUV\_HST + HTUV\_HT + HTUV\_UT + HTUV\_UTV | C, fix 15 Ziffern | PK; (Fahrzeugart + Hersteller + Haupttyp + Untertyp + 4-stellige Untertypvariante; jede Komponente bei Bedarf links mit Nullen aufgefüllt) |
| Con | Marktindex | XLAN\_ISO\_LKZ\_2 + HTUC\_UTV\_CNR | C, fix 5 Zeichen | PK; (zweistelliges ISO-Lkz + 3-stellige Nummer) |
| AVCo | Container-AV 1 | HTUN\_AV | N, 5-stellig | kann auch fehlen |
| AVCoB | Container AV-Benennung 1 | HHAV\_BENN | C, 120 Zeichen | kann auch fehlen |
| AVCo | Container-AV 2 | HTUN\_AV | N, 5-stellig | kann auch fehlen |
| AVCoB | Container AV-Benennung 2 | HHAV\_BENN | C, 120 Zeichen | kann auch fehlen |
| AVCo | Container-AV 3 | HTUN\_AV | N, 5-stellig | kann auch fehlen |
| AVCoB | Container AV-Benennung 3 | HHAV\_BENN | C, 120 Zeichen | kann auch fehlen |
| AVCo | Container-AV 4 | HTUN\_AV | N, 5-stellig | kann auch fehlen |
| AVCoB | Container AV-Benennung 4 | HHAV\_BENN | C, 120 Zeichen | kann auch fehlen |
| AVCo | Container-AV 5 | HTUN\_AV | N, 5-stellig | kann auch fehlen |
| AVCoB | Container AV-Benennung 5 | HHAV\_BENN | C, 120 Zeichen | kann auch fehlen |
| AVCo | Container-AV 6 | HTUN\_AV | N, 5-stellig | kann auch fehlen |
| AVCoB | Container AV-Benennung 6 | HHAV\_BENN | C, 120 Zeichen | kann auch fehlen |
| AVCo | Container-AV 7 | HTUN\_AV | N, 5-stellig | kann auch fehlen |
| AVCoB | Container AV-Benennung 7 | HHAV\_BENN | C, 120 Zeichen | kann auch fehlen |
| AVCo | Container-AV 8 | HTUN\_AV | N, 5-stellig | kann auch fehlen |
| AVCoB | Container AV-Benennung 8 | HHAV\_BENN | C, 120 Zeichen | kann auch fehlen |
| AVCo | Container-AV 9 | HTUN\_AV | N, 5-stellig | kann auch fehlen |
| AVCoB | Container AV-Benennung 9 | HHAV\_BENN | C, 120 Zeichen | kann auch fehlen |
| AbJ | Zeitpunkt-Ab-Jahr | HTUC\_BZ\_VON | N, 4-stellig | Jahr 4-stellig |
| AbM | Zeitpunkt-Ab-Monat | HTUC\_BZ\_VON | N, 2-stellig | 1-12 |
| AbBZ | Zeitpunkt-Ab-Bauzeit | HTUC\_BZ\_VON | N, 4-stellig | Ab-Angabe als DAT Bauzeit-Verschlüsselung |
| BisJ | Zeitpunkt-Bis-Jahr | HTUC\_BZ\_BIS | N, 4-stellig | Jahr 4-stellig; kann auch fehlen |
| BisM | Zeitpunkt-Bis-Monat | HTUC\_BZ\_BIS | N, 2-stellig | 1-12; kann auch fehlen |
| BisBZ | Zeitpunkt-Bis-Bauzeit | HTUC\_BZ\_BIS | N, 4-stellig | Bis-Angabe als DAT Bauzeit-Verschlüsselung; kann auch fehlen |
| CoB | Container-Benennung | HTUC\_BENN oder generisch | C, 120 Zeichen |  |
