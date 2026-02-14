---
title: "Felderliste DAT €uropa-Code Teil 1 zu den Fahrzeugauswahldaten (KBA-Ebene)"
topic_id: "2851"
breadcrumb: "Datenlieferungen > Satzbeschreibung DAT €uropa-Code > Beschreibung DAT €uropa-Code Teil 1 > Felderliste DAT €uropa-Code Teil 1 zu den Fahrzeugauswahldaten (KBA-Ebene)"
---

# Felderliste DAT €uropa-Code Teil 1 zu den Fahrzeugauswahldaten (KBA-Ebene)

| Feld | Beschreibung | DB-Feld | Datentyp | Bemerkungen |
| --- | --- | --- | --- | --- |
| FZA | Fahrzeugart | HTUT\_FZA | N, 2-stellig | PK |
| HST | Hersteller | HTUT\_HST | N, 3-stellig | PK |
| HT | Haupttyp | HTUT\_HT | N, 3-stellig | PK |
| UT | Untertyp | HTUT\_UT | N, 3-stellig | PK |
| AVMo | Motor-AV | MSUT\_AV\_MOTOR | N, 5-stellig | PK (kann aber auch fehlen) |
| AVKa | Karosserie-AV | MSUA\_AV | N, 5-stellig | PK (kann aber auch fehlen); HHAV\_AV\_KLF=2; nicht bei FZA 4 – LKW und 5 – Omnibus |
| HSN | KBA-HSN | MDKB\_KBA\_HST\_SC | C, fix 4 Zeichen | PK |
| TSN | KBA-TSN | MDKB\_KBA\_TYP\_SC | C, fix 3 Zeichen | PK |
| FZAB | Fahrzeugart-Benennung | HHFA\_BENN | C, 30 Zeichen |  |
| HSTB | Hersteller-Benennung | HHST\_BENN | C, 30 Zeichen |  |
| HTB | Haupttyp-Benennung | HTHT\_BENN | C, 60 Zeichen |  |
| UTB | Untertyp-Benennung | HTUT\_BENN | C, 60 Zeichen |  |
| AVMoB | Motor AV-Benennung | HHAV\_BENN | C, 120 Zeichen | kann auch fehlen |
| AVKaB | Karosserie AV-Benennung | HHAV\_BENN | C, 120 Zeichen | kann auch fehlen; nicht bei FZA 4 – LKW und 5 – Omnibus |
| CCM | CCM | XKBA\_CCM | N, 9-stellig |  |
| KW | Kilowatt | XKBA\_KILOWATT | N, ####,## |  |
| TKlH | Typklasse Haftpflicht (neu) | XKBA\_TKL\_HAFT\_N | C, 2 Zeichen | nur bei FZA 1 – PKW und teilweise bei FZA 2 – Transporter |
| TKlT | Typklasse Teilkasko (neu) | XKBA\_TKL\_TEIL\_N | C, 2 Zeichen | nur bei FZA 1 – PKW und teilweise bei FZA 2 – Transporter |
| TKlV | Typklasse Vollkasko (neu) | XKBA\_TKL\_VOLL\_N | C, 2 Zeichen | nur bei FZA 1 – PKW und teilweise bei FZA 2 – Transporter |

PK (Primary Key) bedeutet: Teil der eindeutigen Identifizierung des Datensatzes.
