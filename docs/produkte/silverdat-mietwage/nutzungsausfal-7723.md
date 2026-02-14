---
title: "Nutzungsausfalldaten anhand der VIN ermitteln"
topic_id: "7723"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Nutzungsausfalldaten anhand der VIN ermitteln"
---

# Nutzungsausfalldaten anhand der VIN ermitteln

Mit der Funktion getLossOfUseDatabyVIN bestimmen Sie den Nutzungsausfall anhand der Fahrzeug-Identifizierungsnummer ihres
Fahrzeugs.

Parameter

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| VIN | String | Fahrzeug-Identifizierungsnummer | 17stellig, alphanumerisch | X |
| [firstRegistration](#expandblock-7723-d2e394114)\*  Die Differenz "Jahr der Erstzulassung" zur möglichen Bauzeit des Marktindex darf nicht größer als 1 Jahr sein. In der Fahrzeugbewertung kann sonst kein Wert ermittelt werden. | Date | Erstzulassungsdatum | JJJJ-MM-DD  weitere Infos siehe Popup-Fenster | X |
| beginnigOfRental | Date | Beginndatum der Vermietung | numerisch, [firstRegistration+50 Jahre]  JJJJ-MM-DD |  |
| endOfRental | Date | Enddatum der Vermietung | numerisch [firstRegistration+50 Jahre]  JJJJ-MM-DD |  |

\*weitere Infos siehe Popup-Fenster
