---
title: "Style-Angaben in geographischen Elementen"
topic_id: "1625"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > SVG in den DAT Anwendungen > Dokumentstruktur SVG > Wurzelelement svg > Geometrische Zeichenelemente und -pfade > Style-Angaben in geographischen Elementen"
---

# Style-Angaben in geographischen Elementen

###### Style-Angaben in geographischen Elementen In unseren SVG-Dateien können unterschiedliche Styling-Formen vorkommen, um die geometrischen Zeichenelemente darzustellen. - Jedes Element kann das style-Attribut direkt verwenden: ``` <rect style="stroke:black;fill:yellow" x="20" y="30" width="300" height="200" rx="10" ry="10" /> <rect style="stroke:red; fill:none" x="20" y="330" width="300" height="200" rx="10" ry="10" /> </svg> ``` - Alternativ dazu kann die Darstellung eines Elements auch direkt über die Rendering-Attribute erfolgen: ``` <rect x="20" y="30" width="300" height="200" rx="10" ry="10" fill="yellow" stroke="black" /> <rect stroke="red" fill="none" x="20" y="330" width="300" height="200" rx="10" ry="10" /> ``` Jede Eigenschaft kann als Teil eines style-Attribut definiert werden. Sie kann dem Element auch direkt zugewiesen werden. Die Auswirkungen auf das Element sind in beiden Fällen gleich. Ist einem Element ein Styling-Attribut direkt zugewiesen, kann es durch ein Stylesheet überschrieben werden. Wenn Sie SVG-Grafiken mit eigenen Stylings versehen, sollten Sie Stylesheets verwenden. Sie überschreiben so direkt zugewiesene style-Attribute in Elementen.
