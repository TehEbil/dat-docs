---
title: "Request resetDossierTechDataN"
topic_id: "25262"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Zurücksetzen von technischen Daten eines Vorgangs auf die DAT-Vorgaben > Request resetDossierTechDataN"
---

# Request resetDossierTechDataN

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:resetDossierTechDataN>
         <DossierId>66463807</DossierId>
         <!--Optional:-->
         <Coverage>COMPLETE</Coverage>
      </dos:resetDossierTechDataN>
   </soapenv:Body>
</soapenv:Envelope>
```
