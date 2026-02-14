---
title: "Request getInsurances"
topic_id: "2469"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abrufen von länderspezifischen Versicherungen > Request getInsurances"
---

# Request getInsurances

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleRepairService">
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
