---
title: "Request getValuationN - variant with incomplete vehicle identification"
topic_id: "15198"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Verwalten von Vorgängen > Holen einer Bewertung > Request getValuationN - variant with incomplete vehicle identification"
---

# Request getValuationN - variant with incomplete vehicle identification

###### Request getValuationN - variant with incomplete vehicle identification ``` <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:val="http://www.dat.eu/myClaim/soap/v2/ValuationServiceN">    <soapenv:Header/>    <soapenv:Body>       <val:getValuationN>          <contractID>1292281</contractID>          <!--Optional:-->          <Coverage>NOVALUATIONRESULT</Coverage>       </val:getValuationN>    </soapenv:Body> </soapenv:Envelope> ```
