---
title: "Aufruf der DAT €uropa-Code Fahrzeugauswahl"
topic_id: "1876"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Oberflächen-Schnittstelle > Integration der Oberfläche > Aufruf der DAT €uropa-Code Fahrzeugauswahl"
---

# Aufruf der DAT €uropa-Code Fahrzeugauswahl

Zum Aufruf der DAT €uropa-Code® Fahrzeugauswahl werden benötigt:

- Basis-URL der Fahrzeugauswahl:

  - https://www.dat.de/DATECodeSelection
- Zieladresse, derzeit immer https://www.dat.de/DATECodeSelection/vehicleSelection/model.tmpl
- [Aufbereitung der Authentifizierungsinformationen](#showid/1859 "Aufbereitung der Authentifizierungsinformationen")
- [Callback-Methode für die Verarbeitung einer abgeschlossenen Fahrzeugauswahl](#showid/1861 "Callback-Methode für die Verarbeitung einer abgeschlossenen Fahrzeugauswahl")
- [Callback-Methode für Fehlerbehandlungen](#showid/1875 "Callback-Methode für Fehlerbehandlungen")

Das globale sphinx-Objekt stellt für den Aufruf eine Eigenschaft und zwei Methoden zur Verfügung. Zuerst
muss die Eigenschaft host gesetzt werden, dann wird optional über firstPage die Startseite und über lastPage die letzte Seite im Pageflow festgelegt. Danach wird die Fahrzeugauswahl über die
Methode init initialisiert und zuletzt über die Methode execute zur Anzeige und Ausführung gebracht.

| Methode bzw. Property | Typ | Bedeutung |
| --- | --- | --- |
| sphinx.host | Eigenschaft | Bais-URL der DAT €uropa-Code® Fahrzeugauswahl |
| sphinx.firstPage | Eigenschaft | Steuerung der ersten Seite des Pageflows, mögliche Werte sind 'model selection', 'equipment selection', 'vehicle summary' und 'vehicle data' |
| sphinx.lastPage | Eigenschaft | Steuerung der letzten Seite des Pageflows, mögliche Werte sind 'model selection', 'equipment selection', 'vehicle summary' und 'vehicle data' |
| sphinx.init | Methode | Initialisierung der Fahrzeugauswahl mit den Parametern:  Zieladresse  ID der Zielseite, mögliche Werte sind 'model', 'model selection', 'equipment selection', 'vehicle summary' und 'vehicle data'  Name der DOM-Node unter der der iFrame für die Fahrzeugauswahl erzeugt werden soll (bei Übergabe von null wird der iFrame direkt unter body erzeugt  Name der CSS-Klasse mit CSS-Eigenschaften für den zu erzeugenden iFrame, bspw. modelIFrame  null oder Adresse (URL) eines eigenen CSS-Stylesheets mit weiterführenden CSS-Eigenschaften  Callback-Methode für die Verarbeitung einer abgeschlossenen Fahrzeugauswahl |
| sphinx.execute | Methode | Anzeige bzw. Ausführung der Fahrzeugauswahl mit den Parametern:  Authentifizierungsdaten vom Typ DatLoginInformation  null oder XML-String mit den Eingabeparametern  Callback-Methode für Fehlerbehandlungen |

```
<script type="text/javascript" language="JavaScript">
  ...
   function load(){
    ...
      sphinx.host='https://www.dat.de/DATECodeSelection';

      // adjust pageflow and destination page
      sphinx.firstPage = 'model selection';
      sphinx.lastPage =  'vehicle data';
      var destination = 'model selection';

      //initialize    
      sphinx.init(sphinx.host + "/vehicleSelection/model.tmpl", destination,
                  document.getElementById('iframeContainer'), "modelIFrame");

      //display and execute
      try{
        sphinx.execute(loginInfo, params, errorFunc);
      }
      catch(e){
        document.getElementById('iframeContainer').innerHTML = e;
      }
    }
  ...
</script>
```
