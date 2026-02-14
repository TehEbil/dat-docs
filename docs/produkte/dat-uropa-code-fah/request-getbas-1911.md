---
title: "Request getBaseModelsN"
topic_id: "1911"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getBaseModelsN > Request getBaseModelsN"
---

# Request getBaseModelsN

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getBaseModelsN>
         <request>
            <locale country="de" datCountryIndicator="de" language="de"/>
            <constructionTimeFrom>4040</constructionTimeFrom>
            <constructionTimeTo>4840</constructionTimeTo>
            <restriction>REPAIR</restriction>
            <!--type: int-->
            <vehicleType>4</vehicleType>
            <!--type: int-->
            <manufacturer>750</manufacturer>
            <!--Optional:-->
            <withRepairIncomplete>true</withRepairIncomplete>
         </request>
      </veh:getBaseModelsN>
   </soapenv:Body>
</soapenv:Envelope>
```
