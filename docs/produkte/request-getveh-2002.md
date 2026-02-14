---
title: "Request getVehicleIdentificationByNationalCodeAustria"
topic_id: "2002"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Fahrzeugidentifikation Österreich - anhand des österreichischen Nationalcodes > Request getVehicleIdentificationByNationalCodeAustria"
---

# Request getVehicleIdentificationByNationalCodeAustria

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleIdentificationService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getVehicleIdentificationByNationalCodeAustria>
         <request>
            <!--type: string-->
            <nationalCode>162288</nationalCode>
            <locale country="at" datCountryIndicator="at" language="de"/>
            <!--Optional:-->
            <!--type: releaseRestriction - enumeration: [ALL,REPAIR,APPRAISAL,APPRAISALNEW]-->
            <restriction>ALL</restriction>
         </request>
      </veh:getVehicleIdentificationByNationalCodeAustria>
   </soapenv:Body>
</soapenv:Envelope>
```
