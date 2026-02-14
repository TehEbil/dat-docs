---
title: "Abruf aller vorhandenen Preisständen eines Vorgangs"
topic_id: "18651"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > Abruf aller vorhandenen Preisständen eines Vorgangs"
---

# Abruf aller vorhandenen Preisständen eines Vorgangs

Die Funktion getContractPriceGenerations() gibt die vorhandenen Preisstände eines Vorgangs zurück.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| contractID | Long, Pflicht |  | Vorgangsnummer |

Rückgabe

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| priceDate | priceDate |  |
| date | String | Datum des abgeänderten Preisstands |
| generation | Integer | 1= Die aktuellste Preisstandänderung  10= Letzter Eintrag in der Historie |
