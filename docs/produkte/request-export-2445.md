---
title: "Request exportDossierToDocument"
topic_id: "2445"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Exportieren von Dokumenten > Request exportDossierToDocument"
---

# Request exportDossierToDocument

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:exportDossierToDocument>
         <!--Optional:-->
         <dossierID>999999</dossierID>
         <!--Optional:-->
         <locale country="DE" datCountryIndicator="DE" language="de"/>
         <!--Mögliche Werte: PDF" | "DOCX" |" HTML -->
         <format>DOCX</format>
         <!--Optional:-->
         <product>VRO_CALC_RESULT</product>
      </veh:exportDossierToDocument>
   </soapenv:Body>
</soapenv:Envelope>
```
