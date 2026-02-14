---
title: "Request getManufacturers"
topic_id: "1908"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getManufacturers > Request getManufacturers"
---

# Request getManufacturers

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getManufacturers>
         <request>
            <locale country="de" datCountryIndicator="de" language="de"/>
            <constructionTimeFrom>4040</constructionTimeFrom>
            <constructionTimeTo>4840</constructionTimeTo>
            <!--type: releaseRestriction - enumeration: [ALL,REPAIR,APPRAISAL]-->
            <restriction>APPRAISAL</restriction>
            <!--type: int-->
            <vehicleType>4</vehicleType>
         </request>
      </veh:getManufacturers>
   </soapenv:Body>
</soapenv:Envelope>
```
