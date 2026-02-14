---
title: "Felderliste Serien- und Sonderausstattungen"
topic_id: "2855"
breadcrumb: "Datenlieferungen > Satzbeschreibung DAT €uropa-Code > Beschreibung Zusatzelement 1 > Felderliste Serien- und Sonderausstattungen"
---

# Felderliste Serien- und Sonderausstattungen

| Feld | Beschreibung | DB-Feld | Datentyp | Bemerkungen |
| --- | --- | --- | --- | --- |
| DATECode | DAT €uropa-Code® | HTUV\_FZA + HTUV\_HST + HTUV\_HT + HTUV\_UT + HTUV\_UTV | C, fix 15 Ziffern | PK; (Fahrzeugart + Hersteller + Haupttyp + Untertyp + 4-stellige Untertypvariante; jede Komponente bei Bedarf links mit Nullen aufgefüllt) |
| AV | Ausstattungsvariante (AV) | HTUA\_AV, HTBU\_AV | N, 5-stellig | PK |
| AbJ | AV-Zeitpunkt-Ab-Jahr | HTBU\_BZ\_VON, HTUT\_BZ\_EWV\_1 | N, 4-stellig | PK; Jahr 4-stellig |
| AbM | AV-Zeitpunkt-Ab-Monat | HTBU\_BZ\_VON, HTUT\_BZ\_EWV\_1 | N, 2-stellig | PK; 1-12 |
| SoSe | Kennzeichen Sonder/Serie | HTBU\_KZ\_SONDER | C, fix 1 Zeichen | S (Serienausstattung) oder X (Sonderausstattung) |
| AbBZ | AV-Zeitpunkt-Ab-Bauzeit | HTBU\_BZ\_VON, HTUT\_BZ\_EWV\_1 | N, 4-stellig | Ab-Angabe als DAT-Bauzeit-Verschlüsselung |

PK (Primary Key) bedeutet: Teil der eindeutigen Identifizierung des Datensatzes.
