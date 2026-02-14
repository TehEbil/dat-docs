---
title: "Einbetten einer SVG-Datei als Objekt"
topic_id: "1633"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > SVG in den DAT Anwendungen > Implementation > Einbetten einer SVG-Datei als Objekt"
---

# Einbetten einer SVG-Datei als Objekt

Damit ein Darstellungsprogramm in (x)html selbst entscheiden kann, ob es die SVG-Datei selbst interpretiert oder ob womöglich ein Plugin verwendet werden kann, empfiehlt sich die Verwendung von Objekt-Elementen. Es gibt
bislang drei hauptsächliche Möglichkeiten, eine SVG-Datei als Objekt in ein (x)html einzubinden:

- innerhalb des Elementes <object>

  Vorteil: Wird von den meisten Browsern unterstützt und ist Standard in Html4, Html5 und Xhtml; vom W3C-Consortium empfohlen

  Nachteil: Erlaubt kein scripting
- innerhalb des Elementes <embed>

  Vorteil: Wird von den meisten Browsern unterstützt und erlaubt scripting

  Nachteil: kann nur noch in Html5 benutzt werden
- innerhalb des Elementes <iframe>

  Vorteil: Wird von den meisten Browsern unterstützt

  Nachteil: generiert einen Rahmen um die SVG-Datei und kann nur noch in Html5 benutzt werden
- innerhalb des Elementes <img>

  Diese Verwendung wird nicht empfohlen, da sie nur stark eingeschränkt in bestimmten
  Browsern einsatzfähig ist (Opera, Safari, Chrome).

Für Browser, die kein SVG interpretieren (können), empfiehlt es sich, ein Fallback in Form eines Ersatzbildes oder einer Textalternative vorzusehen. Mit einem direkten
Verweis auf die SVG-Datei erhält der Betrachter die Möglichkeit, sich die SVG-Datei mit einem externen Programm anzusehen. In den unten angegebenen Beispielen
ist auch jedes Mal eine Textalternative, ein Ersatzbild oder ein Verweis zu einem
externen Programm angegeben.

Die Objekt-Elemente sollten ein Minimum an Attributen erhalten, um die SVG-Datei korrekt im Browser darzustellen.

| Name | Beschreibung | genutzt in Objekt-Element |
| --- | --- | --- |
| id | interner Name der eingebundenen SVG-Datei | object |
| name | interner Name der eingebundenen SVG-Datei | iframe |
| width | Breite der SVG-Datei | object, embed, iframe |
| height | Höhe der SVG-Datei | object, embed, iframe |
| type | MIME type für die Darstellung | object, embed |
| src | SVG-Datei mit Pfad-Angabe | embed, iframe |
| data | SVG-Datei mit Pfad-Angabe | object |

Beispiele

```
<object id="svg" width="500" height="800" type="image/svg+xml" data="D_1_040_070_01.svg" >
    Your browser doesn't support SVG. You can download the plugin at 
    <a href="http://www.adobe.com/svg/viewer/install/">http://www.adobe.com/svg/viewer/install/</a>
</object>
```

```
<embed data-src="D_1_040_070_01.svg" type="image/svg+xml">
    <NOEMBED><IMG data-src="imageOnError.gif"/></NOEMBED>
</embed> 
```

```
<iframe data-src="D_1_285_120_12.svg" width="500" height="800" name="imap">
    Your browser doesn't support SVG. You can download the plugin at 
    <a href="http://www.adobe.com/svg/viewer/install/">http://www.adobe.com/svg/viewer/install/</a>
</iframe>
```

Die Attribute zu Breite und Höhe im Objekt-Element werden vom Browser genau interpretiert.
Sind die Größenangaben nicht passgenau, wird die Darstellung u.U. abgeschnitten.

Das folgende [Komplett-Beispiel für die Einbindung als Objekt](#showid/1635 "Komplett-Beispiel für die Einbindung als Objekt") enthält einen Event-Handler, der sowohl für Pixel- als auch für Vektorgrafiken geeignet
ist. Beim Überfahren der eingebundenen SVG-Grafik mit der Maus wird das jeweilige Fahrzeugteil hervorgehoben.

Wenn Sie das Komplett-Beispiel zum Testen verwenden, passen Sie bitte die SVG-Dateien in der Listbox und im Element object an Ihre vorhandenen SVG-Dateien an.
