---
title: "Nutzungsausfalldaten anhand DAT €uropa-Code® ermitteln"
topic_id: "7727"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Nutzungsausfalldaten anhand DAT €uropa-Code® ermitteln"
---

# Nutzungsausfalldaten anhand DAT €uropa-Code® ermitteln

Mit der Funktion getLossOfUseDatabyDATECode bestimmen Sie den Nutzungsausfall anhand des DAT €uropa-Code®.

Parameter

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| DATECode | String | DAT €uropa-Code® inklusive Marktindex | 20stellig | X |
| firstRegistration\*  Die Differenz "Jahr der Erstzulassung" zur möglichen Bauzeit des Marktindex darf nicht größer als 1 Jahr sein. In der Fahrzeugbewertung kann sonst kein Wert ermittelt werden. | Date | Erstzulassung | JJJJ-MM-DD  weitere Infos siehe Popup-Fenster | X |
| beginnigOfRental | Date | Startdatum der Vermietung | numerisch, [firstRegistration+50 Jahre]  JJJJ-MM-DD |  |
| endOfRental | Date | Enddatum der Vermietung | numerisch, [firstRegistration+50 Jahre]  JJJJ-MM-DD |  |

\*weitere Infos siehe Popup-Fenster
