---
title: "Request searchDossierListN"
topic_id: "15054"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Suchen von Vorgängen > Request searchDossierListN"
---

# Request searchDossierListN

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://sphinx.dat.de/services/DossierN">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:searchDossierListN>
         <SearchCriterionList>
            <SearchCriterion>
               <Key>VehicleType</Key>
               <Value>1</Value>
            </SearchCriterion>
            <SearchCriterion>
               <Key>Manufacturer</Key>
               <Value>905</Value>
            </SearchCriterion>
            <SearchCriterion>
               <Key>MainModel</Key>
               <Value>3</Value>
            </SearchCriterion>
            <SearchCriterion>
               <Key>SubModel</Key>
               <Value>2</Value>
            </SearchCriterion>
            <SearchCriterion>
               <Key>SubModelVariant</Key>
               <Value>43</Value>
            </SearchCriterion>
            <SearchCriterion>
               <Key>Container</Key>
               <Value>DE001</Value>
            </SearchCriterion>
            <SearchCriterion>
               <Key>ConstructionTime</Key>
               <LowerLimit>4000</LowerLimit>
               <UpperLimit>5500</UpperLimit>
            </SearchCriterion>
            <SearchCriterion>
               <Key>InitialRegistration</Key>
               <LowerLimit>2001-01-01</LowerLimit>
               <UpperLimit>2013-09-10</UpperLimit>
            </SearchCriterion>
            <SearchCriterion>
               <Key>MileageEstimated</Key>
               <LowerLimit>80000</LowerLimit>
               <UpperLimit>96000</UpperLimit>
            </SearchCriterion>
            <SearchCriterion>
               <Key>LicenseNumber</Key>
               <Value>S DAT*</Value>
               <useWildcard>true</useWildcard>
            </SearchCriterion>
         </SearchCriterionList>
         <Limit>50</Limit>
         <Coverage>COMPLETE</Coverage>
      </dos:searchDossierListN>
   </soapenv:Body>
</soapenv:Envelope>
```
