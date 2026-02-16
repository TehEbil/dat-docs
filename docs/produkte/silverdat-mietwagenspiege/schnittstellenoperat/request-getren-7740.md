---
title: "Request getRentalOffersbyCarClass"
topic_id: "7740"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Mietwagenpreise anhand der Mietwagenklasse und PLZ ermitteln > Request getRentalOffersbyCarClass"
---

# Request getRentalOffersbyCarClass

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ren="http://sphinx.dat.de/services/RentalPricesService">
   <soapenv:Header/>
   <soapenv:Body>
      <ren:getRentalOffersbyCarClass>
         <request>
            <!--Optional:-->
            <beginnigOfRental>2017-05-01</beginnigOfRental>
            <!--Optional:-->
            <duration></duration>
            <!--Optional:-->
            <endOfRental>2017-05-07</endOfRental>
            <postalCode>10965</postalCode>
            <!--Optional:-->
            <radius>10</radius>
            <rentalCarClass>7</rentalCarClass>
         </request>
      </ren:getRentalOffersbyCarClass>
   </soapenv:Body>
</soapenv:Envelope>
```
