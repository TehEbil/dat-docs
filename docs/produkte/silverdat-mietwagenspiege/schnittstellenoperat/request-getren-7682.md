---
title: "Request getRentalCarClassbyVIN"
topic_id: "7682"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Mietwagenklasse anhand der VIN ermitteln > Request getRentalCarClassbyVIN"
---

# Request getRentalCarClassbyVIN

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ren="http://sphinx.dat.de/services/RentalPricesService">
   <soapenv:Header/>
   <soapenv:Body>
      <ren:getRentalCarClassbyVIN>
         <request>
            <firstRegistration>2012-10-01</firstRegistration>
            <VIN>ZFADEXTESTSTUB001</VIN>
         </request>
      </ren:getRentalCarClassbyVIN>
   </soapenv:Body>
</soapenv:Envelope>
```
