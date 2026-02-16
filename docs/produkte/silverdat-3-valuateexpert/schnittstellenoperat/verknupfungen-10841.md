---
title: "Verknüpfungen von Bildern mit Prüfpunkten löschen"
topic_id: "10841"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Funktionen für Sachverständige > Funktionsumfang > Verknüpfungen von Bildern mit Prüfpunkten löschen"
---

# Verknüpfungen von Bildern mit Prüfpunkten löschen

Mit der Funktion deleteLinkImageList löschen Sie die Zuordnung der Bildinformationen zu den Prüfpunkten aus einem bestehenden
Vorgang.

Parameter deleteLinkImageList

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| DossierId | Long | Eindeutige Vorgangskennung |  | x |
| CheckItemList | deleteLinkImagesCheckItems | Enthält 0 bis n Positionen vxs:CheckItem als Unterelement |  | x |

Element vxs:CheckItemList

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| CheckItem | deleteLinkImagesCheckItem | Die zugehörigen Kindelemente enthalten Details zu einem Prüfpunkt |  | x |

Element vxs:CheckItem

| Parameter | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| CheckItemId | Long | Eindeutige Nummerierung der Prüfpunkte |  | x |
| ImageList | deleteImageLinksImageList | Enthält 0 bis n Positionen vxs:Image als Unterelement |  | x |

Element vxs:ImageList

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| Image | deleteImageLinksImage | Die zugehörigen Kindelemente enthalten Details zu einem Bild |  | x |

Element vxs:Image

| Parameter | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| ImageId | Long | Eindeutige Nummerierung der Bilder |  | x |
