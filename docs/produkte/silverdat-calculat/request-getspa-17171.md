---
title: "Request getSparePartsDetailsForDPNByVIN"
topic_id: "17171"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, Ersatzteilnummer und Preishistorie > Request getSparePartsDetailsForDPNByVIN"
---

# Request getSparePartsDetailsForDPNByVIN

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getSparePartsDetailsForDPNByVIN>
         <!--Optional:-->
         <request>
            <!--1 or more repetitions:-->
            <datProcessNo>44210</datProcessNo>
            <locale country="DE" datCountryIndicator="DE" language="DE"/>
            <vin>WVWDEXTESTSTUB001</vin>
         </request>
      </veh:getSparePartsDetailsForDPNByVIN>
   </soapenv:Body>
</soapenv:Envelope>
```
