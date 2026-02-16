---
title: "Request getGearingOptions"
topic_id: "1951"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getGearingOptions > Request getGearingOptions"
---

# Request getGearingOptions

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getGearingOptions>
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
            <!--availableOptions>0</availableOptions-->
         </request>
      </veh:getGearingOptions>
   </soapenv:Body>
</soapenv:Envelope>
```
