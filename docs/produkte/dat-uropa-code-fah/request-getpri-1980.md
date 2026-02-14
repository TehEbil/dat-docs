---
title: "Request getPriceFocusCases"
topic_id: "1980"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getPriceFocusCases > Request getPriceFocusCases"
---

# Request getPriceFocusCases

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getPriceFocusCases>
         <request>
            <locale country="de" datCountryIndicator="de" language="de"/>
            <constructionTimeFrom>4040</constructionTimeFrom>
            <constructionTimeTo>4840</constructionTimeTo>
            <restriction>ALL</restriction>
            <datECode>011300820150001</datECode>
         </request>
      </veh:getPriceFocusCases>
   </soapenv:Body>
</soapenv:Envelope>
```
