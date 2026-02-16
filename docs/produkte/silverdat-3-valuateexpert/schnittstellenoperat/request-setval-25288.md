---
title: "Request setValueInfluencingFactors"
topic_id: "25288"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Benutzerdefinierte Handelsspanne > Benutzerdefinierte Handelsspanne anlegen > Request setValueInfluencingFactors"
---

# Request setValueInfluencingFactors

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:setValueInfluencingFactors>
         <request>
            <DossierId>2188609</DossierId>
            <Language>de_DE</Language>
            <NominalDaysOnLot>150</NominalDaysOnLot>
            <ValueInfluencingFactorList>
               <ValueInfluencingFactorItem>
                  <ValueInfluencingFactorId>18927860</ValueInfluencingFactorId>
                  <ValueNet>100</ValueNet>
               </ValueInfluencingFactorItem>
               <ValueInfluencingFactorItem>
                  <ValueInfluencingFactorId>18927857</ValueInfluencingFactorId>
                  <ValueNet>100</ValueNet>
               </ValueInfluencingFactorItem>
               <ValueInfluencingFactorItem>
                  <ValueInfluencingFactorId>18927862</ValueInfluencingFactorId>
                  <ValueNet>100</ValueNet>
               </ValueInfluencingFactorItem>
               <ValueInfluencingFactorItem>
                  <ValueInfluencingFactorId>18927858</ValueInfluencingFactorId>
                  <ValueNet>100</ValueNet>
               </ValueInfluencingFactorItem>
               <ValueInfluencingFactorItem>
                  <ValueInfluencingFactorId>18927861</ValueInfluencingFactorId>
                  <ValueNet>100</ValueNet>
               </ValueInfluencingFactorItem>
               <ValueInfluencingFactorItem>
                  <ValueInfluencingFactorId>18927859</ValueInfluencingFactorId>
                  <ValueNet>100</ValueNet>
               </ValueInfluencingFactorItem>
            </ValueInfluencingFactorList>
         </request>
      </dos:setValueInfluencingFactors>
   </soapenv:Body>
</soapenv:Envelope>
```
