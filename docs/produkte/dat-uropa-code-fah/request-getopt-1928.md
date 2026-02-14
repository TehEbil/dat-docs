---
title: "Request getOptionsbyClassification"
topic_id: "1928"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getOptionsbyClassification > Request getOptionsbyClassification"
---

# Request getOptionsbyClassification

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getOptionsbyClassification><!--Optional:-->
         <request>
            <locale country="de" datCountryIndicator="de" language="de"/>
            <!--type: releaseRestriction - enumeration: [ALL,REPAIR,APPRAISAL]-->
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
            <!--availableOptions></availableOptions-->
            <!--type: int-->
            <classification>11</classification>
         </request>
      </veh:getOptionsbyClassification>
   </soapenv:Body>
</soapenv:Envelope>
```
