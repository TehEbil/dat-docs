---
title: "Response getLossOfUseDatabyVIN"
topic_id: "7725"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Nutzungsausfalldaten anhand der VIN ermitteln > Response getLossOfUseDatabyVIN"
---

# Response getLossOfUseDatabyVIN

```
<!-- response example if request was successful-->
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns3:getLossOfUseDatabyVINResponse xmlns:ns3="http://sphinx.dat.de/services/RentalPricesService">
         <RentalVehicleResponse>
            <contingencyCostsPerDay>24.83</contingencyCostsPerDay>
            <lossOfUseClass>J</lossOfUseClass>
            <lossOfUseClassExcVehAge>J</lossOfUseClassExcVehAge>
            <lossOfUsePerDay>79.00</lossOfUsePerDay>
         </RentalVehicleResponse>
      </ns3:getLossOfUseDatabyVINResponse>
   </S:Body>
</S:Envelope>

<!-- response example if request was not successful-->
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <S:Fault>
         <faultcode xmlns:dat="http://www.dat.de">dat:validation.firstRegistration.invalid</faultcode>
         <faultstring>Erstzulassung fehlt oder ist ungültig</faultstring>
         <faultactor>de.dat.sphinx.rentalpricesmod.ws.RentalPricesSoapHelper</faultactor>
      </S:Fault>
   </S:Body>
</S:Envelope>
```
