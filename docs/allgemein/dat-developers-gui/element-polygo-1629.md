---
title: "Element polygon"
topic_id: "1629"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > SVG in den DAT Anwendungen > Dokumentstruktur SVG > Wurzelelement svg > Geometrische Zeichenelemente und -pfade > Element polygon"
---

# Element polygon

###### Element polygon Polygon-Elemente definieren einen Verbund von geraden Liniensegmenten. Im Regelfall stellen sie geschlossene Formen dar. Polygon-Elemente werden hauptsächlich in Pixelgraphiken zum Zeichnen benutzt. Mit einem Polygon-Element oder Polyline-Element kann man nur einen Linienzug malen, beim Path-Element können eine beliebige Anzahl von offenen und geschlossenen Linienzügen zu einem Pfad kombiniert werden. Der Unterschied zu einem Polyline ist, dass ein Polygon eine geschlossene Form darstellt. Wenn der erste und der letzte Polygon-Punkt nicht übereinanderpassen, wird die Form automatisch geschlossen. Beispiel ``` <polygon stroke="#FFFFFF" stroke-width="0.01" points="0.005 0.005 83.868 0.005 83.868  137.331 0.005 137.331 0.005 0.005" /> ```
