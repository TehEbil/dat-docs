---
title: "Response getRentalCarClassbyDATECode"
topic_id: "7720"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Mietwagenklasse anhand des DAT €uropa-Code® ermitteln > Response getRentalCarClassbyDATECode"
---

# Response getRentalCarClassbyDATECode

```
<!-- response example if request was successful-->
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns3:getRentalCarClassbyDATECodeResponse xmlns:ns3="http://sphinx.dat.de/services/RentalPricesService">
         <return>7</return>
      </ns3:getRentalCarClassbyDATECodeResponse>
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
