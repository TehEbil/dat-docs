---
title: "Mietwagenpreise anhand der Mietwagenklasse und PLZ ermitteln"
topic_id: "7739"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Mietwagenpreise anhand der Mietwagenklasse und PLZ ermitteln"
---

# Mietwagenpreise anhand der Mietwagenklasse und PLZ ermitteln

Mit der Funktion getRentalOffersbyCarClass ermitteln Sie die Mietwagenpreise anhand der Mietwagenklasse und der Postleitzahl.

Parameter

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| [rentalCarClass](#expandblock-7739-d2e397192)\*  Die DAT hat sämtliche Fahrzeuge im DAT-Fahrzeugbestand in 11 Mietwagenklassen eingestuft. Die Mietwagenklassen wurde dabei definiert durch Fahrzeugkosten und Motorisierung.  Die Mietwagenklassen gehen bei PKW von 1 – 11, bei Transportern von 21 – 31, wobei in der Praxis bei Transportern aufgrund der Preisstrukturen die Klassen 24 – 31 Verwendung finden.  Für jedes Modelljahr, beginnend mit dem Jahr 2003, werden die Klassen anhand der aktuellen Fahrzeugangebote, Preise und Ausstattungskriterien ergänzt, überarbeitet und ggf. angepasst.  Durch die modelljahrbezogene Datenerhebung können die Kosten und Angebotssituationen auch rückblickend ab dem Jahr 2013 ermittelt werden. | Integer | Mietwagenklasse | weitere Infos siehe Popup-Fenster | X |
| beginnigOfRental | Date | Beginndatum der Vermietung | numerisch [aktuelles Datum+50 Jahre]  JJJJ-MM-DD |  |
| endOfRental | Date | Enddatum der Vermietung | numerisch [aktuelles Datum+50 Jahre]  JJJJ-MM-DD |  |
| duration | Integer | Leihdauer in Tagen. Wenn der Mietbeginn und das Mietende angegeben worden sind, müssen diese Werte mit der Leihdauer übereinstimmen. | numerisch [1-30] |  |
| postalCode | Integer | Postleitzahl des Suchgebiets |  | X |
| radius | Integer | Radius für Umkreis | numerisch [1-40] |  |

\*weitere Infos siehe Popup-Fenster
