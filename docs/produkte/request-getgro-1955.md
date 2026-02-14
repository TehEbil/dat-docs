---
title: "Request getGrossVehicleWeightOptions"
topic_id: "1955"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getGrossVehicleWeightOptions > Request getGrossVehicleWeightOptions"
---

# Request getGrossVehicleWeightOptions

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getGrossVehicleWeightOptions>
         <request>
            <locale country="de" datCountryIndicator="de" language="de"/>
            <constructionTimeFrom>4040</constructionTimeFrom>
            <constructionTimeTo>4840</constructionTimeTo>
            <restriction>ALL</restriction>
            <vehicleType>4</vehicleType>
            <manufacturer>285</manufacturer>
            <baseModel>43</baseModel>
            <subModel>1</subModel>
            <!--Comment if not needed-->
            <availableOptions>94204</availableOptions>
         </request>
      </veh:getGrossVehicleWeightOptions>
   </soapenv:Body>
</soapenv:Envelope>
```
