---
title: "Request getHgvPlatformManufacturers"
topic_id: "10792"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getHgvPlatformManufacturers > Request getHgvPlatformManufacturers"
---

# Request getHgvPlatformManufacturers

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
  <soapenv:Header/>
  <soapenv:Body>
    <veh:getHgvPlatformManufacturers>
      <request>
        <locale country="de" datCountryIndicator="de" language="de"/>
        <restriction>APPRAISAL</restriction>
        <hgvPlatformType>20</hgvPlatformType>
      </request>
    </veh:getHgvPlatformManufacturers>
  </soapenv:Body>
</soapenv:Envelope>
```
