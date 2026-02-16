---
title: "Request getSparePartsDetails"
topic_id: "17316"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > Ermittlung von Fahrzeuginformationen, DVN, Verbauungsbedingungen und/oder Preishistorie > Request getSparePartsDetails"
---

# Request getSparePartsDetails

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://www.dat.eu/myClaim/soap/v2/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:getSparePartsDetails>
         <!--Optional:-->
         <request>
            <locale country="DE" datCountryIndicator="DE" language="de"/>
            <restriction>
               <vehicleType>1</vehicleType>
               <manufacturer>130</manufacturer>
               <baseModel>066</baseModel>
               <!--1 or more repetitions:-->
               <sparePartNo>51317070292</sparePartNo>
            </restriction>
            <!--Optional:-->
            <settings>
               <!--Optional:-->
               <sortingCriterions>
                  <constructionTime>
                     <!--Optional:-->
                     <order>desc</order>
                     <!--Optional:-->
                     <priority>2</priority>
                     <!--Optional:-->
                  </constructionTime>
                  <!--Optional:-->
                  <subModel>
                     <!--Optional:-->
                     <order>asc</order>
                     <!--Optional:-->
                     <priority>1</priority>
                     <!--Optional:-->
                  </subModel>
               </sortingCriterions>
               <!--Optional:-->
               <withPriceHistory>true</withPriceHistory>
               <!--Optional:-->
               <withVehicleData>true</withVehicleData>
            </settings>
         </request>
      </veh:getSparePartsDetails>
   </soapenv:Body>
</soapenv:Envelope>
```
