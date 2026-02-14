---
title: "Request createValuationN  mit zu hoher Laufleistung"
topic_id: "24853"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Verwalten von Vorgängen > Erstellen einer neuen Bewertung in der Anwendung > Request createValuationN  mit zu hoher Laufleistung"
---

# Request createValuationN  mit zu hoher Laufleistung

###### Request createValuationN mit zu hoher Laufleistung ``` <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:val="http://www.dat.eu/myClaim/soap/v2/ValuationServiceN" xmlns:vxs="http://www.dat.de/vxs">    <soapenv:Header/>    <soapenv:Body>       <val:createValuationN>          <contractType>bundle_valuation</contractType>          <networkType>DAT</networkType>          <vxs:Dossier overwrite="true">             <vxs:Name>datMileageCorr, milage too high</vxs:Name>             <vxs:Language>de_DE</vxs:Language>             <vxs:Country>DE</vxs:Country>             <vxs:Currency>EUR</vxs:Currency>             <vxs:Vehicle>                <vxs:DatECode>045700670030013</vxs:DatECode>                <vxs:Container>DE001</vxs:Container>                <vxs:ConstructionTime>4273</vxs:ConstructionTime>                <vxs:InitialRegistration>2005-10-07</vxs:InitialRegistration>                <vxs:MileageEstimated>2010000</vxs:MileageEstimated>                <vxs:Country>DE</vxs:Country>             </vxs:Vehicle>             <vxs:VAT>                <vxs:VatType>regular</vxs:VatType>             </vxs:VAT>          </vxs:Dossier>          <Coverage>COMPLETE</Coverage>       </val:createValuationN>    </soapenv:Body> </soapenv:Envelope> ```
