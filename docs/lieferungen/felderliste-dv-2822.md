---
title: "Felderliste DVNs"
topic_id: "2822"
breadcrumb: "Datenlieferungen > Satzbeschreibung DAT €uropa-Code > Beschreibung Zusatzelement 2 > Felderliste DVNs"
---

# Felderliste DVNs

| Feld | Beschreibung | DB-Feld | Datentyp | Bemerkungen |
| --- | --- | --- | --- | --- |
| FZA | Fahrzeugart | HTHT\_FZA | N, 2-stellig | PK |
| HST | Hersteller | HTHT\_HST | N, 3-stellig | PK |
| HT | Haupttyp | HTHT\_HT | N, 3-stellig | PK |
| DVN | Datenverarbeitungs- nummer (DVN) | DTAB\_DVN\_LI, DTAB\_DVN\_RE, DTHD\_DVN, DWHA\_DVN, DWAR\_DVN, DWBS\_DVN, LEHB\_DVN, LLHB\_DVN, LAHB\_DVN | N, 5-stellig | PK |
| DVNB | DVN-Benennung | DTAB\_TH\_DVN\_BENN, DTHD\_BENN, DWHA\_BENN, DWAR\_BENN, DWBS\_BENN, DDVN\_BENN | C, 200 Zeichen |  |
| ET | Ersatzteil vorhanden? |  | b | nur 0 oder 1 möglich. Ausgesagt wird, ob zu der DVN auch Ersatzteile gehören (1) oder nicht (0), da es z.B. auch reine "Arbeits-DVNs" gibt. |
| LT | Lackiertes Teil |  | C | optionales Feld; mögliche Werte:  F = fertig lackiert geliefertes Teil  G = grundiert geliefertes Teil |
| KT | Karosserieteil |  | C | optionales Feld; mögliche Werte:  W = geschweißt  S = geschraubt |
