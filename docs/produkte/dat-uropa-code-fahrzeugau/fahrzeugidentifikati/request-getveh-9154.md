---
title: "Request getVehicleIdentificationByTypecodeToyota"
topic_id: "9154"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Fahrzeugidentifikation anhand Typcode Toyota > Request getVehicleIdentificationByTypecodeToyota"
---

# Request getVehicleIdentificationByTypecodeToyota

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleIdentificationService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getVehicleIdentificationByTypecodeToyota>
         <request>
            <locale country="de" datCountryIndicator="de" language="de"/>
            <!--type: releaseRestriction - enumeration: [ALL,REPAIR,APPRAISAL]-->
            <restriction>APPRAISAL</restriction>
            <coverage>ALL</coverage>
            <manufacturer>TOYOTA</manufacturer>
            <typeCode>DY14 H C2</typeCode>
            <productionDate>2002-03-02</productionDate>
            <equipmentCode>199</equipmentCode>
         </request>
      </veh:getVehicleIdentificationByTypecodeToyota>
   </soapenv:Body>
</soapenv:Envelope>
```
