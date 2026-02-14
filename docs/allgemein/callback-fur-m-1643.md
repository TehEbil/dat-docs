---
title: "Callback für MouseOut-Events"
topic_id: "1643"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > SVG in den DAT Anwendungen > Implementation > Integration der SVG-Dateien > Callback für MouseOut-Events"
---

# Callback für MouseOut-Events

Die nächste Funktion wird immer dann aufgerufen, wenn der User mit der Maus aus einem
auswählbaren Ersatzteil herausfährt. Alle veränderten Werte inklusive Tooltip werden
zurückgesetzt.

```
        function group_mouseout(e) {
            if(!e) {
                e = window.event;
        }
            var t = e.currentTarget;
            t.setAttribute("stroke", "#000000");
            t.setAttribute("fill", "none");
            t.setAttribute("opacity", "1");
            var subs = t.getElementsByTagNameNS(svgns, "g");
            for(var i = 0; i < subs.length; i++) {
                var g = subs.item(i);

<!-- if the id of the group is "DATID_000000" -->
                if(String(g.id).search(/DATID/) >= 0) {
                    g.setAttribute("fill", "none");
                    g.setAttribute("opacity", "1");
                }
            }
            document.getElementById('divToolTip').style.display = 'none';
        }
```
