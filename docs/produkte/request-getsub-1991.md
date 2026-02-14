---
title: "Request getSubModelsByTextSearch"
topic_id: "1991"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getSubModelsByTextSearch > Request getSubModelsByTextSearch"
---

# Request getSubModelsByTextSearch

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:veh="http://sphinx.dat.de/services/VehicleSelectionService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getSubModelsByTextSearch>
         <request>
            <locale country="de" datCountryIndicator="de" language="de"/>
            <restriction>ALL</restriction>
            <!--Optional:-->
            <constructionTimeFrom>4000</constructionTimeFrom>
            <!--Optional:-->
            <constructionTimeTo>5000</constructionTimeTo>
            <searchText>Polo</searchText>
         </request>
      </veh:getSubModelsByTextSearch>
   </soapenv:Body>
</soapenv:Envelope>
```
