---
title: "Element constructionGroup"
topic_id: "1612"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > SVG in den DAT Anwendungen > Dokumentstruktur SVG > Wurzelelement svg > Element constructionGroup"
---

# Element constructionGroup

Das Element constructionGroup wird in einer SVG-Datei ein Mal dargestellt. Das Element enthält Angaben über den DAT Basiscode und die Baugruppe. Diese Informationen mappen die SVG-Grafik mit der entsprechenden DAT-Baugruppe:

| Element | Beschreibung | Datentyp |
| --- | --- | --- |
| fza | Fahrzeugart | byte |
| hst | Hersteller | short |
| ht | Haupttyp | byte |
| constructionGroupId | Baugruppen-ID | byte |
| lkz | ISO-Länderkennzeichen | string |

Beispiel

```
<dat:constructionGroup>
    <dat:fza>1</dat:fza>
    <dat:hst>225</dat:hst>
    <dat:ht>32</dat:ht>
    <dat:constructionGroupId>4</dat:constructionGroupId>
    <dat:lkz>D</dat:lkz>
</dat:constructionGroup>
```
