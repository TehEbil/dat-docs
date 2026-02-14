---
title: "Request getMaintenanceIntervals"
topic_id: "1324"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > Abruf von Wartungsintervallen: getMaintenanceIntervals > Request getMaintenanceIntervals"
---

# Request getMaintenanceIntervals

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://www.dat.eu/myClaim/soap/v2/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getMaintenanceIntervals>
         <!--Optional:-->
         <request>
            <!--Optional:-->
            <constructionTime>5297</constructionTime>
            <datECode>011301110300002</datECode>
            <!--Zero or more repetitions:-->
            <equipment>87410</equipment>
            <!--Optional:-->
            <locale country="DE" datCountryIndicator="DE" language="de"/>
         </request>´
      </veh:getMaintenanceIntervals>
   </soapenv:Body>
</soapenv:Envelope>
```
