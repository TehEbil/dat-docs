---
title: "Request getExtPartNoInfoByModelAndExtPartNo"
topic_id: "2522"
breadcrumb: "SilverDAT Produkte > SilverDAT PartsInfo > Schnittstellenoperationen > Informationsermittlung mit Untertyp und ETN > Request getExtPartNoInfoByModelAndExtPartNo"
---

# Request getExtPartNoInfoByModelAndExtPartNo

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:spar="http://sphinx.dat.de/services/SpareParts">
   <soapenv:Header/>
   <soapenv:Body>
      <spar:getExtPartNoInfoByModelAndExtPartNo>
         <!--Optional:-->
         <request>
            <locale country="DE" datCountryIndicator="DE" language="de"/>
            <coverage>COMPLETE</coverage>
            <baseModel>66</baseModel>
            <!--1 or more repetitions:-->
            <extPartNo>41357111429</extPartNo>
            <manufacturer>130</manufacturer>
            <subModel>34</subModel>
            <vehicleType>1</vehicleType>
         </request>
      </spar:getExtPartNoInfoByModelAndExtPartNo>
   </soapenv:Body>
</soapenv:Envelope>
```
