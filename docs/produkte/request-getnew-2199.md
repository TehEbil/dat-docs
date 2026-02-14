---
title: "Request getNewVehicleForecast"
topic_id: "2199"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Standardbewertung und Standard Restwertprognose > Standard Restwertprognose Neufahrzeuge > Request getNewVehicleForecast"
---

# Request getNewVehicleForecast

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:eval="http://sphinx.dat.de/services/Evaluation">
   <soapenv:Header/>
   <soapenv:Body>
      <eval:getNewVehicleForecast>
         <request>
            <locale country="de" datCountryIndicator="de" language="de"/>
            <!--Optional:-->
            <!--type: int-->
            <constructionTimeFrom>5000</constructionTimeFrom>
            <!--Optional:-->
            <!--type: int-->
            <constructionTimeTo>6000</constructionTimeTo>
            <!-- only APPRAISAL possible -->
            <restriction>APPRAISAL</restriction>
            <!--type: string-->
            <datECode>019051120190002</datECode>
            <!--Optional:-->
            <!--type: string-->
            <container>DE002</container>
            <!--type: int-->
            <constructionTime>5410</constructionTime>
            <!--Optional:-->
            <!--type: string-->
            <coverage>BASE</coverage>
            <!--Optional:-->
            <equipment>
               <!--Zero or more repetitions:-->
               <equipmentPosition>
                  <!--type: int-->
                  <datEquipmentId>1671</datEquipmentId>
                  <!--Optional:-->
                  <!--type: string-->
                  <devaluationType>T1</devaluationType>
               </equipmentPosition>
               <equipmentPosition>
                  <!--type: int-->
                  <datEquipmentId>41150</datEquipmentId>
                  <devaluationType>RV</devaluationType>
               </equipmentPosition>
               <equipmentPosition>
                  <!--type: int-->
                  <datEquipmentId>16708</datEquipmentId>
                  <devaluationType>T4</devaluationType>
               </equipmentPosition>
               <equipmentPosition>
                  <!--type: int-->
                  <datEquipmentId>25800</datEquipmentId>
                  <devaluationType>T2</devaluationType>
               </equipmentPosition>
            </equipment>
            <!--type: string-->
            <save>true</save>
            <!--type: string-->
            <curveType>MAXIMUM</curveType>
            <!--type: string-->
            <decreaseType>Residual value</decreaseType>
            <forecastItems>
               <!--Zero or more repetitions:-->
               <forecastItem>
                  <!--type: int-->
                  <ageInMonth>6</ageInMonth>
                  <!--Optional:-->
                  <!--type: long-->
                  <mileagePerYear>10000</mileagePerYear>
               </forecastItem>
            </forecastItems>
            <!--type: string-->
            <includeVat>true</includeVat>
            <!--Optional:-->
            <!--type: string-->
            <mileageType>YEAR</mileageType>
            <!--type: string-->
            <priceType>SALESPRICE</priceType>
            <!--type: string-->
            <valueType>MONETARY</valueType>
         </request>
      </eval:getNewVehicleForecast>
   </soapenv:Body>
</soapenv:Envelope>
```
