---
title: "Request getEquipmentLineOptions"
topic_id: "1976"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getEquipmentLineOptions > Request getEquipmentLineOptions"
---

# Request getEquipmentLineOptions

```
 <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
    <soapenv:Header/>
    <soapenv:Body>
       <veh:getEquipmentLineOptions>
          <request>
             <locale country="de" datCountryIndicator="de" language="de"/>
             <restriction>ALL</restriction>
             <vehicleType>1</vehicleType>
             <manufacturer>570</manufacturer>
             <baseModel>40</baseModel>
             <subModel>63</subModel>
             <!--Zero or more repetitions:-->
             <availableOptions>87302</availableOptions>
          </request>
       </veh:getEquipmentLineOptions>
    </soapenv:Body>
 </soapenv:Envelope>
```
