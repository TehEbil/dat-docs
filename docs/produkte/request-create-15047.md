---
title: "Request createDossierN"
topic_id: "15047"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Erstellen eines neuen Vorgangs > Request createDossierN"
---

# Request createDossierN

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/${#Project#techpath}/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N" xmlns:vxs="http://www.dat.de/vxs">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:createDossierN>
         <vxs:Dossier>
            <vxs:Name>createDossierN example</vxs:Name>
            <vxs:Language>de_DE</vxs:Language>
            <vxs:Vehicle>
               <vxs:DatECode>010400850080003</vxs:DatECode>
               <vxs:Container>DE003</vxs:Container>
               <vxs:ConstructionTime>5410</vxs:ConstructionTime>
               <vxs:InitialRegistration>2014-06-01</vxs:InitialRegistration>
               <vxs:MileageEstimated>50000</vxs:MileageEstimated>
               <vxs:Country>DE</vxs:Country>
            </vxs:Vehicle>
            <vxs:VAT>
               <vxs:VatType>regular</vxs:VatType>
            </vxs:VAT>
            <vxs:Country/>
         </vxs:Dossier>
         <Coverage>COMPLETE</Coverage>
         <Save>true</Save>
      </dos:createDossierN>
   </soapenv:Body>
</soapenv:Envelope>
```
