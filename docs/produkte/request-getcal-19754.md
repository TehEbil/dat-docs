---
title: "Request getCalculationResultN"
topic_id: "19754"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abrufen eines Kalkulationsergebnisses > Request getCalculationResultN"
---

# Request getCalculationResultN

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getCalculationResultN>
         <request>
            <contractID>12345</contractID>
            <!--Optional:-->
            <locale country="DE" datCountryIndicator="DE" language="de"/>
         <!--Optional:-->
            <includeAttachments>true</includeAttachments>
            <!--Optional:-->
            <includeProtocol>true</includeProtocol>
         </request>
      </veh:getCalculationResultN>
   </soapenv:Body>
</soapenv:Envelope>
```
