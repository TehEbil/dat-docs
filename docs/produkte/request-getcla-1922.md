---
title: "Request getClassificationGroups"
topic_id: "1922"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getClassificationGroups > Request getClassificationGroups"
---

# Request getClassificationGroups

```
 <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
    <soapenv:Header/>
    <soapenv:Body>
       <veh:getClassificationGroups><!--Optional:-->
          <request>
             <locale country="de" datCountryIndicator="de" language="de"/>
             <!--type: releaseRestriction - enumeration: [ALL,REPAIR,APPRAISAL]-->
             <restriction>APPRAISAL</restriction>
             <!--type: int-->
             <vehicleType>1</vehicleType>
             <!--type: int-->
             <manufacturer>130</manufacturer>
             <!--type: int-->
             <baseModel>82</baseModel>
             <!--type: int-->
             <subModel>15</subModel>
          </request>
       </veh:getClassificationGroups>
    </soapenv:Body>
 </soapenv:Envelope>
```
