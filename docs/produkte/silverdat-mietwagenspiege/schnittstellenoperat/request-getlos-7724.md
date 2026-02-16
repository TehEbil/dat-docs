---
title: "Request getLossOfUseDatabyVIN"
topic_id: "7724"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Nutzungsausfalldaten anhand der VIN ermitteln > Request getLossOfUseDatabyVIN"
---

# Request getLossOfUseDatabyVIN

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ren="http://sphinx.dat.de/services/RentalPricesService">
   <soapenv:Header/>
   <soapenv:Body>
      <ren:getLossOfUseDatabyVIN>
         <request>
            <!--Optional:-->
            <beginnigOfRental>2017-05-01</beginnigOfRental>
            <!--Optional:-->
            <endOfRental>2017-05-07</endOfRental>
            <firstRegistration>2012-10-01</firstRegistration>
            <VIN>ZFADEXTESTSTUB001</VIN>
         </request>
      </ren:getLossOfUseDatabyVIN>
   </soapenv:Body>
</soapenv:Envelope>
```
