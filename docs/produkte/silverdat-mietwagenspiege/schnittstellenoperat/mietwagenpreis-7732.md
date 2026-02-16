---
title: "Mietwagenpreise anhand des DAT €uropa-Code® und PLZ ermitteln"
topic_id: "7732"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Mietwagenpreise anhand des DAT €uropa-Code® und PLZ ermitteln"
---

# Mietwagenpreise anhand des DAT €uropa-Code® und PLZ ermitteln

Mit der Funktion getRentalOffersbyDATECode ermitteln Sie die Mietwagenpreise anhand des DAT €uropa-Code® und der Postleitzahl.

Parameter

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| DATECode | String | DAT €uropa-Code® inklusive Marktindex | 20stellig | X |
| firstRegistration\*  Die Differenz "Jahr der Erstzulassung" zur möglichen Bauzeit des Marktindex darf nicht größer als 1 Jahr sein. In der Fahrzeugbewertung kann sonst kein Wert ermittelt werden. | Date | Erstzulassungsdatum | JJJJ-MM-DD  weitere Infos siehe Popup-Fenster | X |
| beginnigOfRental | Date | Beginndatum der Vermietung | numerisch [firstRegistration+50 Jahre]  JJJJ-MM-DD |  |
| endOfRental | Date | Enddatum der Vermietung | numerisch [firstRegistration+50 Jahre]  JJJJ-MM-DD |  |
| duration | Integer | Leihdauer in Tagen. Wenn der Mietbeginn und das Mietende angegeben worden sind, müssen diese Werte mit der Leihdauer übereinstimmen. | numerisch [1-30] |  |
| postalCode | Integer | Postleitzahl des Suchgebiets |  | X |
| radius | Integer | Radius für Umkreis | numerisch [1-40] |  |

\*weitere Infos siehe Popup-Fenster
