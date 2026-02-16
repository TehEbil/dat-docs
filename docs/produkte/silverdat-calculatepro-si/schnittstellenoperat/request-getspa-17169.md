---
title: "Request getSparePartsDetailsByVIN"
topic_id: "17169"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, DVNs und Preishistorie > Request getSparePartsDetailsByVIN"
---

# Request getSparePartsDetailsByVIN

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getSparePartsDetailsByVIN>
         <!--Optional:-->
         <request>
            <locale country="DE" datCountryIndicator="DE" language="de"/>
            <!--1 or more repetitions:-->
            <sparePartNo>4517250100</sparePartNo>
            <vin>WME4514321K600778</vin>
         </request>
      </veh:getSparePartsDetailsByVIN>
   </soapenv:Body>
</soapenv:Envelope>
```
