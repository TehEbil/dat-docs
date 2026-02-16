---
title: "Response getLossOfUseDatabyDATECode"
topic_id: "7729"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Nutzungsausfalldaten anhand DAT €uropa-Code® ermitteln > Response getLossOfUseDatabyDATECode"
---

# Response getLossOfUseDatabyDATECode

```
<!-- response example if request was successful-->
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns4:getLossOfUseDatabyDATECodeResponse xmlns:ns4="http://sphinx.dat.de/services/RentalPricesService">
         <RentalVehicleResponse>
            <contingencyCostsPerDay>15.70</contingencyCostsPerDay>
            <lossOfUseClass>G</lossOfUseClass>
            <lossOfUseClassExcVehAge>G</lossOfUseClassExcVehAge>
            <lossOfUsePerDay>59.00</lossOfUsePerDay>
         </RentalVehicleResponse>
      </ns4:getLossOfUseDatabyDATECodeResponse>
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
