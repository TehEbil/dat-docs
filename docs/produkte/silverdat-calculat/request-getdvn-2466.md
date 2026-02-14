---
title: "Request getDVNEquipments"
topic_id: "2466"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abruf von Ausstattungen zu DVN > Request getDVNEquipments"
---

# Request getDVNEquipments

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleRepairService/">
      <soapenv:Header>
         <soapenv:Header>
             DAT Authentication Header
         </soapenv:Header>
      </soapenv:Header>
      <soapenv:Body>
         <veh:getDVNEquipments>
            <veh:datECode></veh:datECode>
            <veh:manufacturerCode></veh:manufacturerCode>
            <veh:mainTypeCode></veh:mainTypeCode>
            <veh:subTypeCode></veh:subTypeCode>
            <veh:dvn></veh:dvn>
         </veh:getDVNEquipments>
      </soapenv:Body>
</soapenv:Envelope>
```
