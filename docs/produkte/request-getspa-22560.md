---
title: "Request getSparePartsDetailsForDPN"
topic_id: "22560"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > PartsService > Ermittlung der Fahrzeuginformationen, Ersatzteilnummern, Verbauungsbedingungen und/oder Preishistorie > Request getSparePartsDetailsForDPN"
---

# Request getSparePartsDetailsForDPN

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://www.dat.eu/myClaim/soap/v2/PartsService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getSparePartsDetailsForDPN>
         <!--Optional:-->
         <request>
            <locale country="DE" datCountryIndicator="DE" language="de"/>
            <restriction>
               <datProcessNo>44910</datProcessNo>
               <manufacturer>130</manufacturer>
               <baseModel>066</baseModel>
               <vehicleType>1</vehicleType>
            </restriction>
            <settings>
               <!--Optional:-->
               <pageNumber>1</pageNumber>
               <!--Optional:-->
               <pageSize>60</pageSize>
               <!--Optional:-->
               <sortingCriterions>
                  <!--Optional:-->
                  <baseModel>
                     <!--Optional:-->
                     <order>asc</order>
                     <!--Optional:-->
                     <priority>2</priority>
                     <!--Optional:-->
                  </baseModel>
                  <!--Optional:-->
                  <constructionTime>
                     <!--Optional:-->
                     <order>asc</order>
                     <!--Optional:-->
                     <priority>1</priority>
                     <!--Optional:-->
                  </constructionTime>
               </sortingCriterions>
               <!--Optional:-->
               <withPriceHistory>true</withPriceHistory>
               <!--Optional:-->
               <withVehicleData>true</withVehicleData>
            </settings>
            <!--Optional:-->
         </request>
      </veh:getSparePartsDetailsForDPN>
   </soapenv:Body>
</soapenv:Envelope>
```
