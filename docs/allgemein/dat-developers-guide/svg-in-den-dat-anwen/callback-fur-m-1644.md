---
title: "Callback für MouseClick-Events"
topic_id: "1644"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > SVG in den DAT Anwendungen > Implementation > Integration der SVG-Dateien > Callback für MouseClick-Events"
---

# Callback für MouseClick-Events

Die nächste Funktion wird immer dann aufgerufen, wenn der User mit der Maus auf ein
auswählbares Ersatzteil klickt. In diesem Fall wird aus <[metadata](element-metada-1620.md)> die jeweilige DVN-Nummer herausgesucht und in einem kleinen Fenster angezeigt. Wenn
eine DVN aus einer linken und rechten Seite besteht, werden beide DVNs angezeigt.

```
        function group_click(e) {
            if(!e)
                e = window.event;
            var t = e.currentTarget;
            var ms = t.getElementsByTagNameNS(svgns, 'metadata');
            if(ms.length === 0)
                return;
            var meta = ms.item(0);
            var arr = svg_getElementsByTagName(meta, 'dvnLeft');
            var dvnleft = '', dvnright = '';
            if(arr.length > 0)
            {
                arr = svg_getElementsByTagName(arr.item(0), 'dvn');
                if(arr.length > 0)
                {
                    //dvnleft = arr.item(0).textContent;
                    dvnleft = arr.item(0).firstChild.data;
                }
            }
            arr = svg_getElementsByTagName(meta, 'dvnRight');
            if(arr.length > 0)
            {
                arr = svg_getElementsByTagName(arr.item(0), 'dvn');
                if(arr.length > 0)
                {
                    dvnright = arr.item(0).firstChild.data;
                }
            }
            alert("DVN-Left: "+dvnleft + ", DVN-Right: " + dvnright);
        }
```
