---
title: "Request getInsurances"
topic_id: "1320"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > Abrufen von länderspezifischen Versicherungen > Request getInsurances"
---

# Request getInsurances

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://www.dat.eu/myClaim/soap/v2/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getInsurances>
         <request>
            <locale country="DE" datCountryIndicator="DE" language="de"/>
         </request>
      </veh:getInsurances>
   </soapenv:Body>
</soapenv:Envelope>
```
