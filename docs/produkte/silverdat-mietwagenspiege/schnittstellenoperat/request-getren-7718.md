---
title: "Request getRentalCarClassbyDATECode"
topic_id: "7718"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen > Mietwagenklasse anhand des DAT €uropa-Code® ermitteln > Request getRentalCarClassbyDATECode"
---

# Request getRentalCarClassbyDATECode

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:ren="http://sphinx.dat.de/services/RentalPricesService">
   <soapenv:Header/>
   <soapenv:Body>
      <ren:getRentalCarClassbyDATECode>
         <request>
            <DATECode>019051080040002DE002</DATECode>
            <firstRegistration>2015-01-01</firstRegistration>
         </request>
      </ren:getRentalCarClassbyDATECode>
   </soapenv:Body>
</soapenv:Envelope>
```
