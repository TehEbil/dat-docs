---
title: "Request getExistingEquipmentN"
topic_id: "2049"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Konvertierungsoperationen > getExistingEquipmentN > Request getExistingEquipmentN"
---

# Request getExistingEquipmentN

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:con="http://sphinx.dat.de/services/ConversionFunctionsService">
   <soapenv:Header/>
   <soapenv:Body>
      <con:getExistingEquipmentN>
         <request>
            <locale country="de" datCountryIndicator="de" language="de"/>
            <!--type: releaseRestriction - enumeration: [ALL,REPAIR,APPRAISAL]-->
            <restriction>REPAIR</restriction>
            <!--type: string-->
            <datECode>011300820150001</datECode>
            <!--Optional:-->
            <!--type: string-->
            <container>DE001</container>
            <!--type: int-->
            <constructionTime>4573</constructionTime>
         </request>
      </con:getExistingEquipmentN>
   </soapenv:Body>
</soapenv:Envelope>
```
