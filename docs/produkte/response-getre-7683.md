---
title: "Response getRentalCarClassbyVIN"
topic_id: "7683"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Mietwagenklasse anhand der VIN ermitteln > Response getRentalCarClassbyVIN"
---

# Response getRentalCarClassbyVIN

```
<!-- response example if request was successful-->
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns4:getRentalCarClassbyVINResponse xmlns:ns4="http://sphinx.dat.de/services/RentalPricesService">
         <return>10</return>
      </ns4:getRentalCarClassbyVINResponse>
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
