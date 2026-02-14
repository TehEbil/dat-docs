---
title: "Parameter setValueInfluencingFactors"
topic_id: "25287"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Benutzerdefinierte Handelsspanne > Benutzerdefinierte Handelsspanne anlegen > Parameter setValueInfluencingFactors"
---

# Parameter setValueInfluencingFactors

Request setValueInfluencingFactors

| Parameter | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| DossierId | Long | Eindeutige Vorgangskennung | numerisch | X |
| Language | String | Sprachkürzel | Sprachkürzel (Language) Default-Wert = en\_US  | Wert | Beschreibung | | --- | --- | | ca\_ES | Katalanisch Spanien | | cs\_CZ | Tschechisch Tschechien | | de\_AT | deutsch Österreich | | de\_CH | Deutsch Schweiz | | de\_DE | Deutsch Deutschland | | el\_GR | Griechisch Griechenland | | en\_GB | Englisch Grossbrittanien | | en\_US | Englisch USA | | es\_ES | Spanisch Spanien | | fr\_CH | Französisch Schweiz | | fr\_FR | Französisch Frankreich | | hu\_HU | Ungarisch Ungarn | | it\_CH | Italienisch Schweiz | | it\_IT | Italienisch Italien | | nl\_NL | Niederländisch Niederlande | | pl\_PL | Polnisch Polen | | ro\_RO | Rumänisch Rumänien | | ru\_RU | Russisch Russland | | sk\_SK | Slowakisch Slowakei | | tr\_TR | Türkisch Türkei | |  |
| PercentageOfSalesPrice | Decimal | Prozentwert vom Händler-Verkaufswert zur Berechnung der Handelsspanne wird bei Angabe bevorzugt zur weiteren Berechnung verwendet |  |  |
| InPercentageOfSalesPriceNet | Decimal | Handelsspanne in Netto / Manueller Wert wird nicht berücksichtigt, wenn PercentageOfSalesPrice angegeben wurde, aber bevorzugt vor InPercentageOfSalesPriceGross zur weiteren Berechnung verwendet |  |  |
| InPercentageOfSalesPriceGross | Decimal | Handelspanne in Brutto / Manueller Wert wird nicht berücksichtigt, wenn PercentageOfSalesPrice oder InPercentageOfSalesPriceNet angegeben wurden |  |  |
| NominalDaysOnLot | Decimal | Anzahl der Standtage |  |  |
| TonnageClass | String | Tonnage Klasse | a (oder 1) = bis 3,5t Gesamtgewicht b (oder 2) = über 3,5t bis 7,5 Gesamtgewicht c (oder 3) = über 7,5t bis 11t Gesamtgewicht d (oder 4) = über 11t bis 15,9t Gesamtgewicht e (oder 5) = ab 16t Gesamtgewicht | nur bei freien Aktenzeichen für VehicleType = 2 Pflicht |
| VehicleType | Integer | Fahrzeugart | 2 = Lkw 4 = Motorrad 5 = Pkw 6 = Transporter 8 = SUV 90= frei definierte Fahrzeugart | nur bei freien Aktenzeichen Pflicht |
| ValueInfluencingFactorList | ValueInfluencingFactorList | Liste von wertbeeinflussenden Faktoren |  |  |
| MarginFromValueInfluencingFactors | Boolean | Berechnungsmethode der Handelsspanne. | true = Die Handelsspanne wird immer aus den wertbeeinflussenden Faktoren berechnet. false (default) = Falls im Request mindestens einer der Parameter PercentageOfSalesPrice, InPercentageOfSalesPriceNet und InPercentageOfSalesPriceGross gesetzt sind, wird die Handelsspanne aus prozentualem bzw. Sachverständigenwert berechnet, sonst aus den wertbeeinflussenden Faktoren. |  |

Element ValueInfluencingFactorList

| Parameter | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| ValueInfluencingFactorItem | ValueInfluencingFactorItem | wertbeeinflussender Faktor |  | X |

Element ValueInfluencingFactorItem

| Parameter | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| ValueInfluencingFactorId | Long | Id des wertbeeinflussenden Faktors |  | X |
| ValueNet | Decimal | Wert in Netto |  |  |
| ValueGross | Decimal | Wert in Brutto |  |  |
| IntoAccountCheck | Boolean | Angabe, ob der wertbeeinflussende Faktor in der Handelspanne berücksichtigt werden soll | true = wertbeeinflussender Faktor soll berücksichtigt werden false = wertbeeinflussender Faktor soll nicht berücksichtigt werden |  |
| Reset | Boolean | Zurücksetzen eines benutzerdefinierten wertbeeinflussenden Faktors auf DAT-Standard. | true = Wenn für den wertbeeinflussenden Faktor im Request weder ValueNet noch ValueGross übergeben wurde, wird der wertbeeinflussende Faktor auf DAT-Standard zurückgesetzt. false (default) = Der wertbeeinflussende Faktor wird nicht auf DAT-Standard zurückgesetzt. |  |

² siehe Popup Fenster
