---
title: "Request getDriversCabOptions"
topic_id: "1947"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getDriversCabOptions > Request getDriversCabOptions"
---

# Request getDriversCabOptions

```
 <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
    <soapenv:Header/>
    <soapenv:Body>
       <veh:getDriversCabOptions>
          <request>
             <locale country="de" datCountryIndicator="de" language="de"/>
            <constructionTimeFrom>4040</constructionTimeFrom>
            <constructionTimeTo>4840</constructionTimeTo>
             <restriction>ALL</restriction>
             <!--type: int-->
             <vehicleType>4</vehicleType>
             <!--type: int-->
             <manufacturer>570</manufacturer>
             <!--type: int-->
             <baseModel>63</baseModel>
             <!--type: int-->
             <subModel>48</subModel>
             <!--Comment if not needed-->
             <!--type: int
             <availableOptions>0</availableOptions>-->
          </request>
       </veh:getDriversCabOptions>
    </soapenv:Body>
 </soapenv:Envelope>
```
