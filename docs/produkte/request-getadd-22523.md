---
title: "Request getAdditionalItems"
topic_id: "22523"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abrufen der Zusatzpositionen anhand des DAT €urope-Codes > Request getAdditionalItems"
---

# Request getAdditionalItems

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getAdditionalItems>
         <request>
            <locale country="DE" datCountryIndicator="DE" language="de"/>
            <datECode>011301110300002</datECode>
         </request>
      </veh:getAdditionalItems>
   </soapenv:Body>
</soapenv:Envelope>
```
