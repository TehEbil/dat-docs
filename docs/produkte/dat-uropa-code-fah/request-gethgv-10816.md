---
title: "Request getHgvPlatformAggregateModelData"
topic_id: "10816"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getHgvPlatformAggregateModelData > Request getHgvPlatformAggregateModelData"
---

# Request getHgvPlatformAggregateModelData

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
  <soapenv:Header/>
  <soapenv:Body>
    <veh:getHgvPlatformAggregateModelData>
      <request>
        <locale country="de" datCountryIndicator="de" language="de"/>
        <manufacturer>2</manufacturer>
        <model>2</model>
      </request>
    </veh:getHgvPlatformAggregateModelData>
  </soapenv:Body>
</soapenv:Envelope>
```
