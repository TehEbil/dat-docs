---
title: "Response getUsedVehicleForecast"
topic_id: "2203"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Standardbewertung und Standard Restwertprognose > Standard Restwertprognose Gebrauchtfahrzeuge > Response getUsedVehicleForecast"
---

# Response getUsedVehicleForecast

Eine Beschreibung aller Response-Parameter finden Sie unter [Datenaustauschformat VXS](#showid/1369 "Aktenzeichen/Vorgänge (Dossiers)").

```
<!-- Sample response, if request was successful -->
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns2:getUsedVehicleForecastResponse xmlns:ns2="http://sphinx.dat.de/services/Evaluation" xmlns:ns3="http://www.dat.de/vxs">
         <VXS source="SD3" type="singleEvaluation">
            <ns3:Dossier>
               <ns3:UUID>342d7b30-f0f7-4d8c-8333-0ddeeabced8a</ns3:UUID>
               <ns3:DossierId>121423</ns3:DossierId>
               <ns3:IdSD3Network>121423</ns3:IdSD3Network>
               <ns3:Country>DE</ns3:Country>
               <ns3:Language>de_DE</ns3:Language>
               <ns3:DataVersion>1</ns3:DataVersion>
               <ns3:DossierType>evaluation</ns3:DossierType>
               <ns3:CreateDate>2016-07-13T08:50:58.050+02:00</ns3:CreateDate>
               <ns3:ChangeDate>2016-07-13T08:50:58.162+02:00</ns3:ChangeDate>
               <ns3:Vehicle>
                  <ns3:DatECode>019051080040002</ns3:DatECode>
                  <ns3:Container>DE002</ns3:Container>
                  <ns3:ConstructionYear origin="dat">985</ns3:ConstructionYear>
                  <ns3:ConstructionTime>5419</ns3:ConstructionTime>
                  <ns3:InitialRegistration>2015-03-01+01:00</ns3:InitialRegistration>
                  <ns3:MileageEstimated>5500</ns3:MileageEstimated>
                  <ns3:VehicleType>1</ns3:VehicleType>
                  <ns3:Manufacturer>905</ns3:Manufacturer>
                  <ns3:BaseModel>108</ns3:BaseModel>
                  <ns3:SubModel>4</ns3:SubModel>
                  <ns3:IdentificationSource>DATECODE</ns3:IdentificationSource>
                  <ns3:SubModelVariant>2</ns3:SubModelVariant>
                  <ns1:RegistrationData>
                     <ns1:LicenseNumber>ES DAT 123</ns1:LicenseNumber>
                  </ns1:RegistrationData>
               </ns3:Vehicle>
               <ns3:VAT>
                  <ns3:VatAtConstructionTime origin="dat">19</ns3:VatAtConstructionTime>
                  <ns3:VatAtValuationTime origin="dat">19</ns3:VatAtValuationTime>
               </ns3:VAT>
               <ns3:Valuation>
                  <ns3:OriginalPrice origin="dat">27458</ns3:OriginalPrice>
                  <ns3:OriginalPriceGross origin="dat">32675</ns3:OriginalPriceGross>
                  <ns3:BasePrice origin="dat">19858.00</ns3:BasePrice>
                  <ns3:ReferenceMileage>23000</ns3:ReferenceMileage>
                  <ns3:MileageCorr origin="dat">945.80</ns3:MileageCorr>
                  <ns3:InitialRegistrationCorr origin="dat">-166.85</ns3:InitialRegistrationCorr>
                  <ns3:BasePrice2 origin="dat">20636.95</ns3:BasePrice2>
                  <ns3:EquipmentSign>calculated value</ns3:EquipmentSign>
                  <ns3:EquipmentOriginalPrice origin="dat">0</ns3:EquipmentOriginalPrice>
                  <ns3:EquipmentPrice origin="dat">0</ns3:EquipmentPrice>
                  <ns3:ValuationCorrection origin="dat">0.00</ns3:ValuationCorrection>
                  <ns3:BasePrice3 origin="dat">20636.95</ns3:BasePrice3>
                  <ns3:SalesPrice origin="dat">20636.9500</ns3:SalesPrice>
                  <ns3:SalesPriceGross origin="dat">24557.9700</ns3:SalesPriceGross>
                  <ns3:Margin origin="dat">2713.0600</ns3:Margin>
                  <ns3:MarginGross origin="dat">3228.5471</ns3:MarginGross>
                  <ns3:PurchasePrice origin="dat">17923.8800</ns3:PurchasePrice>
                  <ns3:PurchasePriceGross origin="dat">21329.4229</ns3:PurchasePriceGross>
                  <ns3:LastValuationDataYear>2016</ns3:LastValuationDataYear>
                  <ns3:LastValuationDataMonth>7</ns3:LastValuationDataMonth>
                  <ns3:LastValuationDate>2016-07-13T08:50:58.071+02:00</ns3:LastValuationDate>
                  <ns1:Currency>EUR</ns1:Currency>
                  <ns3:DefaultTiresPrice origin="dat">316.00</ns3:DefaultTiresPrice>
                  <ns3:ValuationType>residual value used vehicle</ns3:ValuationType>
                  <ns3:Parameters/>
                  <ns3:Forecasts>
                     <ns3:Forecast>
                        <ns3:ForecastType>used car</ns3:ForecastType>
                        <ns3:PriceType>sales</ns3:PriceType>
                        <ns3:IncludeVat>false</ns3:IncludeVat>
                        <ns3:CurveType>maximum</ns3:CurveType>
                        <ns3:DecreaseType>table1</ns3:DecreaseType>
                        <ns3:StartType>initial registration</ns3:StartType>
                        <ns3:ValueType>km</ns3:ValueType>
                        <ns3:MileageType>year</ns3:MileageType>
                        <ns3:ForecastItems>
                           <ns3:ForecastItem>
                              <ns3:Months>18</ns3:Months>
                              <ns3:MileagePerYear>5000</ns3:MileagePerYear>
                              <ns3:MileageTotal>6333</ns3:MileageTotal>
                              <ns3:Value>20536.84</ns3:Value>
                              <ns3:Percentage>74.7900</ns3:Percentage>
                           </ns3:ForecastItem>
                           <ns3:ForecastItem>
                              <ns3:Months>24</ns3:Months>
                              <ns3:MileagePerYear>10000</ns3:MileagePerYear>
                              <ns3:MileageTotal>12166</ns3:MileageTotal>
                              <ns3:Value>19588.96</ns3:Value>
                              <ns3:Percentage>71.3400</ns3:Percentage>
                           </ns3:ForecastItem>
                           <ns3:ForecastItem>
                              <ns3:Months>30</ns3:Months>
                              <ns3:MileagePerYear>15000</ns3:MileagePerYear>
                              <ns3:MileageTotal>23000</ns3:MileageTotal>
                              <ns3:Value>18480.90</ns3:Value>
                              <ns3:Percentage>67.3100</ns3:Percentage>
                           </ns3:ForecastItem>
                        </ns3:ForecastItems>
                     </ns3:Forecast>
                  </ns3:Forecasts>
               </ns3:Valuation>
            </ns3:Dossier>
         </VXS>
      </ns2:getUsedVehicleForecastResponse>
   </S:Body>
</S:Envelope>
```
