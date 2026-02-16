---
title: "Request getTemplates"
topic_id: "2480"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abruf aller existierenden Druckvorlagen > Request getTemplates"
---

# Request getTemplates

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getTemplates>
         <!--Optional:-->
         <locale country="DE" datCountryIndicator="DE" language="de"/>
      </veh:getTemplates>
   </soapenv:Body>
</soapenv:Envelope>
```
