---
title: "Verknüpfen von Bildern mit Prüfpunkten anlegen"
topic_id: "10839"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Funktionen für Sachverständige > Funktionsumfang > Verknüpfen von Bildern mit Prüfpunkten anlegen"
---

# Verknüpfen von Bildern mit Prüfpunkten anlegen

Mit der Funktion setLinkImageList verknüpfen Sie Bilder mit dem Prüfpunkt, indem Sie den Parameter CheckItemId mit dem Parameter ImageId verknüpfen.

Parameter setLinkImageList

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| DossierId | Long | Einstiegselement, enthält sämtliche Eingabedaten zum Vorgang | numerisch | x |
| CheckItemList | linkImagesCheckItems | Enthält 0 bis n Positionen vxs:CheckItem als Unterelement |  | bedingt |

Element vxs:CheckItemList

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| CheckItem | linkImagesCheckItem | Die zugehörigen Kindelemente enthalten Details zu einem Prüfpunkt | numerisch | bedingt |

Element vxs:CheckItem

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| CheckItemId | Long | Eindeutige Nummerierung der Prüfpunkte | numerisch | bedingt |
| ImageList | checkItemImages | Enthält 0 bis n Positionen vxs:Image als Unterelement |  | bedingt |

Element vxs:ImageList

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| Image | checkItemImage | Die zugehörigen Kindelemente enthalten Details zu einem Bild |  | bedingt |

Element vxs:Image

| Parameter | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| ImageId | Long | Eindeutige Nummerierung der Bilder | numerisch | bedingt |
| ImageComments | String | Bemerkungen |  |  |
| Position | Integer | Position des Bildes |  |  |
