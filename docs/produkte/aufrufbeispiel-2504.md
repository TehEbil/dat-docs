---
title: "Aufrufbeispiele"
topic_id: "2504"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Integration der Oberfläche > Aufruf der SilverDAT calculatePro / calculateExpert Oberfläche > Aufrufbeispiele"
---

# Aufrufbeispiele

Aufruf ohne Seitenbeschränkung

```
<script type="text/javascript" language="JavaScript">
  ...
   function load(){
    ...
      sphinx.host='https://www.dat.de/VehicleRepairOnline;
      sphinx.servletmapping='external';
   //initialize    
    sphinx.init(sphinx.host + "/vehicleSelection/model.tmpl", "model",
                document.getElementById('iframeContainer'),
                "modelIFrame", null, responseCallback);
    //display and execute
    sphinx.execute(loginInfo, params, errorFunc);
  }
</script>
```

Aufrufe mit Seitenbeschränkung durch firstPage oder lastPage

```
// Sprung in die Auftragseröffnung mit der Möglichkeit, bis zur printAndSend-Seite zu springen
// zusätzlicher Parameter lastPage
sphinx.lastPage = "printAndSend";
sphinx.init(sphinx.host +"/VehicleRepairOnline/contractOpening.html","contractOpening",document.getElementById('iframeContainer'), "modelIFrame");
```

```
// Sprung in die grafische Teileauswahl ohne Möglichkeit, vor- oder zurückzuspringen
// zusätzliche Parameter firstPage, lastPage
sphinx.firstPage = "graphicSelectionPage";
sphinx.lastPage = "graphicSelectionPage";
sphinx.init(sphinx.host + "/vehicleRepair/graphicalPartSelectionPage.tmpl", "graphicSelectionPage",  document.getElementById('iframeContainer'), "modelIFrame");
```
