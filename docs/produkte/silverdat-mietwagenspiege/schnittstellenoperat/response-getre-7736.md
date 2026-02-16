---
title: "Response getRentalOffersbyDATECode"
topic_id: "7736"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Mietwagenpreise anhand des DAT €uropa-Code® und PLZ ermitteln > Response getRentalOffersbyDATECode"
---

# Response getRentalOffersbyDATECode

```
<!-- response example if request was successful-->
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns3:getRentalOffersbyDATECodeResponse xmlns:ns3="http://sphinx.dat.de/services/RentalPricesService">
         <RentalVehicleOffersResponse>
            <CDWAverageDeductible>1180.00</CDWAverageDeductible>
            <Offers>
               <CurrencyType>EUR</CurrencyType>
               <Max>229.93</Max>
               <Mean>132.07</Mean>
               <Min>99.00</Min>
               <OffersType>1 day costs</OffersType>
               <PriceType>GROSS</PriceType>
            </Offers>
            <Offers>
               <CurrencyType>EUR</CurrencyType>
               <Max>689.80</Max>
               <Mean>374.40</Mean>
               <Min>296.99</Min>
               <OffersType>3 days costs</OffersType>
               <PriceType>GROSS</PriceType>
            </Offers>
            <Offers>
               <CurrencyType>EUR</CurrencyType>
               <Max>1609.52</Max>
               <Mean>671.62</Mean>
               <Min>415.00</Min>
               <OffersType>1 week costs</OffersType>
               <PriceType>GROSS</PriceType>
            </Offers>
            <rentalOffersNumber>131</rentalOffersNumber>
         </RentalVehicleOffersResponse>
      </ns3:getRentalOffersbyDATECodeResponse>
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
