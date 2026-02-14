---
title: "DatPosition"
topic_id: "11912"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Manuelle Positionen manualPositions > DatPosition"
---

# DatPosition

DatPosition

| Element | Typ | Beschreibung | Wertebereich |
| --- | --- | --- | --- |
| Country | String, optional | Ländercode |  |
| Price | Decimal, optional | Preis |  |
| Designation | String, optional | Name/Bezeichnung der Position |  |
| PreDamage | Integer, optional | Ist ein Vorschaden vorhanden | 0 = Nein  1 = Ja |
| UsedPart | Integer, optional | Ist es ein gebrauchtes Teil | 0 = Nein  1 = Ja |
| DiscountPercentage | Decimal, optional | Rabatt in Prozent |  |
| Nfa | Decimal, optional | Neu für Alt in Prozent |  |
| Worktime | Decimal, optional | Arbeitszeit |  |
| WorkLevel | Integer, optional | Arbeitsstufe | 0, 1, 2 ,3 |
| WorkType | Integer, optional | Arbeitstyp | 1 = Mechanik  2 = Karosserie  3 = Elektrik  60 = Dellen drücken  50 = Nur Zeit (nur bei RC "E") |
| SupplementDifficulty | Decimal, optional |  |  |
| Location | Integer, optional | Ortsangabe des Schadens | 0  1 = Vorne  2 = Hinten  3 = Oben  4 = Unten  5 = Mittig |
| RepairType | String, optional | Repaircode |  |
| CountLevelS | Integer, optional | Leichte Kunststoffschadenanzahl |  |
| CountLevelM | Integer, optional | Mittlerer Kunststoffschadenanzahl |  |
| CountLevelL | Integer, optional | Schwerer Kunststoffschadenanzahl |  |
| CountLevelGlass | Integer, optional |  |  |
| FlatRateValue | Decimal, optional | Pauschalpreis |  |
| SpotCount | Integer, optional | Hagelschadenanzahl |  |
| LacquerMaterial | Decimal, optional | Lakiermaterialpreis |  |
