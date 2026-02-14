---
title: "Callback-Methode für die Verarbeitung eines abgeschlossenen Vorgangs"
topic_id: "2399"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Integration der Oberfläche > Callback-Methode für die Verarbeitung eines abgeschlossenen Vorgangs"
---

# Callback-Methode für die Verarbeitung eines abgeschlossenen Vorgangs

Wurde vom Benutzer eine Kalkulation durchgeführt und der Benutzer klickt auf den Weiter-Button
im letzten Prozessschritt, dann ruft SilverDAT calculatePro eine Callback-Methode
auf, um das Die Callback-Methode wird mit Klick auf den Weiter-Button auf der letzten
Seite aufgerufen. Sie übermittelt das Ergebnis der Schadenkalkulation am Ende des
eingestellten Pageflow.

Die Callback-Methode muss zuvor implementiert sein. Sie benötigt einen Parameter,
der das Ergebnis entgegennimmt. Das Ergebnis besteht aus einem XML-String. Der XML-String
entspricht dem DAT VXS-Schnitttstellenformat und enthält ausschließlich folgende Daten:

- DAT Europa-Code, 15-stellig
- Bauzeit, 4-stellig, DAT-Notation
- Aktenzeichen-Nummer

  ```
  <?xml version="1.0" encoding="UTF-8" standalone="no"?>
  <data>
  <DatECode>01 670 058 015 0004</DatECode>
  <Container/>
  <ConstructionTime>5661</ConstructionTime>
  <az>13690345</az>
  </data>
  ```

- Die Callback-Methode muss vom Schnittstellenpartner so implementiert werden, dass
  sie die Verarbeitung der zurückgelieferten Daten übernimmt oder auslöst.

Ein einfaches Beispiel einer derartigen Callback-Methode sieht wie folgt aus:

```
<script type="text/javascript" language="JavaScript">
  function callbackFromSphinx ( object, xml ){
//delete Sphinx iFrame from DOM-Tree
    sphinx.deleteIframe();
    //show return values
    alert ( "Calculation is ready: " + xml.xml );
  }
</script>
```
