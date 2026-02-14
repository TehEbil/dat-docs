---
title: "Request getExtPartNoInfoByFullVehicleAndIntPartNo"
topic_id: "2540"
breadcrumb: "SilverDAT Produkte > SilverDAT PartsInfo > Schnittstellenoperationen > Rückgabe von ETN über DAT europa-Code Ausstattung und DVN > Request getExtPartNoInfoByFullVehicleAndIntPartNo"
---

# Request getExtPartNoInfoByFullVehicleAndIntPartNo

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:spar="http://sphinx.dat.de/services/SpareParts">
   <soapenv:Header/>
   <soapenv:Body>
      <spar:getExtPartNoInfoByFullVehicleAndIntPartNo>
         <!--Optional:-->
         <request>
            <locale country="DE" datCountryIndicator="DE" language="de"/>
            <coverage>COMPLETE</coverage>
            <!--Optional:-->
            <datECode>011300660340006</datECode>
            <!--Zero or more repetitions:-->
            <intPartNo>44210</intPartNo>
            <intPartNo>43711</intPartNo>
            <contructionTime>4518</contructionTime>
            <!--Zero or more repetitions:-->
            <equipment>4905</equipment>
            <equipment>2701</equipment>
            <equipment>25805</equipment>
         </request>
      </spar:getExtPartNoInfoByFullVehicleAndIntPartNo>
   </soapenv:Body>
</soapenv:Envelope>
```
