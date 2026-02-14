---
title: "Request getEngineOptions"
topic_id: "1932"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getEngineOptions > Request getEngineOptions"
---

# Request getEngineOptions

```
 <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
    <soapenv:Header/>
    <soapenv:Body>
       <veh:getEngineOptions><!--Optional:-->
          <request>
             <locale country="de" datCountryIndicator="de" language="de"/>
            <constructionTimeFrom>4040</constructionTimeFrom>
            <constructionTimeTo>4840</constructionTimeTo>
             <restriction>ALL</restriction>
             <vehicleType>1</vehicleType>
             <manufacturer>130</manufacturer>
             <baseModel>82</baseModel>
             <subModel>10</subModel>
             <!--Comment if not needed-->
             <!--availableOptions>83950</availableOptions-->
             <!--type: int-->
         </request>
       </veh:getEngineOptions>
    </soapenv:Body>
 </soapenv:Envelope>
```
