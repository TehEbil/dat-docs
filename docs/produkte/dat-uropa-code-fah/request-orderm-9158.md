---
title: "Request orderMarkedVin"
topic_id: "9158"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Bestellung gesperrter Fahrzeuge > Request orderMarkedVin"
---

# Request orderMarkedVin

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleIdentificationService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:orderMarkedVin>
         <request>
            <locale country="de" datCountryIndicator="de" language="de"/>
            <!--Optional:-->
            <claimNumber>12345678</claimNumber>
            <contact>Max Mustermann</contact>
            <email>Max.Mustermann@dat.de</email>
            <telephone>0711 12345678</telephone>
            <vin>WVWBLOCKEDTEST001</vin>
         </request>
      </veh:orderMarkedVin>
   </soapenv:Body>
</soapenv:Envelope>
```
