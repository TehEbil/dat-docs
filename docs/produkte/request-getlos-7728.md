---
title: "Request getLossOfUseDatabyDATECode"
topic_id: "7728"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Nutzungsausfalldaten anhand DAT €uropa-Code® ermitteln > Request getLossOfUseDatabyDATECode"
---

# Request getLossOfUseDatabyDATECode

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ren="http://sphinx.dat.de/services/RentalPricesService">
   <soapenv:Header/>
   <soapenv:Body>
      <ren:getLossOfUseDatabyDATECode>
         <request>
            <beginnigOfRental>2017-05-01</beginnigOfRental>
            <DATECode>019051080040002DE002</DATECode>
            <endOfRental>2017-05-07</endOfRental>
            <firstRegistration>2015-01-21</firstRegistration>
         </request>
      </ren:getLossOfUseDatabyDATECode>
   </soapenv:Body>
</soapenv:Envelope>
```
