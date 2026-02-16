---
title: "Integration der SVG-Dateien"
topic_id: "1638"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > SVG in den DAT Anwendungen > Implementation > Integration der SVG-Dateien"
---

# Integration der SVG-Dateien

Bei der Implementation von SVG-Dateien in die eigene Anwendung benötigt man verschiedene Ereignisbehandlungsroutinen,
die Aktionen in der Benutzeroberfläche abfangen und mit Ereignissen versehen. Da die
SVG-Dateien zum großen Teil Explosionsgrafiken des Fahrzeuges darstellen, sollte z. B.
das Überfahren des Bildes mit dem Cursor dazu führen, dass das jeweilige Einzelteil
(farblich) hervorgehoben wird. Event-Handling kann durch Anklicken des Bildes oder
einzelner Teile erfolgen oder durch Überfahren mit dem Cursor.

Bitte lesen Sie die Kapitel [Wurzelelement svg](wurzelelement-1611.md), [Element constructionGroup](element-constr-1612.md), [Element g](element-g-1616.md) und [Element metadata](element-metada-1620.md), um eine Übersicht zu erhalten, welche Werte Sie auslesen und mit einem Event-Handling
verknüpfen können.
