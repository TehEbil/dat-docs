---
title: "Request calculateContract"
topic_id: "18907"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > (Nach-) Kalkulieren eines bestehenden Vorgangs > Request calculateContract"
---

# Request calculateContract

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://www.dat.eu/myClaim/soap/v2/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:calculateContract>
         <!--Optional:-->
         <request>
            <contractID>99999999</contractID>
            <!--Optional:-->
            <includeAttachments>false</includeAttachments>
            <!--Optional:-->
            <locale country="DE" datCountryIndicator="DE" language="de"/>
         </request>
      </veh:calculateContract>
   </soapenv:Body>
</soapenv:Envelope>
```
