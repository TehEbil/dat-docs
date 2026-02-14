---
title: "Request getVehicleIdentification"
topic_id: "1995"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Fahrzeugidentifikation anhand DAT €uropa-Code® > Request getVehicleIdentification"
---

# Request getVehicleIdentification

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleIdentificationService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getVehicleIdentification>
         <!--Optional:-->
         <request>
            <locale country="de" datCountryIndicator="de" language="de"/>
            <!--type: releaseRestriction - enumeration: [ALL,REPAIR,APPRAISAL]-->
            <restriction>ALL</restriction>
            <!--type: string-->
            <datECode>011300220020006</datECode>
            <!--Optional:-->
            <!--type: string-->
            <container>DE001</container>
            <!--type: int-->
            <constructionTime>3610</constructionTime>
         </request>
      </veh:getVehicleIdentification>
   </soapenv:Body>
</soapenv:Envelope>
```
