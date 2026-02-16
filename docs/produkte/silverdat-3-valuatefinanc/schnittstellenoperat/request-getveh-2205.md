---
title: "Request getVehicleTargetDateEvaluationHistory"
topic_id: "2205"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Stichtagsbezogene Bewertung durchführen (Historische Bewertung) > Request getVehicleTargetDateEvaluationHistory"
---

# Request getVehicleTargetDateEvaluationHistory

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:eval="http://sphinx.dat.de/services/Evaluation">
   <soapenv:Header/>
   <soapenv:Body>
      <eval:getVehicleTargetDateEvaluationHistory>
         <request>
            <locale country="de" datCountryIndicator="de" language="de"/>
            <restriction>APPRAISAL</restriction>
            <datECode>019051080040002</datECode>
            <container>DE002</container>
            <constructionTime>5419</constructionTime>
            <coverage>COMPLETE</coverage>
            <save>false</save>
            <condition>
               <accidentDamage>accident free</accidentDamage>
               <correctionFactorPercent>90</correctionFactorPercent>
               <decreaseInValue>500.50</decreaseInValue>
               <increaseInValue>300</increaseInValue>
               <numberOfOwners>3</numberOfOwners>
               <ownerCorrectionPercent>5</ownerCorrectionPercent>
               <repairCosts>2000</repairCosts>
               <tiresMountedValue>-100</tiresMountedValue>
            </condition>
            <mileage>50000</mileage>
            <registrationDate>2018-11-01</registrationDate>
            <licenseNumber>ES DAT 123</licenseNumber>
            <vatType>difference</vatType>
            <evaluationDate>2018-11-01</evaluationDate>
         </request>
      </eval:getVehicleTargetDateEvaluationHistory>
   </soapenv:Body>
</soapenv:Envelope>
```
