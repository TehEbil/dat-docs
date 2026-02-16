---
title: "Request getConstructionPeriodsN"
topic_id: "8656"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getConstructionPeriodsN > Request getConstructionPeriodsN"
---

# Request getConstructionPeriodsN

```
 <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
    <soapenv:Header/>
    <soapenv:Body>
       <veh:getConstructionPeriodsN>
          <request>
             <locale country="de" datCountryIndicator="de" language="de"/>
             <!--type: releaseRestriction - enumeration: [ALL,REPAIR,APPRAISAL]-->
             <restriction>ALL</restriction>
             <!--type: string-->
             <datECode>015700460110001</datECode>
             <!--Optional:-->
             <!--type: string-->
             <container>DE001</container>
          </request>
       </veh:getConstructionPeriodsN>
    </soapenv:Body>
 </soapenv:Envelope>
```
