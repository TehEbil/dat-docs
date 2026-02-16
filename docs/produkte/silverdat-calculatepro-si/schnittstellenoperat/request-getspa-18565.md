---
title: "Request getSparePartVariants"
topic_id: "18565"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abruf aller Ersatzteilevarianten > Request getSparePartVariants"
---

# Request getSparePartVariants

```
<?xml version="1.0" encoding="UTF-8"?>
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getSparePartVariants>
         <!--Optional:-->
         <request>
            <!--Optional:-->
            <constructionTime>9999</constructionTime>
            <datECode>011300570140001</datECode>
            <datProcessId>44910</datProcessId>
            <!--Zero or more repetitions:-->
            <equipment/>
            <locale country="DE" datCountryIndicator="DE" language="de"/>
            <!--Zero or more repetitions:-->
            <manufacturerCode>130</manufacturerCode>
            <!--Optional:-->
            <vin/>
         </request>
      </veh:getSparePartVariants>
   </soapenv:Body>
</soapenv:Envelope>
```
