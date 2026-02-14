---
title: "Wurzelelement svg"
topic_id: "1611"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > SVG in den DAT Anwendungen > Dokumentstruktur SVG > Wurzelelement svg"
---

# Wurzelelement svg

Element svg

Den Anfang der eigentlichen SVG-Datei markiert das Element <svg>. Ab hier beginnt das Wurzelelement des Dokuments, das alle anderen Elemente enthält.
Normalerweise kommt es nur einmal im Dokument vor. Das Root-Element enthält die folgenden
Informationen in seinen Attributen:

- Verwendete Namensräume
- Evtl. verwendete SVG-Version
- Angaben zu graphischen Inhalten und deren Eigenschaften
- ID

Mit diesen Attributen können Sie aus den SVG-Dateien dynamische Inhalte generieren.

- Einfache Animationen direkt
- XML- und CSS-Attribute mit Animationen
- Komplexeres Verhalten oder Interaktion über internes oder externes Skripting

Namensräume

Im Wurzelelement <svg> ist ein eindeutiger Namensraum angegeben:

```
xmlns="http://www.w3.org/2000/svg". 
```

Damit das Format SVG selbst identifizieren. Gegebenenfalls gibt es Angaben zu weiteren Namensräumen, um
weitere, verwendete XML-Formate zu identifizieren. Gebräuchlich in den SVG-Dateien der DAT sind unter anderem noch die Namensräume zur Referenzierung von z.B. Hyperlinks, xmlns:xlink, und Namensräume zur Referenzierung der intern definierten Elemente, xmlns:dat.

```
<svg xmlns="http://www.w3.org/2000/svg" xmlns:dat="http://www.dat.de/sphinx/svg" 
xmlns:xlink="http://www.w3.org/1999/xlink" width="100%" height="100%" viewBox="0 0 83.868 137.331" 
id="miniBlobAsSvg" preserveAspectRatio="xMidYMid meet" zoomAndPan="magnify" version="1.0" 
baseProfile="full" 
contentScriptType="text/ecmascript" contentStyleType="text/css" pointer-events="visible">
```

Attribute von Element svg

In der Regel werden die folgenden Attribute ausgegeben:

| Attribut-Name | Mögliche Werte | Beschreibung |
| --- | --- | --- |
| version | "1.0" | "1.1" | "1.2" | Gibt die SVG Sprachversion der SVG-Datei wieder |
| baseProfile | "none" | "full" | "basic" | "tiny" | Beschreibt das SVG-Sprachprofil, das notwendig ist, um den Inhalt korrekt zu rendern; vorgeschlagener Wert: "full" |
| width / height | 1-100 | Geben die eigentliche Höhe und Breite der Grafik im Dokument an. Unterscheiden sich diese Werte von denen in viewBox, wird die Grafik skaliert dargestellt. Die Angabe erfolgt üblicherweise in %. |
| viewBox | (minx, miny, width, height) | Gibt die Koordinaten wieder, um die Grafik im Dokument darzustellen. Es gibt eine rechteckige Region wieder, in die der darzustellende Inhalt fällt. Die erste Zahl ist der minimale x-Wert, die zweite das minimale y-Wert, die dritte die Breite und die vierte die Höhe. |
| preserveAspectRatio | 'xMinYMin' - die skalierte viewBox wird links oben in den Anzeigebereich eingepaßt.  'xMidYMin' - in x-Richtung wird gegebenenfalls zentriert, in y-Richtung nach oben eingepaßt.  'xMaxYMin' - in x-Richtung wird gegebenenfalls rechts eingepaßt, in y-Richtung oben.  'xMinYMid' - in x-Richtung wird gegebenenfalls links eingepaßt, in y-Richtung zentriert.  'xMaxYMid' - in x-Richtung wird gegebenenfalls rechts eingepaßt, in y-Richtung zentriert.  'xMinYMax' - in x-Richtung wird gegebenenfalls links eingepaßt, in y-Richtung unten.  'xMidYMax'  - in x-Richtung wird gegebenenfalls zentriert, in y-Richtung nach unten eingepaßt.  'xMaxYMax'- in x-Richtung wird gegebenenfalls rechts eingepaßt, in y-Richtung nach unten. | Gibt den Skalierungsgrad wieder, wenn viewBox im Seitenverhältnis nicht zu width/height passt. |
| zoomAndPan | "magnify" | "disabled" | Lautet der Wert des Attributes magnify, ist das Vergrößern und Verkleinern, Rotieren und Verschieben der Grafik erlaubt. Dieser Wert ist default. Steht der Wert auf disabled, ist diese Funktionalität deaktiviert. |
| contentScriptType | "text/ecmascript" | Hier wird die vorausgewählte Skriptsprache angegeben. Nachfolgende Skripte können mit einem einfach <script> eingeleitet werden, sofern sie den gleichen Skripttyp verwenden |
| contentStyleType | "text/css" | voreingestellter Typ für Stilvorlagen; Default ist "text/css"; ehemals MIME-Type. |
| pointer-events | "visible" | Ist nur notwendig in SVG-Dateien mit Pixelgrafiken, um Polygone, die das Attribut "fill:none" besitzen, anklickbar zu machen |
| id |  | Identifizierer der SVG-Grafik |
