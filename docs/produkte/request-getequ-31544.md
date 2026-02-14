---
title: "Request getEquipmentFromManufacturerCode"
topic_id: "31544"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getEquipmentFromManufacturerCode > Request getEquipmentFromManufacturerCode"
---

# Request getEquipmentFromManufacturerCode

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:con="http://sphinx.dat.de/services/ConversionFunctionsService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getEquipmentFromManufacturerCodeN>
         <request>
            <locale country="de" datCountryIndicator="de" language="de"/>
            <!--type: releaseRestriction - enumeration: [ALL,REPAIR,APPRAISAL]-->
            <restriction>ALL</restriction>
            <!--type: string-->
            <datECode>019051450310001</datECode>
            <!--Optional:-->
            <!--type: string-->
            <container>DE001</container>
            <!--type: int-->
            <constructionTime>6077</constructionTime>
            <!--1 or more repetitions:-->
            <!--type: string-->
            <manufacturerCodes>G1A</manufacturerCodes>
            <manufacturerCodes>K8D</manufacturerCodes>
            <manufacturerCodes>8IT</manufacturerCodes>
         </request>
      </veh:getEquipmentFromManufacturerCodeN>
   </soapenv:Body>
</soapenv:Envelope>
```
