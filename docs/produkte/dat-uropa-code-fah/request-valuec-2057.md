---
title: "Request valueCode2Description"
topic_id: "2057"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Konvertierungsoperationen > valueCode2Description > Request valueCode2Description"
---

# Request valueCode2Description

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:con="http://sphinx.dat.de/services/ConversionFunctionsService">
   <soapenv:Header/>
   <soapenv:Body>
      <con:valueCode2Description>
         <request>
            <locale country="de" datCountryIndicator="de" language="de"/>
            <!--type: releaseRestriction - enumeration: [ALL,REPAIR,APPRAISAL]-->
            <restriction>REPAIR</restriction>
            <!--type: string-->
            <datECode>011301061440002</datECode>
            <!--Optional:-->
            <!--type: string-->
            <container>DE002</container>
         </request>
      </con:valueCode2Description>
   </soapenv:Body>
</soapenv:Envelope>
```
