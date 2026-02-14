---
title: "Element path"
topic_id: "1626"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > SVG in den DAT Anwendungen > Dokumentstruktur SVG > Wurzelelement svg > Geometrische Zeichenelemente und -pfade > Element path"
---

# Element path

###### Element path Path-Elemente definieren den Umriss einer graphischen Gestalt. Mathematisch gesehen sind Path-Elemente ein Zusammenschluss von Polygon, Polyline und Line-Elementen. Über das spezifische Attribut "d" werden die Pfaddaten übergeben. Die Pfaddaten bestehen aus Kommandos und lokalen Koordinaten. Außerdem können in diesem Element die Attribute id und [style-Angaben](#showid/1625 "Style-Angaben in geographischen Elementen") benutzt werden. Durch die Angabe des Attributes id wird die Zuordnung eines Path-Elementes zu einem Gruppenelement gekennzeichnet. Beispiele ``` <!-- hier werden die Attribute id und style verwendet--> <path d="M 78.00436849813843,129.07366523706054 L 81.8680056928711,129.07366523706054  L 81.8680056928711,135.3309765649414 L 78.00436849813843,135.3309765649414  L 78.00436849813843,129.07366523706054 Z" id="path2914" style="fill: rgb(40, 87, 155);  fill-opacity: 1; fill-rule: nonzero; stroke: none;" /> ``` ``` <!-- hier werden die style-Attribute direkt verwendet--> <path stroke="#FFFFFF" fill="#FFFFFF" stroke-width="0.12"  d="M 11.035239999999995,56.83644400000001  11.035239999999995,56.72735300000001 11.0679673,56.749171200000006 11.0679673,56.8146258 Z" /> ```
