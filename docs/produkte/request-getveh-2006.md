---
title: "Request getVehicleIdentificationByCodeSwitzerland"
topic_id: "2006"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Fahrzeugidentifikation Schweiz - anhand Kennzeichen, Stammnummer oder Typenscheinnummer > Request getVehicleIdentificationByCodeSwitzerland"
---

# Request getVehicleIdentificationByCodeSwitzerland

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleIdentificationService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getVehicleIdentificationByCodeSwitzerland>
         <request>
            <locale country="ch" datCountryIndicator="ch" language="de"/>
            <restriction>ALL</restriction>
            <typeNoteNumber>1LC582</typeNoteNumber>
         </request>
      </veh:getVehicleIdentificationByCodeSwitzerland>
   </soapenv:Body>
</soapenv:Envelope>
```
