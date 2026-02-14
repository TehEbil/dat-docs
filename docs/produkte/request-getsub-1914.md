---
title: "Request getSubModels"
topic_id: "1914"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getSubModels > Request getSubModels"
---

# Request getSubModels

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getSubModels><!--Optional:-->
         <request>
            <locale country="de" datCountryIndicator="de" language="de"/>
            <constructionTimeFrom>4040</constructionTimeFrom>
            <constructionTimeTo>4840</constructionTimeTo>
            <restriction>APPRAISAL</restriction>
            <!--type: int-->
            <vehicleType>4</vehicleType>
            <!--type: int-->
            <manufacturer>750</manufacturer>
            <!--type: int-->
            <baseModel>11</baseModel>
         </request>
      </veh:getSubModels>
   </soapenv:Body>
</soapenv:Envelope>
```
