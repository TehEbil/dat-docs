---
title: "Request getFillingQuantities"
topic_id: "22894"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abrufen der Füllmengen anhand des DAT €urope-Codes > Request getFillingQuantities"
---

# Request getFillingQuantities

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getFillingQuantities>
         <request>
            <locale country="DE" datCountryIndicator="DE" language="de"/>
            <datECode>015700320150001</datECode>
         </request>
      </veh:getFillingQuantities>
   </soapenv:Body>
</soapenv:Envelope>
```
