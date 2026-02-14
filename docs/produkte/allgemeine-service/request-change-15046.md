---
title: "Request changeDossierN"
topic_id: "15046"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Aendern eines Vorgangs > Request changeDossierN"
---

# Request changeDossierN

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N" xmlns:vxs="http://www.dat.de/vxs">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:changeDossierN>
         <vxs:Dossier>
            <vxs:DossierId>2539149</vxs:DossierId>
            <vxs:Language>de_DE</vxs:Language>
            <vxs:Name>name change</vxs:Name>
            <vxs:Valuation>
               <vxs:Condition>
                  <vxs:NumberOfOwnersN>5</vxs:NumberOfOwnersN>
               </vxs:Condition>
            </vxs:Valuation>
         </vxs:Dossier>
      </dos:changeDossierN>
   </soapenv:Body>
</soapenv:Envelope>
```
