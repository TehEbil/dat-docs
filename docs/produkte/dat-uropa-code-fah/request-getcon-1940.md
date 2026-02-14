---
title: "Request getConstructionOptions"
topic_id: "1940"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getConstructionOptions > Request getConstructionOptions"
---

# Request getConstructionOptions

```
 <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
    <soapenv:Header/>
    <soapenv:Body>
       <veh:getConstructionOptions>
          <request>
             <locale country="de" datCountryIndicator="de" language="de"/>
             <constructionTimeFrom>4040</constructionTimeFrom>
             <constructionTimeTo>4840</constructionTimeTo>
             <restriction>ALL</restriction>
             <!--type: int-->
             <vehicleType>4</vehicleType>
             <!--type: int-->
             <manufacturer>905</manufacturer>
             <!--type: int-->
             <baseModel>57</baseModel>
             <!--type: int-->
             <subModel>2</subModel>
             <!--Comment if not needed-->
             <!--type: int-->
             <availableOptions>15100</availableOptions>
          </request>
       </veh:getConstructionOptions>
    </soapenv:Body>
 </soapenv:Envelope>
```
