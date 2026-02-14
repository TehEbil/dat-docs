---
title: "Abrufen eines Kalkulationsausdrucks"
topic_id: "2609"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Abrufen eines Kalkulationsausdrucks"
---

# Abrufen eines Kalkulationsausdrucks

Mit dieser Funktion kann anhand der übergebenen Auftrags ID, der Kalkulationsausdruck
eines Vorgangs heruntergeladen werden.

Falls der Parameter reportIdentification gesetzt wurde, wird die Kalkulation in der entsprechenden benutzerdefinierte Vorlage
zurückgegeben, andernfalls über die standard Vorlage.

Der Kalkulationsausdruck ist nur verfügbar wenn der Vorgang kalkuliert wurde und das
Recht zum Lesen der Kalkulation vorhanden ist.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| contractId | Long |  | ID des Auftrags | X |
| reportIdentification | String |  | Optionaler Identifier einer benutzerdefinierten Vorlage |  |
| attributes |  | <isWithEquipment>true</isWithEquipment>  <isNetto>true</isNetto>  <isWithNewPrices>true</isWithNewPrices> | isWithEquipment = inkl. Austattungsliste  isNetto= Netto  isWithNewPrices = inkl. Listenneupreise |  |

Rückgabe

Druckvorlage des Auftrags
