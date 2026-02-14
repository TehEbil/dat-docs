---
title: "Response getLockedInfo"
topic_id: "2476"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abfrage des Bearbeitungsstatus/ -benutzer eines Vorgangs > Response getLockedInfo"
---

# Response getLockedInfo

```
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns2:getLockedInfoResponse xmlns:ns2="http://sphinx.dat.de/services/VehicleRepairService" xmlns:ns3="http://www.dat.de/vxs">
         <!--Wenn einen Benutzer einen Kalkulation noch bearbeitet:-->      
         <lockedInfo>"Mustermann, Max"</lockedInfo>
      </ns2:getLockedInfoResponse>
   </S:Body>
</S:Envelope>
```
