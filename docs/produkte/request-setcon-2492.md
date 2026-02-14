---
title: "Request setContractPriceGeneration"
topic_id: "2492"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Änderung eines Preisstands eines Vorgangs > Request setContractPriceGeneration"
---

# Request setContractPriceGeneration

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:setContractPriceGeneration>
         <request>
            <contractId>999999</contractId>
            <generation>3</generation>
            <removeResult>true</removeResult>
         </request>
      </veh:setContractPriceGeneration>
   </soapenv:Body>
</soapenv:Envelope>
```
