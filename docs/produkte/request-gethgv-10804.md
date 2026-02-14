---
title: "Request getHgvPlatformSubModelData"
topic_id: "10804"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getHgvPlatformSubModelData > Request getHgvPlatformSubModelData"
---

# Request getHgvPlatformSubModelData

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
  <soapenv:Header/>
  <soapenv:Body>
    <veh:getHgvPlatformSubModelData>
      <request>
        <locale country="de" datCountryIndicator="de" language="de"/>
        <restriction>APPRAISAL</restriction>
        <hgvPlatformType>20</hgvPlatformType>
        <manufacturer>999</manufacturer>
        <baseModel>1</baseModel>
        <subModel>1</subModel>
      </request>
    </veh:getHgvPlatformSubModelData>
  </soapenv:Body>
</soapenv:Envelope>
```
