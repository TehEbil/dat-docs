---
title: "Request getRentalOffersbyVIN"
topic_id: "7733"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Mietwagenpreise anhand der VIN und PLZ ermitteln > Request getRentalOffersbyVIN"
---

# Request getRentalOffersbyVIN

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ren="http://sphinx.dat.de/services/RentalPricesService">
   <soapenv:Header/>
   <soapenv:Body>
      <ren:getRentalOffersbyVIN>
         <request>
            <!--Optional:-->
            <beginnigOfRental>2017-05-01</beginnigOfRental>
            <!--Optional:-->
            <duration>7</duration>
            <!--Optional:-->
            <endOfRental>2017-05-07</endOfRental>
            <firstRegistration>2012-10-01</firstRegistration>
            <postalCode>10965</postalCode>
            <!--Optional:-->
            <radius>10</radius>
            <VIN>ZFADEXTESTSTUB001</VIN>
         </request>
      </ren:getRentalOffersbyVIN>
   </soapenv:Body>
</soapenv:Envelope>
```
