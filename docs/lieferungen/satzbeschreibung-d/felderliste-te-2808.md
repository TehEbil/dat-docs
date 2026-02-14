---
title: "Felderliste Teil 2 zu den im DAT €uropa-Code enthaltenen Ausstattungen"
topic_id: "2808"
breadcrumb: "Datenlieferungen > Satzbeschreibung DAT €uropa-Code > Beschreibung DAT €uropa-Code Teil 2 > Felderliste Teil 2 zu den im DAT €uropa-Code enthaltenen Ausstattungen"
---

# Felderliste Teil 2 zu den im DAT €uropa-Code enthaltenen Ausstattungen

| Feld | Beschreibung | DB-Feld | Datentyp | Bemerkungen |
| --- | --- | --- | --- | --- |
| FZA | Fahrzeugart | HTUV\_FZA | N, 2-stellig |  |
| HST | Hersteller | HTUV\_HST | N, 3-stellig |  |
| HT | Haupttyp | HTUV\_HT | N, 3-stellig |  |
| UT | Untertyp | HTUV\_UT | N, 3-stellig |  |
| DATECode | DAT €uropa-Code® | HTUV\_FZA + HTUV\_HST + HTUV\_HT + HTUV\_UT + HTUV\_UTV | C, fix 15 Ziffern | PK; (Fahrzeugart + Hersteller + Haupttyp + Untertyp + 4-stellige Untertypvariante; jede Komponente bei Bedarf links mit Nullen aufgefüllt) |
| FZAB | Fahrzeugart-Benennung | HHFA\_BENN | C, 30 Zeichen |  |
| HSTB | Hersteller-Benennung | HHST\_BENN | C, 30 Zeichen |  |
| HTB | Haupttyp-Benennung | HTHT\_BENN | C, 60 Zeichen |  |
| UTB | Untertyp-Benennung | HTUT\_BENN | C, 60 Zeichen |  |
| AVMo | Motor-AV | HTUA\_AV | N, 5-stellig | HHAV\_AV\_KLF=1 |
| AVMoB | Motor-AV-Benennung | HHAV\_BENN | C, 120 Zeichen |  |
| AVKa | Karosserie-AV | HTUA\_AV | N, 5-stellig | HHAV\_AV\_KLF=2; nicht bei FZA 4 – LKW und 5 – Omnibus |
| AVKaB | Karosserie AV-Benennung | HHAV\_BENN | C, 120 Zeichen | nicht bei FZA 4 – LKW und 5 – Omnibus |
| AVRa | Radstand-AV | HTUA\_AV | N, 5-stellig | HHAV\_AV\_KLF=3; bei FZA 1 – PKW nur teilweise, nicht bei FZA 3 – Kraftrad |
| AVRaB | Radstand-AV-Benennung | HHAV\_BENN | C, 120 Zeichen | bei FZA 1 - PKW nur teilweise, nicht bei FZA 3 – Kraftrad |
| AVAn | Antriebsart-AV | HTUA\_AV | N, 5-stellig | HHAV\_AV\_KLF=4; bei FZA 1 – PKW nur teilweise, nicht bei FZA 3 – Kraftrad, 4 – LKW und 5 – Omnibus |
| AVAnB | Antriebsart AV-Benennung | HHAV\_BENN | C, 120 Zeichen | bei FZA 1 – PKW nur teilweise, nicht bei FZA 3 – Kraftrad 4 – LKW und 5 – Omnibus |
| AVFa | Fahrerhaus/Fahrzeuglänge-AV | HTUA\_AV | N, 5-stellig | HHAV\_AV\_KLF=5; nur bei FZA 4 – LKW und 5 – Omnibus |
| AVFaB | Fahrerhaus/Fahrzeuglänge AV-Benennung | HHAV\_BENN | C, 120 Zeichen | nur bei FZA 4 – LKW und 5 – Omnibus |
| AVTo | Tonnage-AV | HTUA\_AV | N, 5-stellig | HHAV\_AV\_KLF=6; nur bei FZA 4 – LKW und 5 – Omnibus |
| AVToB | Tonnage AV-Benennung | HHAV\_BENN | C, 120 Zeichen | nur bei FZA 4 – LKW und 5 – Omnibus |
| AVBa | Bauart-AV | HTUA\_AV | N, 5-stellig | HHAV\_AV\_KLF=7; nur bei FZA 4 – LKW und 5 – Omnibus |
| AVBaB | Bauart AV-Benennung | HHAV\_BENN | C, 120 Zeichen | nur bei FZA 4 – LKW und 5 – Omnibus |
| AVFe | Federung-AV | HTUA\_AV | N, 5-stellig | HHAV\_AV\_KLF=8; nur bei FZA 4 – LKW und 5 – Omnibus |
| AVFeB | Federung AV-Benennung | HHAV\_BENN | C, 120 Zeichen | nur bei FZA 4 – LKW und 5 – Omnibus |
| AVAa | Anzahl-Achsen/Antriebsart-AV | HTUA\_AV | N, 5-stellig | HHAV\_AV\_KLF=9; nur bei 4 – LKW und 5 – Omnibus |
| AVAaB | Anzahl-Achsen/Antriebsart AV-Benennung | HHAV\_BENN | C, 120 Zeichen | nur bei FZA 4 – LKW und 5 – Omnibus |
| AVAl | Ausstattungslinie-AV 1 | HTUA\_AV | N, 5-stellig | HHAV\_AV\_KLF=10; nicht bei FZA 3 – Kraftrad, ansonsten nur gelegentlich |
| AVAlB | Ausstattungslinie AV-Benennung 1 | HHAV\_BENN | C, 120 Zeichen | nicht bei FZA 3 – Kraftrad, ansonsten nur gelegentlich |
| AVAl | Ausstattungslinie-AV 2 | HTUA\_AV | N, 5-stellig | HHAV\_AV\_KLF=10; nicht bei FZA 3 – Kraftrad, ansonsten nur gelegentlich |
| AVAlB | Ausstattungslinie AV-Benennung 2 | HHAV\_BENN | C, 120 Zeichen | nicht bei FZA 3 – Kraftrad, ansonsten nur gelegentlich |
| AVAl | Ausstattungslinie-AV 3 | HTUA\_AV | N, 5-stellig | HHAV\_AV\_KLF=10; nicht bei FZA 3 – Kraftrad, ansonsten nur gelegentlich |
| AVAlB | Ausstattungslinie AV-Benennung 3 | HHAV\_BENN | C, 120 Zeichen | nicht bei FZA 3 – Kraftrad, ansonsten nur gelegentlich |
| AVGe | Getriebe-AV | HTUA\_AV | N, 5-stellig | HHAV\_AV\_KLF=11; nicht bei FZA 3 – Kraftrad, 4 – LKW und 5 – Omnibus |
| AVGeB | Getriebe AV-Benennung | HHAV\_BENN | C, 120 Zeichen | nicht bei FZA 3 – Kraftrad, 4 – LKW und 5 – Omnibus |
| CCM | CCM | MSUT\_CCM | N, 9-stellig |  |
| KW | Kilowatt | MSUT\_KILOWATT | N, ####,## |  |
| AZyl | Anzahl Zylinder | MSUT\_ANZ\_ZYL | N, 2-stellig |  |
| Antr | Antrieb | MSAT\_KUERZEL | C, 10 Zeichen | nicht bei FZA 3 – Kraftrad, bei FZA 1 – PKW und 4 – LKW nur teilweise |
| AbFh | Fahrerhausaufbauart | MSAA\_AA\_KUERZEL | C, 10 Zeichen | über MSUT\_AUFBAUA\_FH; nur bei FZA 2 – Transporter und 4 – LKW teilweise |
| Ab | Aufbauart | MSAA\_AA\_KUERZEL | C, 10 Zeichen | über MSUT\_AUFBAUA; nicht bei FZA 3 – Kraftrad |
| ATS | Anzahl Türen / Sitzreihen | MSUT\_ANZ\_TUE\_SI | N, 2-stellig | nicht bei FZA 3 – Kraftrad und 4 – LKW |
| RSt | Radstand | MSUT\_RADSTAND | N, 9-stellig | in mm; bei FZA 1 – PKW nur teilweise, nicht bei FZA 3 – Kraftrad |
| GG | Gesamtgewicht | MSUT\_GES\_GEW | N, 9-stellig | in kg; nur bei FZA 2 – Transporter, 4 – LKW und 5 – Omnibus |
| KSt | Kraftstoffart | MSKA\_KA\_KUERZEL | C, 2 Zeichen | nicht bei FZA 3 – Kraftrad und bei FZA 4 – LKW und 5 – Omnibus nur teilweise |
| KZbewert | DAT €uropa-Code® ist bewertbar | HTUV\_KZ\_FREI | C, 1 Zeichen | 2 Werte möglich: J oder N |
| KZkalk | DAT €uropa-Code® ist kalkulierbar | HTUV\_KZ\_FREI | C, 1 Zeichen | 2 Werte möglich: J oder N |
| KZGlas | Glaskalkulation möglich | HTUT\_KZ\_FREI | C, 1 Zeichen | 2 Werte möglich: J oder N |
| OTG | Obertypgruppe | XMHG\_HT\_GRP\_FM | C, 3 Zeichen |  |
| OTGB | Obertypgruppe-Benennung | XMHG\_BENN | C, 30 Zeichen |  |
