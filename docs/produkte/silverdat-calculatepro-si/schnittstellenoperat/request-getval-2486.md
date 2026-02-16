---
title: "Request getValidDATProcesses"
topic_id: "2486"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abfragen von DVNs anhand von DAT €uropa-Code, Bauzeit und AVs > Request getValidDATProcesses"
---

# Request getValidDATProcesses

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getValidDATProcesses>
         <!--Optional:-->
         <request>
            <!--Optional:-->
            <constructionTime>4567</constructionTime>
            <datECode>011300450230003</datECode>
            <!--Zero or more repetitions:-->
            <equipment>40802</equipment>
            <!--Optional:-->
            <locale country="DE" datCountryIndicator="DE" language="de"/>
            <!--Optional:-->
            <coverage>WITH_MAINTANCE</coverage>
         </request>
      </veh:getValidDATProcesses>
   </soapenv:Body>
</soapenv:Envelope>
```
