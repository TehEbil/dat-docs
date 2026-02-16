---
title: "Request getUsedVehicleForecast"
topic_id: "2202"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Standardbewertung und Standard Restwertprognose > Standard Restwertprognose Gebrauchtfahrzeuge > Request getUsedVehicleForecast"
---

# Request getUsedVehicleForecast

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:eval="http://sphinx.dat.de/services/Evaluation">
   <soapenv:Header/>
   <soapenv:Body>
      <eval:getUsedVehicleForecast>
         <request>
            <locale country="de" datCountryIndicator="de" language="de"/>
            <constructionTimeFrom>5000</constructionTimeFrom>
            <constructionTimeTo>5800</constructionTimeTo>
            <!-- only APPRAISAL possible -->
            <restriction>APPRAISAL</restriction>
            <datECode>019051080040002</datECode>
            <container>DE002</container>
            <constructionTime>5419</constructionTime>
            <!--simple => response with less data volume-->
            <coverage>simple</coverage>
            <!--store this valuation as dossier -->
            <save>true</save>
            <curveType>MAXIMUM</curveType>
            <decreaseType>Table1</decreaseType>
            <forecastItems>
               <forecastItem>
                  <ageInMonth>18</ageInMonth>
                  <mileagePerYear>5000</mileagePerYear>
               </forecastItem>
               <forecastItem>
                  <ageInMonth>24</ageInMonth>
                  <mileagePerYear>10000</mileagePerYear>
               </forecastItem>
               <forecastItem>
                  <ageInMonth>30</ageInMonth>
                  <mileagePerYear>15000</mileagePerYear>
               </forecastItem>
            </forecastItems>
            <includeVat>false</includeVat>
            <mileageType>YEAR</mileageType>
            <priceType>SalesPrice</priceType>
            <valueType>Mileage</valueType>
            <mileage>5500</mileage>
            <registrationDate>2015-03-01</registrationDate>
            <licenseNumber>ES DAT 123</licenseNumber>
         </request>
      </eval:getUsedVehicleForecast>
   </soapenv:Body>
</soapenv:Envelope>
```
