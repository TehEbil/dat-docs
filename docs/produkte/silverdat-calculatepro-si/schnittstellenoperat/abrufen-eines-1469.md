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
| locale | Locale, optional |  | [Element locale](../../../allgemein/dat-developers-guide/arbeiten-mit-den-web/element-locale-1352.md) |

Rückgabe

Als Antwort wird das angefragte Dossier zurückgegeben.

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| [Dossiers](../../../vxs/aktenzeichenvo-1369.md) | [Dossiers](../../../vxs/aktenzeichenvo-1369.md) | Enthält das Berechnungsergebnis inklusive aller sonstigen Fahrzeuginformationen. |
