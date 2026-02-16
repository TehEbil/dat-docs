---
title: "Request getNumberOfAxleOptions"
topic_id: "1960"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getNumberOfAxleOptions > Request getNumberOfAxleOptions"
---

# Request getNumberOfAxleOptions

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getNumberOfAxleOptions>
         <request>
            <locale country="de" datCountryIndicator="de" language="de"/>
            <restriction>ALL</restriction>
            <constructionTimeFrom>4040</constructionTimeFrom>
            <constructionTimeTo>4840</constructionTimeTo>
            <vehicleType>4</vehicleType>
            <manufacturer>285</manufacturer>
            <baseModel>43</baseModel>
            <subModel>1</subModel>
            <!--Comment if not needed-->
            <availableOptions>94204</availableOptions>
         </request>
      </veh:getNumberOfAxleOptions>
   </soapenv:Body>
</soapenv:Envelope>
```
