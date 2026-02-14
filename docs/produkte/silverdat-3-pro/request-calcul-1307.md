---
title: "Request calculate"
topic_id: "1307"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > Kalkulieren eines Fahrzeugs ohne Speicherung > Request calculate"
---

# Request calculate

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://www.dat.eu/myClaim/soap/v2/VehicleRepairService">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:calculate>
         <!--Optional:-->
         <request>
            <!--Optional:-->
            <calculationWages>
               <!--Zero or more repetitions:-->
               <calculationWage level="1" type="VRO_REPAIRWAGE_ELECTRIC">132.10</calculationWage>
               <calculationWage level="1" type="VRO_REPAIRWAGE_MECHANIC">145.50</calculationWage>
               <calculationWage level="1" type="VRO_REPAIRWAGE_BODY">136.60</calculationWage>
               <calculationWage level="1" type="lacquer">156.51</calculationWage>
               <calculationWage level="1" type="lacquerType">12</calculationWage>
               <calculationWage level="1" type="dent">25</calculationWage>
               <calculationWage level="2" type="VRO_REPAIRWAGE_ELECTRIC"/>
               <calculationWage level="2" type="VRO_REPAIRWAGE_MECHANIC"/>
               <calculationWage level="2" type="VRO_REPAIRWAGE_BODY"/>
               <calculationWage level="3" type="VRO_REPAIRWAGE_ELECTRIC"/>
               <calculationWage level="3" type="VRO_REPAIRWAGE_MECHANIC"/>
               <calculationWage level="3" type="VRO_REPAIRWAGE_BODY"/>

            </calculationWages>
            <!--Optional:-->
            <contructionTime>4567</contructionTime>
            <!--Optional:-->
            <datECode>011940020020010</datECode>
            <!--Optional:-->
            <!--Zero or more repetitions:-->
            <equipment>98206</equipment>
            <equipment>98207</equipment>
            <equipment>57202</equipment>
            <equipment>35301</equipment>
            <!--datProcessInfos-->
            <!--Repair-->
            <datProcessInfo>
               <datProcessId>44210</datProcessId>
            </datProcessInfo>
            <datProcessInfo>
               <datProcessId>43712</datProcessId>
            </datProcessInfo>
            <!--Maintenance-->
            <datProcessInfo method="MAINTENANCE" type="INTERVAL">
               <datProcessId>94030</datProcessId>
            </datProcessInfo>
            <!--Zahnriemen der Motorsteuerung austauschen-->
            <datProcessInfo method="MAINTENANCE" type="LABOUR">
               <datProcessId>81715</datProcessId>
            </datProcessInfo>
            <!--REP.-SATZ ZAHNRIEMEN-->
            <datProcessInfo method="MAINTENANCE" type="MATERIAL">
               <datProcessId>81715</datProcessId>
            </datProcessInfo>
            <datProcessInfo>
               <datProcessId>81691</datProcessId>
            </datProcessInfo>
            <datProcessInfo>
               <datProcessId>81200</datProcessId>
            </datProcessInfo>
            <!--Optional:-->
            <includeAttachments>false</includeAttachments>
            <!--Optional:-->
            <includeComments>false</includeComments>
            <!--Optional:-->
            <includeProtocol>true</includeProtocol>
            <!--Optional:-->
            <isAlternativeCalculationUsed>false</isAlternativeCalculationUsed>
            <!--Optional:-->
            <isCountryCurrency>false</isCountryCurrency>
            <!--Optional:-->
            <isDMSCalculation>false</isDMSCalculation>
            <!--Optional:-->
            <isPhantomCalculation>false</isPhantomCalculation>
            <isSerialCalculation>false</isSerialCalculation>
            <!--Optional:-->
            <locale country="DE" datCountryIndicator="DE" language="de"/>
            <!--Optional:-->
            <paintingColorDescription>
               <!--Optional:-->
               <datCode>1</datCode>
               <!--Optional:-->
               <expression>0</expression>
               <!--Optional:-->
               <name>Weiß</name>
               <!--Optional:-->
               <priceCategory>200</priceCategory>
               <!--Optional:-->
               <type>1</type>
            </paintingColorDescription>
            <!--Optional:-->
            <paintingMethod>EURO_LACQUER</paintingMethod>
            <!--Optional:-->
            <useTimeUnitsOfManufacturer>false</useTimeUnitsOfManufacturer>
         </request>
      </veh:calculate>
   </soapenv:Body>
</soapenv:Envelope>
```
