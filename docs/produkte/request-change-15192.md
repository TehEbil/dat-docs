---
title: "Request changeValuationN - standard case"
topic_id: "15192"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Verwalten von Vorgängen > Ändern einer Bewertung > Request changeValuationN - standard case"
---

# Request changeValuationN - standard case

###### Request changeValuationN - standard case ``` <!-- SilverDAT 3 PRO sample --> <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:val="http://www.dat.eu/myClaim/soap/v2/ValuationServiceN" xmlns:vxs="http://www.dat.de/vxs"> <soapenv:Header/>    <soapenv:Body>       <val:changeValuationN>          <!-- mandatory process ID -->          <contractID>123456789</contractID>          <!-- mandatory dossier -->          <vxs:Dossier overwrite="true">             <!-- optional name of contract -->             <vxs:Name>SampleDossier</vxs:Name>             <vxs:Vehicle>                <vxs:RegistrationData>                   <vxs:LicenseNumber>B CHANGE 1</vxs:LicenseNumber>                </vxs:RegistrationData>             </vxs:Vehicle>          </vxs:Dossier>          <!--optional data volume-->          <Coverage>COMPLETE</Coverage>       </val:changeValuationN>    </soapenv:Body> </soapenv:Envelope> ```
