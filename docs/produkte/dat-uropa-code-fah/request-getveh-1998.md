---
title: "Request getVehicleIdentificationByKba"
topic_id: "1998"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Fahrzeugidentifikation anhand KBA > Request getVehicleIdentificationByKba"
---

# Request getVehicleIdentificationByKba

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleIdentificationService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getVehicleIdentificationByKba>
         <request>
            <!--type: string-->
            <kba>0005/AHT</kba>
            <!--Optional:-->
            <locale country="de" datCountryIndicator="de" language="de"/>
            <!--Optional:-->
            <!--type: releaseRestriction - enumeration: [ALL,REPAIR,APPRAISAL,APPRAISALNEW]-->
            <restriction>ALL</restriction>
         </request>
      </veh:getVehicleIdentificationByKba>
   </soapenv:Body>
</soapenv:Envelope>
```
