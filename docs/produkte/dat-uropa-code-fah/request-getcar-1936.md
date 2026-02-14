---
title: "Request getCarBodyOptions"
topic_id: "1936"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getCarBodyOptions > Request getCarBodyOptions"
---

# Request getCarBodyOptions

```
 <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
    <soapenv:Header/>
    <soapenv:Body>
       <veh:getCarBodyOptions><!--Optional:-->
          <request>
             <locale country="de" datCountryIndicator="de" language="de"/>
            <constructionTimeFrom>4040</constructionTimeFrom>
            <constructionTimeTo>4840</constructionTimeTo>
             <restriction>ALL</restriction>
             <!--type: int-->
             <vehicleType>1</vehicleType>
             <!--type: int-->
             <manufacturer>130</manufacturer>
             <!--type: int-->
             <baseModel>82</baseModel>
             <!--type: int-->
             <subModel>15</subModel>
             <!--Comment if not needed-->
             <!--type: int-->
             <!--availableOptions>10003</availableOptions-->
          </request>
       </veh:getCarBodyOptions>
    </soapenv:Body>
 </soapenv:Envelope>
```
