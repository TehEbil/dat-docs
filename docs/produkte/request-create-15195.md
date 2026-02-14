---
title: "Request createValuationN - variant with incomplete vehicle identification"
topic_id: "15195"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Verwalten von Vorgängen > Erstellen einer neuen Bewertung in der Anwendung > Request createValuationN - variant with incomplete vehicle identification"
---

# Request createValuationN - variant with incomplete vehicle identification

###### Request createValuationN - variant with incomplete vehicle identification ``` <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:val="http://www.dat.eu/myClaim/soap/v2/ValuationServiceN" xmlns:vxs="http://www.dat.de/vxs">    <soapenv:Header/>    <soapenv:Body>       <val:createValuationN>          <contractId/>          <contractType>bundle_valuation</contractType>          <networkType>DAT</networkType>          <vxs:Dossier overwrite="true">             <vxs:Name>DAT-TEST_16:43:14,379</vxs:Name>             <vxs:Country>DE</vxs:Country>             <vxs:Language>de_DE</vxs:Language>             <vxs:Currency>EUR</vxs:Currency>             <vxs:Vehicle>                <vxs:DatECode>019051080040002</vxs:DatECode>                <vxs:Container>DE002</vxs:Container>                <vxs:ConstructionTime>5419</vxs:ConstructionTime>                <vxs:InitialRegistration>2015-01-01</vxs:InitialRegistration>                <vxs:Country>DE</vxs:Country>             </vxs:Vehicle>          </vxs:Dossier>          <Coverage>NONE</Coverage>       </val:createValuationN>    </soapenv:Body> </soapenv:Envelope> ```
