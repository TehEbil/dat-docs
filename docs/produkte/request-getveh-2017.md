---
title: "Request getVehicleTranslation"
topic_id: "2017"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Fahrzeugidentifikation in mehreren Sprachen > Request getVehicleTranslation"
---

# Request getVehicleTranslation

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleIdentificationService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getVehicleTranslation>
         <request>
            <locale country="de" datCountryIndicator="de" language="de"/>
            <!--type: releaseRestriction - enumeration: [ALL,REPAIR,APPRAISAL]-->
            <restriction>ALL</restriction>
            <!--type: string-->
            <datECode>018000510150004</datECode>
            <!--Optional:-->
            <!--type: string-->
            <container>DE007</container>
            <!--type: int-->
            <constructionTime>5260</constructionTime>
            <!--Optional:-->
            <specialEquipmentId>14205</specialEquipmentId>
            <specialEquipmentId>2756</specialEquipmentId>
            <specialEquipmentId>18505</specialEquipmentId>
            <specialEquipmentId>11271</specialEquipmentId>
            <!--Optional:-->
            <language>en_US</language>
         </request>
      </veh:getVehicleTranslation>
   </soapenv:Body>
</soapenv:Envelope>
```
