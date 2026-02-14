---
title: "Element image"
topic_id: "1615"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > SVG in den DAT Anwendungen > Dokumentstruktur SVG > Wurzelelement svg > Element image"
---

# Element image

Das Element image ist nur in SVG-Dokumenten mit Pixelgrafik enthalten.

Mit dem Element image wird die SVG-Grafik als Bild in das Dokument eingebunden. Durch das URI-Schema werden die Daten
so in den Quelltext eingebettet, als wären es externe Ressourcen. Das Element image ist in einer SVG-Datei genau einmal. Es enthält die folgenden Attribute:

| Attribut | Beschreibung | Immer vorhanden |
| --- | --- | --- |
| xlink:href | Die Syntax ist im Regelfall wie folgt:  data:[<MIME-Typ>][;charset="<Zeichensatz>"][;base64],<Image in base64 Codierung> | X |
| x / y | X- und Y-Achse, gemessen von der oberen linken Ecke des Images; default ist 0 |  |
| height | Die Höhe des Images | X |
| width | Die Breite des Images | X |
| id | Der Identifizierer des Images | X |

Beispiel

```
<image xlink:href="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAe8AAAMrCAMAAA
BXsep0AAADAFBMVEUAAAAQEBAgICAwMDBAQEBQUFBgYGBwcHB4eHiAgICIiIiYmJioqKi4uLjIyMjY2N
jo6Oj4+PgSEhITExMUFBQVFRUWFhYXFxcYGBgZGRkaGhobGxscHBwdHR0eHh4fHx8gICAhISEi
...
nwDvgHfgG/AN+Ab8A34xjfgG/AN+AZ8A74B34BvwDfgG/AN+AZ84xvwDfgGfAO+Ad+Ab8A34BvwDfgGf
AO+8Q34BnwDvgHfgG/AN+Ab8A34BnwDvgHf+AZ8A74B34BvwDfgG/AN+AZ8A74B34BvfAO+Ad+Ab8A3
4BvwDfgGfAO+Ad+Ab3zzCPAN+AZ8A74B34BvwDfgG/AN+AZ8A77xDfgGfAO+Ad+Ab8A34BvwDfgGfAO+A
d/4BnwDvgHfgG/AN+Ab8A34BnwDvgHfgO+/mP8DZ9m94dIYHR4AAAAASUVORK5CYII="
 x="0" y="0" width="83.868" height="137.331" id="pcxImageB64" />
```
