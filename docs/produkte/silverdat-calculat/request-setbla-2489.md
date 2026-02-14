---
title: "Request setBlanketCalculation"
topic_id: "2489"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Festlegen von Überschläge Kalkulationswerte > Request setBlanketCalculation"
---

# Request setBlanketCalculation

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:setBlanketCalculation>
         <!--Optional:-->
         <request>
            <dossierId>999999</dossierId>
            <!--Optional:-->
            <labourCosts>2.00</labourCosts>
            <!--Optional:-->
            <lacquerCosts>1</lacquerCosts>
            <!--Optional:-->
            <sparePartsCosts>2</sparePartsCosts>
         </request>
      </veh:setBlanketCalculation>
   </soapenv:Body>
</soapenv:Envelope>
```
