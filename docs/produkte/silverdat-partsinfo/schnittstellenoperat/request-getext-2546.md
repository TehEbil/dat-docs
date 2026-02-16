---
title: "Request getExtPartNoInfoByVinAndIntPartNo"
topic_id: "2546"
breadcrumb: "SilverDAT Produkte > SilverDAT PartsInfo > Schnittstellenoperationen > Rückgabe ETN über VIN und DVN > Request getExtPartNoInfoByVinAndIntPartNo"
---

# Request getExtPartNoInfoByVinAndIntPartNo

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:spar="http://sphinx.dat.de/services/SpareParts">
   <soapenv:Header/>
   <soapenv:Body>
      <spar:getExtPartNoInfoByVinAndIntPartNo>
         <!--Optional:-->
         <request>
            <locale country="de" datCountryIndicator="de" language="DE"/>
            <!--type: string-->
            <coverage>COMPLETE</coverage>
            <!--Zero or more repetitions:-->
            <!--type: int-->
            <intPartNo>83110</intPartNo>
            <!--Optional:-->
            <!--type: string-->
            <vin>WMWMG31090TU52263</vin>
         </request>
      </spar:getExtPartNoInfoByVinAndIntPartNo>
   </soapenv:Body>
</soapenv:Envelope>
```
