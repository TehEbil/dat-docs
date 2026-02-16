---
title: "SVG in den DAT Anwendungen"
topic_id: "1551"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > SVG in den DAT Anwendungen"
---

# SVG in den DAT Anwendungen

Die DAT verwendet in verschiedenen Anwendungen sowohl Pixel- als auch Vektorgrafiken
für Grafik. Diese Grafiken stellen wir als SVG-Dateien zur Verfügung.

Was ist SVG?

SVG, oder Scalable Vektor Graphics, ist die vom World Wide Web Consortium (W3C) empfohlene
Spezifikation zur Beschreibung zweidimensionaler Vektorgrafiken. SVG ist eine XML-basierte,
textorientierte Auszeichnungssprache. SVG verbindet, Vektorgrafiken, Pixelgrafiken
(jpeg, png etc.) und Text zu grafischen Objekten. SVG-Grafiken sind gut skalierbar.

SVG-Dateien tragen die Endung .svg. SVG-Quelltexte sind reine ASCII-Textdokumente,
die geometrische Objekte durch Markup-Befehle beschreiben. SVG-Support-Stil Sprachen
(z. B. CSS) und Skriptsprachen (z. B. JavaScript, ECMAScript); So ist es möglich,
Interaktion (Maus über etc.) zu definieren.

Die Darstellung der Grafiken erfolgt durch sogenannte user agents. Das sind in der Regel Browser, Browser-Plugins oder eigenständige SVG-Viewer. Ein
SVG user agent kann eine SVG-Datei direkt am Bildschirm darstellen.

Unter <http://caniuse.com/svg> können Sie erfahren, ob die von Ihnen genutzte Browserversion SVG unterstützt.

Manche Webbrowser können ohne nachträgliche Installation von Erweiterungen einen Großteil
des Sprachumfangs darstellen.

Vektorgrafik versus Pixelgrafik

Eine Vektorgrafik enthält im wesentlichen Linien- und Kurveninformationen, die durch
Vektoren definiert werden.

Eine Pixelgrafik (=Rastergrafik) speichert Bilder in einem Farbraster in einer Vielzahl
von quadratischen Bildpunkten (=Pixel).
