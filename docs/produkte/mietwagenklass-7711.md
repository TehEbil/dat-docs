---
title: "Mietwagenklasse anhand des DAT €uropa-Code® ermitteln"
topic_id: "7711"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Mietwagenklasse anhand des DAT €uropa-Code® ermitteln"
---

# Mietwagenklasse anhand des DAT €uropa-Code® ermitteln

Mit der Funktion getRentalCarClassbyDATECode ermitteln Sie die zugehörige Mietwagenklasse anhand des DAT €uropa-Code®.

Parameter

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| DATECode | String | DAT €uropa-Code® inklusive Marktindex | 20stellig | X |
| [firstRegistration](#expandblock-7711-d2e393401)\*  Die Differenz "Jahr der Erstzulassung" zur möglichen Bauzeit des Marktindex darf nicht größer als 1 Jahr sein. In der Fahrzeugbewertung kann sonst kein Wert ermittelt werden. | Date | Datum der Erstzulassung | JJJJ-MM-DD  weitere Infos siehe Popup-Fenster | X |

\*weitere Infos siehe Popup-Fenster
