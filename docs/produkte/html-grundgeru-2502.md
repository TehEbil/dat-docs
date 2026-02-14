---
title: "HTML-Grundgerüst"
topic_id: "2502"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Integration der Oberfläche > HTML-Grundgerüst"
---

# HTML-Grundgerüst

Die bereitzustellende HTML-Datei sollte in etwa so aussehen:

```
<html>
  <head>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
    <title>Title</title>
  </head>
  <body></body>
</html>
```

SilverDAT calculatePro kann entweder direkt unter <body> oder aber einem Kind-Element erzeugt werden. Wichtig ist dabei, ob die Seite lediglich
SilverDAT calculatePro beinhalten soll oder ob noch weitere Inhalte/Steuerelemente
dazu kommen. Sollte letzteres der Fall sein, bietet es sich u.U. an ein eigenes Vater-Element
für SilverDAT calculatePro zu benutzen:

```
<html>
  <head>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
    <title>Title</title>
  </head>
  <body>
    <div id="datParentNode"></div>
  </body>
</html>
```

In das HTML-Grundgerüst müssen weiterhin die zwingend benötigten JavaScript-Dateien
von DAT inkludiert werden:

```
<html>
  <head>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
    <title>Title</title>
    <script language="JavaScript" src="http://www.dat.de/sphinx/js/lazyload.js"
 type="text/javascript"></script>
    <script language="JavaScript" data-src=" http://www.dat.de/sphinx/js/externalSphinx.js"
 type="text/javascript"></script>
  </head>
  <body>
    <div id="datParentNode"></div>
  </body>
</html>
```

Die Datei externalSphinx.js stellt dabei ein globales JavaScript-Objekt namens sphinx zur Verfügung, das für alle Interaktionen mit SilverDAT calculatePro benutzt wird.
