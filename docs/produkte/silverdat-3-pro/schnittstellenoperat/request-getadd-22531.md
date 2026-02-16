---
title: "Request getAdditionalItems"
topic_id: "22531"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > Abrufen der Zusatzpositionen anhand des DAT €urope-Codes > Request getAdditionalItems"
---

# Request getAdditionalItems

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://www.dat.eu/myClaim/soap/v2/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getAdditionalItems>
         <request>
            <locale country="DE" datCountryIndicator="DE" language="de"/>
            <datECode>019051200350004</datECode>
         </request>
      </veh:getAdditionalItems>
   </soapenv:Body>
</soapenv:Envelope>
```
