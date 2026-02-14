---
title: "Request getLastPriceGenerationByMfr"
topic_id: "9196"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abfrage letzter Preisstand eines Herstellers > Request getLastPriceGenerationByMfr"
---

# Request getLastPriceGenerationByMfr

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getLastPriceGenerationByMfr>
         <manufacturer>130</manufacturer>
         <!--Optional:--> 
         <generation>1</generation>
      </veh:getLastPriceGenerationByMfr>
   </soapenv:Body>
</soapenv:Envelope>
```
