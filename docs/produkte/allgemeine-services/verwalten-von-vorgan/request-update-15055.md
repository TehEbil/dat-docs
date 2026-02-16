---
title: "Request updateDossierN"
topic_id: "15055"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Aktualisieren eines Vorgangs ohne Wertänderung > Request updateDossierN"
---

# Request updateDossierN

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/DossierN">
   <soapenv:Header/>
   <soapenv:Body>
     <dos:updateDossierN>
         <DossierId>2539149</DossierId>
         <!--Optional:-->
         <Coverage>COMPLETE</Coverage>
      </dos:updateDossierN>
   </soapenv:Body>
</soapenv:Envelope>
```
