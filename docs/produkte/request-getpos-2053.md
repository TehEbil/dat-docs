---
title: "Request getPossibleEquipmentN"
topic_id: "2053"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Konvertierungsoperationen > getPossibleEquipmentN > Request getPossibleEquipmentN"
---

# Request getPossibleEquipmentN

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:con="http://sphinx.dat.de/services/ConversionFunctionsService">
   <soapenv:Header/>
   <soapenv:Body>
      <con:getPossibleEquipmentN>
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
      </con:getPossibleEquipmentN>
   </soapenv:Body>
</soapenv:Envelope>
```
