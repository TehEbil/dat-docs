---
title: "Request getLacquerTypeKeys"
topic_id: "2472"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abrufen von Lackartschlüsseln > Request getLacquerTypeKeys"
---

# Request getLacquerTypeKeys

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getLacquerTypeKeys>
         <request>
            <!--Optional:-->
            <locale country="DE" datCountryIndicator="DE" language="de"/>
            <!--Optional:-->
            <vehicleType>1</vehicleType>
            <!--Optional:-->
            <manufacturer>905</manufacturer>
            <!--Optional:-->
            <mainType>85</mainType>
            <paintMethod>EURO_LACQUER</paintMethod>
         </request>
      </veh:getLacquerTypeKeys>
   </soapenv:Body>
</soapenv:Envelope>
```
