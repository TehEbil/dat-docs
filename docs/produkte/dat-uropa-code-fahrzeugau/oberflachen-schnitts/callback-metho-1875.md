---
title: "Callback-Methode für Fehlerbehandlungen"
topic_id: "1875"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Oberflächen-Schnittstelle > Integration der Oberfläche > Callback-Methode für Fehlerbehandlungen"
---

# Callback-Methode für Fehlerbehandlungen

Sollte beim Aufruf der DAT €uropa-Code® Fahrzeugauswahl ein Fehler auftreten und die
Fahrzeugauswahl nicht geladen werden können, wird eine Callback-Methode zur Fehlerbehandlung
aufgerufen.

Diese Callback-Methode benötigt ebenfalls einen Parameter, der einen optionalen Error-String
entgegennimmt. Sie dient prinzipiell lediglich dazu, auf Verbindungsfehler oder Fehlermeldungen
aufgrund falscher oder falsch formatierter Eingabeparameter reagieren zu können.

Eine einfache Implementierung sieht wie folgt aus:

```
<script type="text/javascript" language="JavaScript">
  function errorFunc(e){
    alert(e);
  }
</script>
```
