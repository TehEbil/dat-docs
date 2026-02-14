---
title: "HTML-Grundgerüst"
topic_id: "1855"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Oberflächen-Schnittstelle > Integration der Oberfläche > HTML-Grundgerüst"
---

# HTML-Grundgerüst

Wenn Sie aus den folgenden Fragmenten ein Komplettbeispiel erzeugen und in eine HTML-Datei
schreiben, können Sie dies nicht direkt über file://... aus dem Browser aufrufen.
Die Browser erlauben das nicht und der Integrationsprozess scheitert. Verwenden Sie
bitte hierfür einen HTTP Web-Server.

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

Die DAT €uropa-Code® Fahrzeugauswahl kann entweder direkt unter <body> oder aber einem
Kindelement erzeugt werden. Wichtig ist dabei, ob die Seite lediglich die DAT €uropa-Code®
Fahrzeugauswahl beinhalten soll oder ob noch weitere Inhalte/Steuerelemente dazu kommen.
Sollte letzteres der Fall sein, bietet es sich u.U. an, ein eigenes Vaterelement für
die DAT €uropa-Code® Fahrzeugauswahl zu benutzen:

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
      <script language="JavaScript" src="https://www.dat.de/sphinx/js/lazyload.js" type="text/javascript"></script>
      <script language="JavaScript" src="https://www.dat.de/sphinx/js/externalSphinx.js" type="text/javascript"></script>
      <script language="JavaScript" src="https://code.jquery.com/jquery-2.2.4.min.js" type="text/javascript"></script>
  </head>
  <body>
    <div id="datParentNode"></div>
  </body>
</html>
```

Die Datei sphinx.js stellt dabei ein globales JavaScript-Objekt namens sphinx zur Verfügung, das für alle Interaktionen mit der DAT €uropa-Code Fahrzeugauswahl
benutzt wird.
