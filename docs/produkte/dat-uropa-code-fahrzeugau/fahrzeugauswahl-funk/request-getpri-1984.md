---
title: "Request getPriceFocusConstructionYears"
topic_id: "1984"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getPriceFocusConstructionYears > Request getPriceFocusConstructionYears"
---

# Request getPriceFocusConstructionYears

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getPriceFocusConstructionYears>
         <request>
            <locale country="de" datCountryIndicator="de" language="de"/>
            <restriction>APPRAISAL</restriction>
            <datECode>015700400630002</datECode>
         </request>
      </veh:getPriceFocusConstructionYears>
   </soapenv:Body>
</soapenv:Envelope>
```
