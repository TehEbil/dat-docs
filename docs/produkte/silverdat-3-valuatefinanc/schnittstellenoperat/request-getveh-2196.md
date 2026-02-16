---
title: "Request getVehicleEvaluation"
topic_id: "2196"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Standardbewertung und Standard Restwertprognose > Standardbewertung > Request getVehicleEvaluation"
---

# Request getVehicleEvaluation

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:eval="http://sphinx.dat.de/services/Evaluation">
   <soapenv:Header/>
   <soapenv:Body>
      <eval:getVehicleEvaluation>
         <!--Optional:-->
         <request>
           <locale country="DE" datCountryIndicator="de" language="de"/>
            <!--Optional:-->
            <!--type: int-->
            <constructionTimeFrom>3</constructionTimeFrom>
            <!--Optional:-->
            <!--type: int-->
            <constructionTimeTo>3</constructionTimeTo>
            <!-- only APPRAISAL possible -->
            <restriction>APPRAISAL</restriction>
            <!--type: string-->
            <datECode>019100570060001</datECode>
            <!--Optional:-->
            <!--type: string-->
            <container>DE002</container>
            <!--type: int-->
            <constructionTime>4970</constructionTime>
            <!--Optional:-->
            <!--type: string-->
            <coverage>COMPLETE</coverage>
            <!--Optional:-->
            <equipment>
            <!--Zero or more repetitions:-->
               <equipmentPosition>
                <!--type: int-->
                  <datEquipmentId>26704</datEquipmentId>
                  <!--Optional:-->
                  <!--type: string-->
                  <devaluationType>T1</devaluationType>
               </equipmentPosition>
            </equipment>
            <!--type: string-->
            <save>true</save>
            <!--Optional:-->
            <condition>
               <!--Optional:-->
               <!--type: int-->
               <accidentDamage>accident free</accidentDamage>
               <!--Optional:-->
               <!--type: decimal-->
               <correctionFactorPercent>90</correctionFactorPercent>
               <!--Optional:-->
               <!--type: decimal-->
               <decreaseInValue>500.50</decreaseInValue>
               <!--Optional:-->
               <!--type: decimal-->
               <increaseInValue>300</increaseInValue>
               <!--Optional:-->
               <!--type: int-->
               <numberOfOwners>3</numberOfOwners>
               <!--Optional:-->
               <!--type: decimal-->
               <ownerCorrectionPercent>5</ownerCorrectionPercent>
               <!--Optional:-->
               <!--type: decimal-->
               <repairCosts>2000</repairCosts>
               <!--Optional:-->
               <!--type: decimal-->
               <tiresMountedValue>-100</tiresMountedValue>
               <!--Optional:-->
               <!--type: decimal-->
               <tiresUnmountedValue>300</tiresUnmountedValue>
            </condition>
            <!--type: long-->
            <mileage>12000</mileage>
            <!--type: anySimpleType-->
            <registrationDate>2010-10-20</registrationDate>
            <licenseNumber>ES DAT 123</licenseNumber>
            <!--Optional:-->
            <!--type: string-->
            <vatType>R</vatType>
         </request>
      </eval:getVehicleEvaluation>
   </soapenv:Body>
</soapenv:Envelope>
```
