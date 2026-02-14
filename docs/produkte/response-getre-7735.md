---
title: "Response getRentalOffersbyVIN"
topic_id: "7735"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Mietwagenpreise anhand der VIN und PLZ ermitteln > Response getRentalOffersbyVIN"
---

# Response getRentalOffersbyVIN

```
<!-- response example if request was successful-->
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns3:getRentalOffersbyVINResponse xmlns:ns3="http://sphinx.dat.de/services/RentalPricesService">
         <RentalVehicleOffersResponse>
            <CDWAverageDeductible>1276.00</CDWAverageDeductible>
            <Offers>
               <CurrencyType>EUR</CurrencyType>
               <Max>427.21</Max>
               <Mean>238.82</Mean>
               <Min>155.00</Min>
               <OffersType>1 day costs</OffersType>
               <PriceType>GROSS</PriceType>
            </Offers>
            <Offers>
               <CurrencyType>EUR</CurrencyType>
               <Max>1281.63</Max>
               <Mean>667.22</Mean>
               <Min>433.99</Min>
               <OffersType>3 days costs</OffersType>
               <PriceType>GROSS</PriceType>
            </Offers>
            <Offers>
               <CurrencyType>EUR</CurrencyType>
               <Max>2990.47</Max>
               <Mean>1237.62</Mean>
               <Min>543.00</Min>
               <OffersType>1 week costs</OffersType>
               <PriceType>GROSS</PriceType>
            </Offers>
            <rentalOffersNumber>98</rentalOffersNumber>
         </RentalVehicleOffersResponse>
      </ns3:getRentalOffersbyVINResponse>
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
