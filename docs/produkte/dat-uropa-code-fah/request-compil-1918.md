---
title: "Request compileDatECode"
topic_id: "1918"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > compileDatECode > Request compileDatECode"
---

# Request compileDatECode

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:compileDatECode><!--Optional:-->
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
            <!--1 or more repetitions:-->
            <!--type: int-->
            <selectedOptions>10003</selectedOptions>
            <selectedOptions>83950</selectedOptions>
            <selectedOptions>75205</selectedOptions>
         </request>
      </veh:compileDatECode>
   </soapenv:Body>
</soapenv:Envelope>
```
