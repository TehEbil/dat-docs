---
title: "Request getTypeOfDriveOptions"
topic_id: "1968"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getTypeOfDriveOptions > Request getTypeOfDriveOptions"
---

# Request getTypeOfDriveOptions

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getTypeOfDriveOptions>
         <request>
            <locale country="de" datCountryIndicator="de" language="de"/>
            <restriction>ALL</restriction>
            <constructionTimeFrom>4040</constructionTimeFrom>
            <constructionTimeTo>4840</constructionTimeTo>
            <vehicleType>2</vehicleType>
            <manufacturer>520</manufacturer>
            <baseModel>10</baseModel>
            <subModel>22</subModel>
            <!--Zero or more repetitions:-->
            <availableOptions>96513</availableOptions>
         </request>
      </veh:getTypeOfDriveOptions>
   </soapenv:Body>
</soapenv:Envelope>
```
