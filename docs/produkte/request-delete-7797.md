---
title: "Request deleteDossier"
topic_id: "7797"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Löschen eines Dossiers/Vorgangs > Request deleteDossier"
---

# Request deleteDossier

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:deleteDossier>
         <!--Optional:-->
         <DossierId>9999999</DossierId>
      </veh:deleteDossier>
   </soapenv:Body>
</soapenv:Envelope>
```
