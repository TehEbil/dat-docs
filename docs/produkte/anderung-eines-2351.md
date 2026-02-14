---
title: "Änderung eines Preisstands eines Vorgangs"
topic_id: "2351"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Änderung eines Preisstands eines Vorgangs"
---

# Änderung eines Preisstands eines Vorgangs

Mit der Funktion setContractPriceGeneration kann der Preisstand eines Vorgangs geändert werden. Wenn ein Kalkulationsergebnis
bereits existiert wird dieses verworfen.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| contractId | Long, Pflicht |  | Vorgangsnummer |
| generation | Integer, Pflicht | Interval [1-10] | 1= Die aktuellste Preisstandänderung  10= Letzter Eintrag in der Historie    Dieser Wert kann über die Funktion [getContractPriceGenerations](#showid/2343 "Abruf aller vorhandenen Preisständen eines Vorgangs") abgefragt werden. |
| removeResult | Boolean, Optional | true / false | Kalkulationsergebnis löschen? |

Rückgabe

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| dateChanged | Boolean | Änderungsdatum der Überschlägige-Kalkulationswerte |
| resultDeleted | Boolean | Ist der Wert auf true gesetzt, deutet dies darauf hin, dass das bereits existierende Kalkulationsergebnis verworfen wurde. |
