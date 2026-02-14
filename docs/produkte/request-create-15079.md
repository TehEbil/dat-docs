---
title: "Request createDossierN ForeCast in FinanceLine"
topic_id: "15079"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Erstellen eines neuen Vorgangs > Request createDossierN ForeCast in FinanceLine"
---

# Request createDossierN ForeCast in FinanceLine

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N" xmlns:vxs="http://www.dat.de/vxs">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:createDossierN>
         <vxs:Dossier>
              <vxs:Name>createDossierN Forecast example</vxs:Name>
            <vxs:Language>de_DE</vxs:Language>
            <vxs:Vehicle>
               <vxs:DatECode>015700990870025</vxs:DatECode>
               <vxs:Container>DE00R</vxs:Container>
               <vxs:ConstructionTime>6540</vxs:ConstructionTime>
               <vxs:InitialRegistration>2024-06-01</vxs:InitialRegistration>
               <vxs:MileageEstimated>500</vxs:MileageEstimated>
               <vxs:Country>DE</vxs:Country>
               <vxs:Equipment>
                  <vxs:SpecialEquipment>
                     <vxs:EquipmentPosition>
                        <vxs:DatEquipmentId>18026</vxs:DatEquipmentId>
                        <vxs:DevaluationType>T1</vxs:DevaluationType>
                     </vxs:EquipmentPosition>
                     <vxs:EquipmentPosition>
                        <vxs:DatEquipmentId>68796</vxs:DatEquipmentId>
                        <vxs:DevaluationType>T2</vxs:DevaluationType>
                     </vxs:EquipmentPosition>
                  </vxs:SpecialEquipment>
               </vxs:Equipment>
               </vxs:Vehicle>
               <vxs:Valuation>
                  <vxs:ValuationType>VALUATION</vxs:ValuationType>
                  <vxs:Forecasts>
                     <vxs:Forecast>
                        <vxs:PriceType>purchase</vxs:PriceType>
                        <vxs:IncludeVat>true</vxs:IncludeVat>
                        <vxs:CurveType>default</vxs:CurveType>
                        <vxs:DecreaseType>residual value</vxs:DecreaseType>
                        <vxs:StartType>initial registration</vxs:StartType>
                        <vxs:ValueType>monetary</vxs:ValueType>
                        <vxs:MileageType>year</vxs:MileageType>
                        <vxs:ForecastItems>
                           <vxs:ForecastItem>
                              <vxs:Months>38</vxs:Months>
                              <vxs:MileagePerYear>500</vxs:MileagePerYear>
                           </vxs:ForecastItem>
                        </vxs:ForecastItems>
                     </vxs:Forecast>
                  </vxs:Forecasts>
               </vxs:Valuation>
         </vxs:Dossier>
         <Save>false</Save>
      </dos:createDossierN>
   </soapenv:Body>
</soapenv:Envelope>
```
