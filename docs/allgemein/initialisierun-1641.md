---
title: "Initialisierung der SVG-Datei"
topic_id: "1641"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > SVG in den DAT Anwendungen > Implementation > Integration der SVG-Dateien > Initialisierung der SVG-Datei"
---

# Initialisierung der SVG-Datei

In einem onLoad-Event wird die Initialisierung der SVG-Datei vorgenommen. Um mit der SVG-Datei arbeiten zu können, wird das Root Element benötigt, das mit Hilfe des entsprechenden
Namespace identifiziert wird. Gesucht wird erst ab dem [Gruppenelement](#showid/1616 "Element g") "Standardebene".

Im nachfolgenden Beispiel wird allen Elementen, die ein Element <[metadata](#showid/1620 "Element metadata")> besitzen, ein Event-Listener zugewiesen, der auf Anklicken oder Überfahren mit dem
Cursor reagiert.

```
<body onload="init('svg')">
```

```
<script>
var svgns = 'http://www.w3.org/2000/svg';
var datns = 'http://www.dat.de/sphinx/svg';

        function init(svgid){
            var svg = document.getElementById(svgid).contentDocument;
            var elements = svg.getElementsByTagNameNS(svgns, "g");
            for(var idx = 0; idx < elements.length; idx++) {
                var g=elements.item(idx);
                <!-- only those elements having a child "metadata" will get a listener
                if(String(g.id).search(/DATID/) >= 0 && g.id != "DATID_000000" &&
                g.getElementsByTagNameNS(svgns, "metadata").length > 0) {
                        g.onmouseover = group_mouseover;
                        g.onmouseout = group_mouseout;
                        g.onclick = group_click;
                }
            }
            var std = svg.getElementById('Standardebene');
            for(idx = 0; idx < std.childNodes.length; idx++) {
                var c = std.childNodes.item(idx);
                if(c.nodeName == "g") {
                    if(c.getElementsByTagNameNS(svgns, "metadata").length === 0) {
                        c.setAttribute('stroke','#C0C0C0');
                    }
                }
            }
        }
</script>
```
