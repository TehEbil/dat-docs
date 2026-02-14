---
title: "Request resetValuation2defaultN"
topic_id: "15218"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Verwalten von Vorgängen > Zurücksetzen einer Bewertung auf die DAT Standardeinstellungen > Request resetValuation2defaultN"
---

# Request resetValuation2defaultN

###### Request resetValuation2defaultN ``` <!-- SilverDAT 3 PRO sample --> <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:val="http://www.dat.eu/myClaim/soap/v2/ValuationServiceN">    <soapenv:Header/>    <soapenv:Body>       <val:resetValuation2defaultN>          <!-- mandatory process ID -->          <contractID>1291993</contractID>       </val:resetValuation2defaultN>    </soapenv:Body> </soapenv:Envelope> ```
