---
title: "Request setContractPriceGeneration"
topic_id: "1328"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > Änderung eines Preisstands eines Vorgangs > Request setContractPriceGeneration"
---

# Request setContractPriceGeneration

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://www.dat.eu/myClaim/soap/v2/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:setContractPriceGeneration>
         <request>
            <contractId>9999999</contractId>
            <generation>2</generation>
            <removeResult>true</removeResult>
         </request>
      </veh:setContractPriceGeneration>
   </soapenv:Body>
</soapenv:Envelope>
```
