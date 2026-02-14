---
title: "Request getVehicleImagesN"
topic_id: "6809"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugbilder Funktionen > getVehicleImagesN > Request getVehicleImagesN"
---

# Request getVehicleImagesN

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleImagery">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getVehicleImagesN>
         <request>
            <datECode>019050880010001</datECode>
            <imageType>PICTURE</imageType>
            <aspect>SIDEVIEW</aspect>
            <aspect>ANGULARFRONT</aspect>
         </request>
      </veh:getVehicleImagesN>
   </soapenv:Body>
</soapenv:Envelope>
```
