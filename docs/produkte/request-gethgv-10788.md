---
title: "Request getHgvPlatformTypes"
topic_id: "10788"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getHgvPlatformTypes > Request getHgvPlatformTypes"
---

# Request getHgvPlatformTypes

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
  <soapenv:Header/>
  <soapenv:Body>
    <veh:getHgvPlatformTypes>
      <request>
        <locale country="de" datCountryIndicator="de" language="de"/>
        <restriction>APPRAISAL</restriction>
      </request>
    </veh:getHgvPlatformTypes>
  </soapenv:Body>
</soapenv:Envelope>
```
