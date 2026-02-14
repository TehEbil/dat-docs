---
title: "Request calculateContract"
topic_id: "18902"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > (Nach-) Kalkulieren eines bestehenden Vorgangs > Request calculateContract"
---

# Request calculateContract

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:calculateContract>
         <!--Optional:-->
         <request>
            <contractID>3512829</contractID>
            <!--Optional:-->
            <includeAttachments>false</includeAttachments>
            <!--Optional:-->
            <locale country="DE" datCountryIndicator="DE" language="de"/>
         </request>
      </veh:calculateContract>
   </soapenv:Body>
</soapenv:Envelope>
```
