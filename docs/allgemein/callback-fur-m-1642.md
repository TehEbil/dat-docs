---
title: "Callback für MouseOver-Events"
topic_id: "1642"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > SVG in den DAT Anwendungen > Implementation > Integration der SVG-Dateien > Callback für MouseOver-Events"
---

# Callback für MouseOver-Events

Das nachfolgende Beispiel zeigt drei Funktionen. Die erste Funktion wird immer dann
aufgerufen, wenn der User mit der Maus über ein auswählbares Ersatzteil fährt. Zur
Verdeutlichung verändert das ausgewählte Ersatzteil für diesen Event seine Füllfarbe
und die Rahmenfarbe. Außerdem wird in dieser Funktion der Tooltip-Text in der gewünschten
Sprache aus <[metadata](#showid/1620 "Element metadata")> herausgesucht.

Die zweite Funktion zeigt den Tooltip in der Oberfläche an. X und Y Koordinate des
Tooltips können hier den eigenen Wünschen angepasst werden. Um den Text in der Oberfläche
anzeigen zu können, wird zusätzlich noch ein Eintrag im Html-Body benötigt, der beispielhaft so aussehen könnte:

```
<div id="divToolTip" style="font-family: Arial;display:none;position:fixed;background:white;
    border:1px solid black;padding:3px;z-index: 5000;"></div>
```

Die letzte Funktion svg\_getElementsByTagName sorgt für die Zuweisung des DAT Namespace zum jeweiligen Element. Diese Funktion wird außerdem durchgehend in diesem
Beispielskript benutzt.

```
        function group_mouseover(e) {
            if (!e) {
                e = window.event;
            }
            var t = e.currentTarget;
            t.setAttribute("stroke", "#0000FF");
            var subs = t.getElementsByTagNameNS(svgns, "g");
            var count = 0;
            for(var i = 0; i < subs.length; i++) {
                var g = subs.item(i);
                //if(g.id == "DATID_000000")
                if(String(g.id).search(/DATID/) >= 0)
                {
                    g.setAttribute("fill", "#C0C0C0");
                    g.setAttribute("opacity", "0.5");
                    count++;
                }
            }
            if(count === 0) {
                t.setAttribute("fill", "#C0C0C0");
                t.setAttribute("opacity", "0.5");
            }

<!-- Determines the Tooltip-Text -->
            var ms = t.getElementsByTagNameNS(svgns, 'metadata');
            if(ms.length === 0)
                return;
            var meta = ms.item(0);
            var arr = svg_getElementsByTagName(meta, 'title');
            var tooltiptext = false;
            if(arr.length > 0) {
                arr = svg_getElementsByTagName(arr.item(0), 'lang');
                for(i = 0; i < arr.length; i++) {
                    var l = arr.item(i);
                    if(l.getAttribute('languageCode') === 'D') {
                        tooltiptext = l.firstChild.textContent;
                        break;
                    }
                }
            }
            if(tooltiptext !== false) {
                var x = e.x ? e.x : e.clientX;
                var y = e.y ? e.y : e.clientY;
                document.getElementById('divToolTip').innerHTML = tooltiptext;
                showTooltip('divToolTip', x, y);
            }
    }

<!-- Shows the tooltip -->
        function showTooltip(tooltipid, x, y) {
            var tooltip = document.getElementById(tooltipid);
            var nx = x+55;
            var ny = y + 10;
            tooltip.style.left = nx+'px';
            tooltip.style.top = ny+'px';
            tooltip.style.display = 'block';
        }

        function svg_getElementsByTagName(e, tagname) {
            return e.getElementsByTagNameNS(datns,tagname);
        }
```
