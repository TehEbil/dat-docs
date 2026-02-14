---
title: "Verknüpfungen von Bildern mit Prüfpunkten holen"
topic_id: "10895"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Funktionen für Sachverständige > Funktionsumfang > Verknüpfungen von Bildern mit Prüfpunkten holen"
---

# Verknüpfungen von Bildern mit Prüfpunkten holen

Mit der Funktion getLinkImageList holen Sie die Verknüpfungen zwischen Bildern und Prüfpunkten zu einem bestehenden
Vorgang, indem sie Parameter CheckItemId und dem Parameter ImageId angeben.

Parameter getLinkImageList

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| DossierId | Long | Einstiegselement, enthält sämtliche Eingabedaten zum Vorgang |  | x |
| CheckItemList | linkImagesCheckItems | Enthält 0 bis n Positionen vxs:CheckItem als Unterelemente |  | x |

Element vxs:CheckItemList

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| CheckItem | linkImagesCheckItem | Die zugehörigen Kindelemente enthalten Details zu einem Prüfpunkt |  | x |

Element vxs:CheckItem

| Parameter | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| CheckItemId | Long | Eindeutige Nummerierung der Prüfpunkte |  | x |
| ImageList | checkItemImages | Enthält 0 bis n Positionen vxs:Image als Unterelemente |  | bedingt |

Element vxs:ImageList

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| Image | checkItemImage | Die zugehörigen Kindelemente enthalten Details zu einem Bild |  | bedingt |

Element vxs:Image

| Parameter | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| ImageId | Long | Eindeutige Nummerierung der Bilder |  | bedingt |
