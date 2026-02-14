---
title: "Request getVehicleApproximateValue"
topic_id: "2193"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Annäherungsbewertung > Request getVehicleApproximateValue"
---

# Request getVehicleApproximateValue

```
<!-- approximation / no equipment example, first trying KBA and then maybe DATECODE -->
<soap:Envelope xmlns:soap = "http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header/>
    <soap:Body>
        <ns3:getVehicleApproximateValue xmlns:ns3 = "http://sphinx.dat.de/services/Evaluation" xmlns:ns2 = "http://www.dat.de/vxs">
            <request>
                <!-- mandatory language and data country -->
                <locale country="DE" datCountryIndicator="DE" language="de"/>
                <!-- only APPRAISAL possible -->
                <restriction>APPRAISAL</restriction>
                <datECode>019051050020005</datECode>
                <kba>0603/BJH</kba>
                <!-- define the order for identification, default: DATECODE|KBA|MODEL -->
                <identificationOrder>KBA|DATECODE</identificationOrder>
                <exFactoryPrice>18382</exFactoryPrice>
                <approximationSign>APPROXIMATION</approximationSign>
                <!-- mandatory registration date -->
                <registrationDate>2013-10-21+02:00</registrationDate>
                <!-- optional mileage; default Bezugsfahrstrecke -->
                <mileage>52766</mileage>
                <!-- optional: type of vat REGULAR or DIFFERENCE  -->
                <vatType>D</vatType>
                <coverage>COMPLETE</coverage>
            </request>
        </ns3:getVehicleApproximateValue>
    </soap:Body>
</soap:Envelope>

<!-- minimum / flat rate equipment example -->
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:eval="http://sphinx.dat.de/services/Evaluation">
   <soapenv:Header/> 
   <soapenv:Body> 
      <eval:getVehicleApproximateValue> 
         <request>
            <locale country="de" datCountryIndicator="DE" language="de"/>
            <restriction>APPRAISAL</restriction>
            <coverage>COMPLETE</coverage> 
            <identificationOrder>DATECODE</identificationOrder> 
            <approximationSign>MINIMUM</approximationSign> 
            <mileage>150000</mileage> 
            <registrationDate>2005-05-15</registrationDate> 
            <datECode>010600990240001</datECode> 
            <container>DE002</container>
            <constructionTime>4240</constructionTime>
            <manualEquipmentExFactoryPrice>9981</manualEquipmentExFactoryPrice>
            <manualEquipmentDevaluations>
                <manualEquipmentDevaluation>
                    <devaluationType>RV</devaluationType>
                    <percent>60</percent>
                </manualEquipmentDevaluation>
                <manualEquipmentDevaluation>
                    <devaluationType>T4</devaluationType>
                    <percent>40</percent>
                </manualEquipmentDevaluation>
            </manualEquipmentDevaluations>
         </request> 
      </eval:getVehicleApproximateValue> 
   </soapenv:Body>
</soapenv:Envelope>
```
