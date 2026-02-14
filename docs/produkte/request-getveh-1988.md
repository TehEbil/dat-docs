---
title: "Request getVehicleData"
topic_id: "1988"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getVehicleData > Request getVehicleData"
---

# Request getVehicleData

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getVehicleData>
         <request>
            <locale country="de" datCountryIndicator="de" language="de"/>
            <!--type: releaseRestriction - enumeration: [ALL,REPAIR,APPRAISAL]-->
            <restriction>REPAIR</restriction>
            <!--type: string-->
            <datECode>011300820150001</datECode>
            <!--Optional:-->
            <!--type: string-->
            <container>DE001</container>
            <!--type: int-->
            <constructionTime>4667</constructionTime>
         </request>
      </veh:getVehicleData>
   </soapenv:Body>
</soapenv:Envelope>
```
