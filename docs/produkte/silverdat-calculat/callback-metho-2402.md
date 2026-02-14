---
title: "Callback-Methode für Fehlerbehandlungen"
topic_id: "2402"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Integration der Oberfläche > Callback-Methode für Fehlerbehandlungen"
---

# Callback-Methode für Fehlerbehandlungen

Sollte beim Aufruf der SilverDAT calculatePro ein Fehler auftreten und deshalb die Oberfläche nicht geladen werden können, wird
eine Callback-Methode zur Fehlerbehandlung aufgerufen.

Diese Methode benötigt ebenfalls einen Parameter, der einen optionalen Error-String
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
