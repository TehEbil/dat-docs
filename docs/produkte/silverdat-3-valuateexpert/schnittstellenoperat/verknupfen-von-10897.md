---
title: "Verknüpfen von Bildern mit Prüfpunkten ändern"
topic_id: "10897"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Funktionen für Sachverständige > Funktionsumfang > Verknüpfen von Bildern mit Prüfpunkten ändern"
---

# Verknüpfen von Bildern mit Prüfpunkten ändern

Mit der Funktion changeLinkImageList verändern Sie die Verknüpfung zwischen den Bildern und Prüfpunkten zu einem bestehenden
Vorgang.

Parameter changeLinkImageList

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| DossierId | Long | Einstiegselement, enthält sämtliche Eingabedaten zum Vorgang | numerisch | x |
| CheckItemList | linkImagesCheckItems | Die zugehörigen Kindelemente enthalten Details zu den Prüfpunkten |  | x |

Element vxs:CheckItemList

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| CheckItem | linkImagesCheckItem | Die zugehörigen Kindelemente enthalten Details zu einem Prüfpunkt |  | x |

Element vxs:CheckItem

| Parameter | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| CheckItemId | Integer | Eindeutige Nummerierung der Prüfpunkte | numerisch | x |
| ImageList | checkItemImages | Die zugehörigen Kindelemente enthalten Details zu den Bildern |  | x |

Element vxs:ImageList

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| Image | checkItemImage | Die zugehörigen Kindelemente enthalten Details zu einem Bild |  | x |

Element vxs:Image

| Parameter | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| ImageId | Integer | Eindeutige Nummerierung der Bilder | numerisch | x |
| ImageComments | String | Bemerkungen |  |  |
| Position | Integer | Position des Bildes |  |  |
