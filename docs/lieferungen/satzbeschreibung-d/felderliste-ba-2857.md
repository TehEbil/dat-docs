---
title: "Felderliste Bauzeitraum"
topic_id: "2857"
breadcrumb: "Datenlieferungen > Satzbeschreibung DAT €uropa-Code > Beschreibung Zusatzelement 1 > Felderliste Bauzeitraum"
---

# Felderliste Bauzeitraum

| Feld | Beschreibung | DB-Feld | Datentyp | Bemerkungen |
| --- | --- | --- | --- | --- |
| DATECode | DAT €uropa-Code® | HTUV\_FZA + HTUV\_HST + HTUV\_HT + HTUV\_UT + HTUV\_UTV | C, fix 15 Ziffern | PK; (Fahrzeugart + Hersteller + Haupttyp + Untertyp + 4-stellige Untertypvariante; jede Komponente bei Bedarf links mit Nullen aufgefüllt) |
| AbJ | Zeitpunkt-Ab-Jahr | HTUT\_BZ\_EWV\_1, HTBU\_BZ\_VON | N, 4-stellig | Jahr 4-stellig |
| AbM | Zeitpunkt-Ab-Monat | HTUT\_BZ\_EWV\_1, HTBU\_BZ\_VON | N, 2-stellig | 1-12 |
| BisJ | Zeitpunkt-Bis-Jahr | MSUT\_BJ\_BIS | N, 4-stellig | Jahr 4-stellig; kann auch fehlen |
| BisM | Zeitpunkt-Bis-Monat | MSUT\_BJ\_BIS | N, 2-stellig | 1-12; kann auch fehlen |
| AbBZ | Zeitpunkt-Ab-Bauzeit | HTUT\_BZ\_EWV\_1, HTBU\_BZ\_VON | N, 4-stellig | Ab-Angabe als DAT-Bauzeit-Verschlüsselung |
| BisBZ | Zeitpunkt-Bis-Bauzeit | MSUT\_BJ\_BIS | N, 4-stellig | Bis-Angabe als DAT-Bauzeit-Verschlüsselung; kann auch fehlen |

PK (Primary Key) bedeutet: Teil der eindeutigen Identifizierung des Datensatzes.
