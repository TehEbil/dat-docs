---
title: "Request getVehicleIdentificationByVin"
topic_id: "2013"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Fahrzeugidentifikation anhand VIN (VIN-Abfrage) > Request getVehicleIdentificationByVin"
---

# Request getVehicleIdentificationByVin

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleIdentificationService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getVehicleIdentificationByVin>
         <request>
            <locale country="de" datCountryIndicator="de" language="de"/>
            <!--Optional:-->
            <!--type: int-->
            <!--constructionTime>?</constructionTime-->
            <!--type: releaseRestriction - enumeration: [ALL,REPAIR,APPRAISAL]-->
            <restriction>ALL</restriction>
            <!--type: string-->
            <vin>WVWDEXTESTSTUB001</vin>
            <!--Optional:-->
            <!--type: coverage - enumeration: [ALL,WITH_MANUFACTURER_TEXTS,WITH_PRICE_LIST_TIME]-->
            <coverage>ALL</coverage>
         </request>
      </veh:getVehicleIdentificationByVin>
   </soapenv:Body>
</soapenv:Envelope>
```
