---
title: "Request getExtPartNoInfoByMfrAndExtPartNo"
topic_id: "2544"
breadcrumb: "SilverDAT Produkte > SilverDAT PartsInfo > Schnittstellenoperationen > Informationsermittlung mit Herstellerschlüssel und ETN > Request getExtPartNoInfoByMfrAndExtPartNo"
---

# Request getExtPartNoInfoByMfrAndExtPartNo

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:spar="http://sphinx.dat.de/services/SpareParts">
   <soapenv:Header/>
   <soapenv:Body>
      <spar:getExtPartNoInfoByMfrAndExtPartNo>
         <request>
            <locale country="de" datCountryIndicator="de" language="DE"/>
            <!--type: string-->
            <coverage>BASE</coverage>
            <!--Zero or more repetitions:-->
            <!--type: string-->
            <extPartNo>11617569966</extPartNo>
            <!--type: int-->
            <mfr>580</mfr>
         </request>
      </spar:getExtPartNoInfoByMfrAndExtPartNo>
   </soapenv:Body>
</soapenv:Envelope>
```
