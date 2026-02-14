---
title: "Request getHgvPlatformBaseModels"
topic_id: "10796"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getHgvPlatformBaseModels > Request getHgvPlatformBaseModels"
---

# Request getHgvPlatformBaseModels

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
  <soapenv:Header/>
  <soapenv:Body>
    <veh:getHgvPlatformBaseModels>
      <request>
        <locale country="de" datCountryIndicator="de" language="de"/>
        <restriction>APPRAISAL</restriction>
        <hgvPlatformType>20</hgvPlatformType>
        <manufacturer>999</manufacturer>
      </request>
    </veh:getHgvPlatformBaseModels>
  </soapenv:Body>
</soapenv:Envelope>
```
