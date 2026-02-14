---
title: "Komplett-Beispiel für die Einbindung als Objekt"
topic_id: "1635"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > SVG in den DAT Anwendungen > Implementation > Integration der SVG-Dateien > Komplett-Beispiel für die Einbindung als Objekt"
---

# Komplett-Beispiel für die Einbindung als Objekt

```
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
<html lang="de" >
<body onload="document.getElementById('cgSelect').onchange = changeGroup; init('svg');">
    Demo on how to interact with SVGs that come with "DAT €uropa-Code Data Set, Supplemental element 4<br />
    Copyright &copy; 2010-2012 by Deutsche Automobil Treuhand GmbH<br />
    Construction group 
        <select id="cgSelect">
        <option val="D_1_040_070_01.svg" selected>D_1_040_070_01.svg</option>
        <option val="D_1_345_007_18.svg">D_1_345_007_18.svg</option>
        <option val="D_1_285_120_12.svg">D_1_285_120_12.svg</option>
        <option val="D_1_190_080_06.svg">D_1_190_080_06.svg</option>
        </select>
    <p />
<!-- The next div is used for displaying the tooltips -->
    <div id="divToolTip" style="font-family: Arial;display:none;position:fixed;background:white;
    border:1px solid black;padding:3px;z-index: 5000;"></div>
<!-- Element object contains the svg-files, displayed as a list -->
    <object id="svg" width="500" height="800" type="image/svg+xml"
        data="D_1_040_070_01.svg"> 
   Your browser doesn't support SVG. You can download the plugin at 
<a href="http://www.adobe.com/svg/viewer/install/">http://www.adobe.com/svg/viewer/install/</a>
    </object>
<!-- following script handles events like mouseover and so on -->
    <script type="text/javascript">
        var svgns = 'http://www.w3.org/2000/svg';
        var datns = 'http://www.dat.de/sphinx/svg';

<!-- Callback is called whenever the user moves the mouse over a selectable part -->
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
        
<!-- Callback is called whenever the user moves the mouse out of the spare part; mostly used to -->
<!-- restore the standard appearance and to remove the tooltip -->
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
        
        function svg_getElementsByTagName(e, tagname) {
            return e.getElementsByTagNameNS(datns,tagname);
        }    

<!-- Callback is called whenever the user clicks on a selectable spare part -->
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
        
<!-- Add a mouseover, mouseout and click-event to all g-Elements that have metadata-children -->
        function init(svgid){
            var svg = document.getElementById(svgid).contentDocument;
            var elements = svg.getElementsByTagNameNS(svgns, "g");
            for(var idx = 0; idx < elements.length; idx++) {
                var g=elements.item(idx);
<!-- only those elements having a child "metadata" will get a listener
                if(String(g.id).search(/DATID/) >= 0 && g.id != "DATID_000000" && g.getElementsByTagNameNS(svgns, "metadata").length > 0) {
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
<!-- next function only used for drowdownbox in html. don't forget to enhance the onload in body
        function changeGroup(evt) {
            var t = evt.currentTarget;

            document.getElementById('svg').setAttribute('data', t.value);
            setTimeout(function() {
            init('svg');
            }, 2000);
        }        
    </script>
</body>
</html>
```
