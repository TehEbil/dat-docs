---
title: "Abfrage des Bearbeitungsstatus/ -benutzer eines Vorgangs"
topic_id: "2347"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abfrage des Bearbeitungsstatus/ -benutzer eines Vorgangs"
---

# Abfrage des Bearbeitungsstatus/ -benutzer eines Vorgangs

Die Funktion getLockedInfo gibt an, ob ein Vorgang gelockt also sich in Bearbeitung befindet.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| contractID | Long, Pflicht |  | Vorgangsnummer |

Rückgabe

Als Antwort wird der Benutzername vom Anwender, der den Vorgang bearbeitet, zurückgegeben.

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| lockedInfo | String | Benutzerinformation |
