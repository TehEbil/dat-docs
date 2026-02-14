---
title: "Request getDVNEquipments"
topic_id: "1318"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > Abruf von Ausstattungen zu DVN > Request getDVNEquipments"
---

# Request getDVNEquipments

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://www.dat.eu/myClaim/soap/v2/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getDVNEquipments>
         <!--Optional:-->
         <request>
            <constructionTime>4930</constructionTime>             
            <datECode>010600110010001</datECode>             
            <!--1 or more repetitions:-->            
            <datProcessIds>30711</datProcessIds>             
            <datProcessIds>32741</datProcessIds>             
            <locale country="DE" datCountryIndicator="DE" language="de"/> 
         </request>
      </veh:getDVNEquipments>
   </soapenv:Body>
</soapenv:Envelope>
```
