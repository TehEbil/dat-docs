---
title: "Request getPossibleEquipment"
topic_id: "31546"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getPossibleEquipment > Request getPossibleEquipment"
---

# Request getPossibleEquipment

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:con="http://sphinx.dat.de/services/VehicleSelectionService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getPossibleEquipment>
         <request>
            <locale country="de" datCountryIndicator="de" language="de"/>
            <!--type: releaseRestriction - enumeration: [ALL,REPAIR,APPRAISAL]-->
            <restriction>ALL</restriction>
            <!--type: string-->
            <datECode>019051740220001</datECode>
            <!--Optional:-->
            <!--type: string-->
            <container>DE001</container>
            <!--type: int-->
            <constructionTime>6539</constructionTime>
         </request>
      </veh:getPossibleEquipment>
   </soapenv:Body>
</soapenv:Envelope>
```
