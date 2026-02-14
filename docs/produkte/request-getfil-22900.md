---
title: "Request getFillingQuantities"
topic_id: "22900"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > Abrufen der Füllmengen anhand des DAT €urope-Codes > Request getFillingQuantities"
---

# Request getFillingQuantities

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://www.dat.eu/myClaim/soap/v2/VehicleRepairService">
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
