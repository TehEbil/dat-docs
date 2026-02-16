---
title: "Request getLacquerTypeKeys"
topic_id: "1322"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > Abrufen von Lackartschlüsseln > Request getLacquerTypeKeys"
---

# Request getLacquerTypeKeys

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://www.dat.eu/myClaim/soap/v2/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getLacquerTypeKeys>
     <request>
            <!--Optional:-->
            <locale country="DE" datCountryIndicator="DE" language="de"/>
            <!--Optional:-->
            <mainType>85</mainType>
            <!--Optional:-->
            <manufacturer>905</manufacturer>
            <paintMethod>EURO_LACQUER</paintMethod>
            <!--Optional:-->
            <vehicleType>1</vehicleType>
         </request>
      </veh:getLacquerTypeKeys>
   </soapenv:Body>
</soapenv:Envelope>
```
