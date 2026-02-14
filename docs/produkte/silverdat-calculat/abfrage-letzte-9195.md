---
title: "Abfrage letzter Preisstand eines Herstellers"
topic_id: "9195"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abfrage letzter Preisstand eines Herstellers"
---

# Abfrage letzter Preisstand eines Herstellers

Die Funktion getLastPriceGenerationByMfr gibt den letzten Preisstand eines Herstellers an.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| manufacturer | Integer, Pflicht | 20 ="Abarth"  40 = "Alfa Romeo"  42 ="Alpina"  43"= "Alpine"  57 = "Aston Martin"  60 = "Audi"  95 = "Barkas"  107 = "Bentley"  130 = "BMW"  145 = "Brilliance"  141 = "Buick"  150 = "Cadillac"  157 = "Caterham"  160 = "Chevrolet"  170 = "Chrysler"  190 = "Citroen"  191 = "Corvette"  194 = "Dacia"  195 = "Daewoo"  210 = "Daihatsu"  230 = "Dodge"  235 = "DS"  277 = "Ferrari"  280 = "Fiat"  285 = "Ford"  340 = "Honda"  345 = "Hyundai"  357 = "Infiniti"  362 = "Isuzu"  365 = "Iveco"  380 = "Jaguar"  390 = "Jeep"  425 = "Kia"  460 = "Lada"  465 = "Lamborghini"  470 = "Lancia"  730 = "Land Rover"  487 = "Lexus"  502 = "Lotus"  522 = "Maserati"  550 = "Mazda"  570" value== "Mercedes-Benz"  70 = "MG Rover"  580 = "MINI"  590 = "Mitsubishi"  225 = "Nissan"  650 = "Opel"  670 = "Peugeot"  895 = "Piaggio (Vespa)"  700 = "Pontiac"  710 = "Porsche"  715 = "Proton"  720 = "Renault"  727 = "Rolls Royce"  740 = "Saab"  790 = "Seat"  800 = "Skoda"  560 = "Smart"  810 = "Ssangyong"  820 = "Subaru"  830 = "Suzuki"  850 = "Tata"  853 = "Tesla"  860 = "Toyota"  865 = "Trabant"  905 = "Volkswagen"  910 = "Volvo"  930 = "Wartburg"  935 = "Westfield"  960 = "Zastava" | Hersteller |
| generation | Integer, Optional | 1 bis 10 | 1 = Die aktuellste Preisstandänderung  10 = Letzter Eintrag in der Historie |
| locale | complexType, optional    country, string  datCountryIndicator, string  language, string |  | [Element locale](../../allgemein/dat-developers-gui/element-locale-1352.md) |

Rückgabe

Als Antwort wird der letzte Preisstand des abgefragten Herstellers zurückgegeben.

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| priceDate | String | Datum des abgeänderten Preisstands |
| generation | Integer | 1 = Die aktuellste Preisstandänderung  10 = Letzter Eintrag in der Historie |
