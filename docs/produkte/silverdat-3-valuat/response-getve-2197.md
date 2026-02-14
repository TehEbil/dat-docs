---
title: "Response getVehicleEvaluation"
topic_id: "2197"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Standardbewertung und Standard Restwertprognose > Standardbewertung > Response getVehicleEvaluation"
---

# Response getVehicleEvaluation

Eine Beschreibung aller Response-Parameter finden Sie unter [Datenaustauschformat VXS](../../vxs/aktenzeichenvo-1369.md).

```
<!--Sample response if request was successful-->
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns2:getVehicleEvaluationResponse xmlns:ns2="http://sphinx.dat.de/services/Evaluation" xmlns:ns3="http://www.dat.de/vxs">
         <VXS source="SD3" type="singleEvaluation">
            <ns3:Dossier>
               <ns3:Country>DE</ns3:Country>
               <ns3:Language>de_DE</ns3:Language>
               <ns3:DatCustomerId>XXXX</ns3:DatCustomerId>
               <ns3:Vehicle>
                  <ns3:DatECode>019100570060001</ns3:DatECode>
                  <ns3:Container>DE002</ns3:Container>
                  <ns3:ConstructionTime>4970</ns3:ConstructionTime>
                  <ns3:InitialRegistration>2010-10-20+02:00</ns3:InitialRegistration>
                  <ns3:MileageEstimated>12000</ns3:MileageEstimated>
                  <ns3:ManufacturerName>Volvo</ns3:ManufacturerName>
                  <ns3:VehicleTypeName>Pkw, SUV, Kleintransporter</ns3:VehicleTypeName>
                  <ns3:BaseModelName>V 60 Kombi (08.2010->)</ns3:BaseModelName>
                  <ns3:SubModelName>Ocean Race</ns3:SubModelName>
                  <ns3:ContainerName>DE - Kb5 1.6 D Drive Euro-Norm 5, Ocean Race, 2011 - 2012</ns3:ContainerName>
                  <ns3:IdentificationSource>DATECODE</ns3:IdentificationSource>
                  <ns3:Country>DE</ns3:Country>
                  <ns1:RegistrationData>
                     <ns1:LicenseNumber>ES DAT 123</ns1:LicenseNumber>
                  </ns1:RegistrationData>
                  <ns3:TechInfo/>
                  <ns3:Equipment>
                     <ns3:EquipmentValue origin="dat">0</ns3:EquipmentValue>
                     <ns3:EquipmentValueGross origin="dat">0.00</ns3:EquipmentValueGross>
                     <ns3:OriginalEquipmentValue origin="dat">0</ns3:OriginalEquipmentValue>
                     <ns3:OriginalEquipmentValueGross origin="dat">0.00</ns3:OriginalEquipmentValueGross>
                     <ns3:EquipmentValueType>calculated value</ns3:EquipmentValueType>
                     <ns3:SeriesEquipment>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>627</ns3:DatEquipmentId>
                           <ns3:Description>Modellvariante Drive</ns3:Description>
                        </ns3:EquipmentPosition>
                        ...
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>83715</ns3:DatEquipmentId>
                           <ns3:Description>Motor 1,6 Ltr. - 84 kW Diesel KAT</ns3:Description>
                        </ns3:EquipmentPosition>
                     </ns3:SeriesEquipment>
                  </ns3:Equipment>
                  <ns3:DATECodeEquipment>
                     <ns3:EquipmentPosition>
                        <ns3:DatEquipmentId>83715</ns3:DatEquipmentId>
                        <ns3:Description>Motor 1,6 Ltr. - 84 kW Diesel KAT</ns3:Description>
                     </ns3:EquipmentPosition>
                     ...
                     <ns3:EquipmentPosition>
                        <ns3:DatEquipmentId>75205</ns3:DatEquipmentId>
                        <ns3:Description>Getriebe 6-Gang</ns3:Description>
                     </ns3:EquipmentPosition>
                  </ns3:DATECodeEquipment>
               </ns3:Vehicle>
               <ns3:VAT>
                  <ns3:VatType>regular</ns3:VatType>
                  <ns3:VatAtConstructionTime>19</ns3:VatAtConstructionTime>
                  <ns3:VatAtValuationTime origin="dat">19</ns3:VatAtValuationTime>
               </ns3:VAT>
               <ns3:Valuation>
                  <ns3:OriginalPrice origin="dat">27773</ns3:OriginalPrice>
                  <ns3:OriginalPriceGross origin="dat">33050</ns3:OriginalPriceGross>
                  <ns3:BasePrice origin="dat">16559.00</ns3:BasePrice>
                  <ns3:ReferenceMileage>37000</ns3:ReferenceMileage>
                  <ns3:MileageCorr origin="dat">1269.08</ns3:MileageCorr>
                  <ns3:InitialRegistrationCorr origin="dat">-853.33</ns3:InitialRegistrationCorr>
                  <ns3:BasePrice2 origin="dat">16974.75</ns3:BasePrice2>
                  <ns3:EquipmentSign>calculated value</ns3:EquipmentSign>
                  <ns3:EquipmentOriginalPrice origin="dat">0</ns3:EquipmentOriginalPrice>
                  <ns3:EquipmentPrice origin="dat">0</ns3:EquipmentPrice>
                  <ns3:ValuationCorrection origin="dat">-4121.22</ns3:ValuationCorrection>
                  <ns3:BasePrice3 origin="dat">16974.75</ns3:BasePrice3>
                  <ns3:ConditionCorrectionPerc origin="user">75.72</ns3:ConditionCorrectionPerc>
                  <ns3:SalesPrice>12853.53</ns3:SalesPrice>
                  <ns3:SalesPriceGross>15295.70</ns3:SalesPriceGross>
                  <ns3:Margin origin="dat">1849.86</ns3:Margin>
                  <ns3:MarginGross origin="dat">2201.33</ns3:MarginGross>
                  <ns3:PurchasePrice>11003.67</ns3:PurchasePrice>
                  <ns3:PurchasePriceGross>13094.37</ns3:PurchasePriceGross>
                  <ns3:LastValuationDataYear>2013</ns3:LastValuationDataYear>
                  <ns3:LastValuationDataMonth>1</ns3:LastValuationDataMonth>
                  <ns3:LastValuationDate>2013-01-18T15:28:28.264+01:00</ns3:LastValuationDate>
                  <ns1:Currency>EUR</ns1:Currency>
                  <ns3:ValuationType>valuation</ns3:ValuationType>
                  <ns3:Condition>
                     <ns3:OwnerCorrectionPerc>5</ns3:OwnerCorrectionPerc>
                     <ns3:OwnerCorrectionAmount>-873.74</ns3:OwnerCorrectionAmount>
                     <ns3:OwnerCorrectionAmountGross>-1039.75</ns3:OwnerCorrectionAmountGross>
                     <ns3:ConditionCorrectionFactorPerc>90</ns3:ConditionCorrectionFactorPerc>
                     <ns3:ConditionCorrectionAmount>-1747.48</ns3:ConditionCorrectionAmount>
                     <ns3:ConditionCorrectionAmountGross>-2079.50</ns3:ConditionCorrectionAmountGross>
                     <ns3:NumberOfOwners>3</ns3:NumberOfOwners>
                     <ns3:AccidentDamage>accident free</ns3:AccidentDamage>
                     <ns3:IncreaseInValue>300</ns3:IncreaseInValue>
                     <ns3:IncreaseInValueGross>357.00</ns3:IncreaseInValueGross>
                     <ns3:TiresMountedValue>-100</ns3:TiresMountedValue>
                     <ns3:TiresMountedValueGross>-119.00</ns3:TiresMountedValueGross>
                     <ns3:TiresUnmountedValue>300</ns3:TiresUnmountedValue>
                     <ns3:TiresUnmountedValueGross>357.00</ns3:TiresUnmountedValueGross>
                     <ns3:RepairCosts>2000</ns3:RepairCosts>
                     <ns3:RepairCostsGross>2380.00</ns3:RepairCostsGross>
                     <ns3:ConditionSubTotal1>17474.75</ns3:ConditionSubTotal1>
                     <ns3:ConditionSubTotal1Gross>20794.95</ns3:ConditionSubTotal1Gross>
                     <ns3:ConditionSubTotal2>14853.53</ns3:ConditionSubTotal2>
                     <ns3:ConditionSubTotal2Gross>17675.70</ns3:ConditionSubTotal2Gross>
                  </ns3:Condition>
                  <ns3:Parameters/>
               </ns3:Valuation>
            </ns3:Dossier>
         </VXS>
      </ns2:getVehicleEvaluationResponse>
   </S:Body>
</S:Envelope>
```
