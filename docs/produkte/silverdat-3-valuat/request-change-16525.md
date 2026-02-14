---
title: "Request changeDossierN unvollstaendiges Aktenzeichen"
topic_id: "16525"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Unvollständiges Aktenzeichen > Verwalten von unvollstaendigen Aktenzeichen > Aendern eines unvollstaendigen Aktenzeichens > Request changeDossierN unvollstaendiges Aktenzeichen"
---

# Request changeDossierN unvollstaendiges Aktenzeichen

###### Request changeDossierN unvollstaendiges Aktenzeichen ``` <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1" xmlns:vxs="http://www.dat.de/vxs">    <soapenv:Header/>    <soapenv:Body>       <dos:changeDossierN>          <vxs:Dossier>             <vxs:DossierId>1234567</vxs:DossierId>             <vxs:Name>changed IncompleteDossier</vxs:Name>             <vxs:Country>DE</vxs:Country>             <vxs:Language>de_DE</vxs:Language>             <vxs:Vehicle>                <vxs:VehicleIdentNumber/>                <vxs:Container>DE002</vxs:Container>                <vxs:ConstructionTime>5438</vxs:ConstructionTime>                <vxs:InitialRegistration>2015-03-25</vxs:InitialRegistration>                <vxs:MileageEstimated>86000</vxs:MileageEstimated>                <vxs:Country>DE</vxs:Country>                <vxs:RegistrationData>                   <vxs:LicenseNumber>ES DAT 123</vxs:LicenseNumber>                </vxs:RegistrationData>             </vxs:Vehicle>          </vxs:Dossier>          <Coverage>NOVALUATIONRESULT</Coverage>          <Save>true</Save>       </dos:changeDossierN>    </soapenv:Body> </soapenv:Envelope> ```
