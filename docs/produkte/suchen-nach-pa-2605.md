---
title: "Suchen nach Partnern"
topic_id: "2605"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Auflisten von Informationen innerhalb einer Kundennummer > Suchen nach Partnern"
---

# Suchen nach Partnern

Über die Funktion searchForPartners lassen sich Partnerwerkstätten anzeigen, die zusätzlich nach Markenwerkstatt, Hersteller
Reparatur oder dem Ort weiter eingeschränkt werden können.

Die nummerischen Werte der Fahrzeughersteller sind in der Auflistung der Hersteller zu finden.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| network | Networktype | VW, Nissan.... | Netzwerk in dem der Partner interagiert | X |
| rolePartner | String | REPAIRER, MANUFACTURER, INSURER, EXPERT | Rolle des Partners | X |
| brandSearchCriteria | BrandSearch | 230 | Fahrzeughersteller (Nummerisch) |  |
| textSearchCriteria | String |  | Freitextsuche |  |
| location | Location |  | Ort des Partners |  |
| distanceCalculationMode | String | DRIVING\_DISTANCE, AS\_THE\_CROW\_FLIES | Art der Entfernung    DRIVING\_STISTANCE = Gefahrene Fahrtstrecke  AS\_THE\_CROW\_FLIES = Luftlinie |  |

Rückgabe

Liste der gesuchten Partnern inklusive der reparierenden Hersteller
