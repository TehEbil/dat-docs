---
title: "Abrufen eines bestimmten Vorgangs"
topic_id: "1469"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abrufen eines bestimmten Vorgangs"
---

# Abrufen eines bestimmten Vorgangs

Die Funktion getContract() gibt den angegebenen Vorgang als Dossier zurück, es kann gesteuert werden, ob hier
auch das Protokoll mit ausgegeben werden soll.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| contractID | Long, Pflicht |  | Vorgangsnummer |
| includeProtocol | Boolean, optional | true / false | Soll das Protokoll inkludiert werden? |
| includeAttachments | Boolean, optional | true / false | Kennzeichen, ob Anhänge exportiert werden sollen |
| locale | Locale, optional |  | [Element locale](#showid/1352 "Element locale ") |

Rückgabe

Als Antwort wird das angefragte Dossier zurückgegeben.

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| [Dossiers](#showid/1369 "Aktenzeichen/Vorgänge (Dossiers)") | [Dossiers](#showid/1369 "Aktenzeichen/Vorgänge (Dossiers)") | Enthält das Berechnungsergebnis inklusive aller sonstigen Fahrzeuginformationen. |
