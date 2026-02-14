---
title: "Request getValuationN - with Marketplace data"
topic_id: "25352"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Verwalten von Vorgängen > Holen einer Bewertung > Request getValuationN - with Marketplace data"
---

# Request getValuationN - with Marketplace data

###### Request getValuationN - with Marketplace data ``` <!-- SilverDAT 3 PRO sample --> <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:val="http://www.dat.eu/myClaim/soap/v2/ValuationServiceN">    <soapenv:Header/>    <soapenv:Body>       <val:getValuationN>          <!-- get the process via ID -->          <contractID>1291993</contractID>          <!-- with entire data volume -->          <Coverage>MARKETPLACEEXPORT</Coverage>       </val:getValuationN>    </soapenv:Body> </soapenv:Envelope> ```
