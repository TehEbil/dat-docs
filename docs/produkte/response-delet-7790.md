---
title: "Response deleteDossier"
topic_id: "7790"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Löschen eines Dossiers/Vorgangs > Response deleteDossier"
---

# Response deleteDossier

```
<!--Sample response if request was successful-->
<S:Envelope xm<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns8:deleteDossierResponse xmlns:ns8="http://sphinx.dat.de/services/VehicleRepairService">
         <ns1:success xmlns:ns1="http://www.dat.de/vxs">true</ns1:success>
      </ns8:deleteDossierResponse>
   </S:Body>
</S:Envelope>


<!--Sample response if request was not successful-->
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <S:Fault>
         <faultcode xmlns:dat="http://www.dat.de">dat:Error deleting dessier:</faultcode>
         <faultstring>Process not found.</faultstring>
         <faultactor>de.dat.sphinx.vehiclerepair.ws.server.VehicleRepairService</faultactor>
      </S:Fault>
   </S:Body>
</S:Envelope>
```
