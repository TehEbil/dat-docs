---
title: "Beschreibung getRentalOffersbyDATECodeResponse"
topic_id: "14955"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Mietwagenpreise anhand des DAT €uropa-Code® und PLZ ermitteln > Beschreibung getRentalOffersbyDATECodeResponse"
---

# Beschreibung getRentalOffersbyDATECodeResponse

Elemente getRentalOffersbyDATECodeResponse

| Name | Datentyp | Beschreibung | Schreibweise |
| --- | --- | --- | --- |
| RentalVehicleOffersResponse | rentalVehicleOffersResponse | enthält Unterelemte mit Mietangeboten |  |

Elemente RentalVehicleOffersResponse

| Name | Datentyp | Beschreibung | Schreibweise |
| --- | --- | --- | --- |
| CDWAverageDeductible | Decimal | Kosten der durchschnittlichen Selbstbeteiligung bei der Vollkaskoversicherung (CDW) |  |
| Offers | offersData | enthält Unterelemte mit Mietangeboten |  |
| rentalOffersNumber | Integer | Anzahl der Mietangebote/Filialen in der angegeben Umgebung |  |

Elemente Offers

| Name | Datentyp | Beschreibung | Schreibweise |
| --- | --- | --- | --- |
| CurrencyType | String | Währung | EUR |
| Max | Decimal | Maximalste Kosten |  |
| Mean | Decimal | Durchschnittliche Kosten |  |
| Min | Decimal | Niedrigeste Kosten |  |
| OffersType | String | Kosten für ein Tag oder Kosten für 3 Tage oder Kosten für eine Woche |  |
| PriceType | String | GROSS = Brutto |  |
