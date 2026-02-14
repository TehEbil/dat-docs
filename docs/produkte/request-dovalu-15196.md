---
title: "Request doValuationInMemoryN"
topic_id: "15196"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Verwalten von Vorgängen > Erstellen einer Bewertung im Speicher > Request doValuationInMemoryN"
---

# Request doValuationInMemoryN

###### Request doValuationInMemoryN ``` <!-- SilverDAT 3 PRO sample --> <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:val="http://www.dat.eu/myClaim/soap/v2/ValuationServiceN" xmlns:vxs="http://www.dat.de/vxs">    <soapenv:Header/>    <soapenv:Body>       <val:doValuationInMemoryN>          <vxs:Dossier overwrite="true">             <!-- mandatory Language -->             <vxs:Language>de_DE</vxs:Language>             <vxs:Vehicle>                <!--mandatory; datECode -->                <vxs:DatECode>015700381600001</vxs:DatECode>                <!--mandatory; container -->                <vxs:Container>DE001</vxs:Container>                <!--mandatory; construction time -->                <vxs:ConstructionTime>5475</vxs:ConstructionTime>                <!--mandatory; initial registration-->                <vxs:InitialRegistration>2015-10-22+02:00</vxs:InitialRegistration>                <!--mandatory; milage-->                <vxs:MileageEstimated>25000</vxs:MileageEstimated>                <vxs:Country>DE</vxs:Country>                <vxs:RegistrationData>                   <!-- optional set the license number -->                   <vxs:LicenseNumber>S DAT 123</vxs:LicenseNumber>                </vxs:RegistrationData>             </vxs:Vehicle>            </vxs:Dossier>          <!--optional data volume-->          <Coverage>COMPLETE</Coverage>       </val:doValuationInMemoryN>    </soapenv:Body> </soapenv:Envelope> ```
