---
title: "Request getContract"
topic_id: "2457"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abrufen eines bestimmten Vorgangs > Request getContract"
---

# Request getContract

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getContract>
         <!--Optional:-->
         <request>
            <contractID>999999</contractID>
            <!--Optional:-->
            <includeProtocol>true</includeProtocol>
            <!--Optional:-->
            <locale country="DE" datCountryIndicator="DE" language="de"/>
         </request>
      </veh:getContract>
   </soapenv:Body>
</soapenv:Envelope>
```
