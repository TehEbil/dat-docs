---
title: "Request getHgvPlatformSubModels"
topic_id: "10800"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getHgvPlatformSubModels > Request getHgvPlatformSubModels"
---

# Request getHgvPlatformSubModels

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
  <soapenv:Header/>
  <soapenv:Body>
    <veh:getHgvPlatformSubModels>
      <request>
        <locale country="de" datCountryIndicator="de" language="de"/>
        <restriction>APPRAISAL</restriction>
        <hgvPlatformType>20</hgvPlatformType>
        <manufacturer>999</manufacturer>
        <baseModel>1</baseModel>
      </request>
    </veh:getHgvPlatformSubModels>
  </soapenv:Body>
</soapenv:Envelope>
```
