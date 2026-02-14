---
title: "Request getModelInfoByMfrAndExtPartNo"
topic_id: "2549"
breadcrumb: "SilverDAT Produkte > SilverDAT PartsInfo > Schnittstellenoperationen > Rückgabe von Modellinfo über HST und ETN > Request getModelInfoByMfrAndExtPartNo"
---

# Request getModelInfoByMfrAndExtPartNo

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:spar="http://sphinx.dat.de/services/SpareParts">
   <soapenv:Header/>
   <soapenv:Body>
      <spar:getModelInfoByMfrAndExtPartNo>
         <!--Optional:-->
         <request>
            <locale country="de" datCountryIndicator="de" language="de"/>
            <!--type: string-->
            <coverage>BASE</coverage>
            <!--Zero or more repetitions:-->
            <!--type: string-->
            <extPartNo>1K6941005P</extPartNo>
            <!--type: int-->
            <manufacturer>905</manufacturer>
         </request>
      </spar:getModelInfoByMfrAndExtPartNo>
   </soapenv:Body>
</soapenv:Envelope>
```
