---
title: "Request createDossierN mit zu hoher Laufleistung"
topic_id: "24850"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Erstellen eines neuen Vorgangs > Request createDossierN mit zu hoher Laufleistung"
---

# Request createDossierN mit zu hoher Laufleistung

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N" xmlns:vxs="http://www.dat.de/vxs">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:createDossierN>
         <vxs:Dossier overwrite="true">
            <vxs:Name>datMileageCorr, milage too high (truck)</vxs:Name>
            <vxs:Language>de_DE</vxs:Language>
            <vxs:Country>DE</vxs:Country>
            <vxs:Currency></vxs:Currency>
            <vxs:Vehicle>
               <vxs:DatECode>045700670030013</vxs:DatECode>
               <vxs:Container>DE001</vxs:Container>
               <vxs:ConstructionTime>4273</vxs:ConstructionTime>
               <vxs:InitialRegistration>2005-10-07</vxs:InitialRegistration>
               <vxs:MileageEstimated>2010000</vxs:MileageEstimated>
               <vxs:Country>DE</vxs:Country>
            </vxs:Vehicle>
         </vxs:Dossier>
         <Save>false</Save>
      </dos:createDossierN>
   </soapenv:Body>
</soapenv:Envelope>
```
