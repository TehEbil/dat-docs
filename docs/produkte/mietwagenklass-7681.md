---
title: "Mietwagenklasse anhand der VIN ermitteln"
topic_id: "7681"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Mietwagenklasse anhand der VIN ermitteln"
---

# Mietwagenklasse anhand der VIN ermitteln

Mit der Funktion getRentalCarClassbyVIN ermitteln Sie die zugehörige Mietwagenklasse entsprechend der Fahrzeug-Identifizierungsnummer
ihres Fahrzeugs.

Parameter

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| VIN | String | Fahrzeug-Identifizierungsnummer | 17stellig, alphanumerisch | X |
| [firstRegistration](#expandblock-7681-d2e392182)\*  Die Differenz "Jahr der Erstzulassung" zur möglichen Bauzeit des Marktindex darf nicht größer als 1 Jahr sein. In der Fahrzeugbewertung kann sonst kein Wert ermittelt werden. | Date | Erstzulassungsdatum | JJJJ-MM-DD  weitere Infos siehe Popup-Fenster | X |

\*weitere Infos siehe Popup-Fenster
