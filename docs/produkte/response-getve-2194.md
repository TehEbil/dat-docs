---
title: "Response getVehicleApproximateValue"
topic_id: "2194"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Annäherungsbewertung > Response getVehicleApproximateValue"
---

# Response getVehicleApproximateValue

Eine Beschreibung aller Response-Parameter finden Sie unter [Datenaustauschformat VXS](#showid/1369 "Aktenzeichen/Vorgänge (Dossiers)").

```
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns2:getVehicleApproximateValueResponse xmlns:ns2="http://sphinx.dat.de/services/Evaluation" xmlns:ns3="http://www.dat.de/vxs">
         <VXS source="SD3" type="singleEvaluation">
            <ns3:Dossier>
               <ns3:Country>DE</ns3:Country>
               <ns3:Language>de_DE</ns3:Language>
               <ns3:DatCustomerId>XXXX</ns3:DatCustomerId>
               <ns3:Vehicle>
                  <ns3:DatECode>019051050020005</ns3:DatECode>
                  <ns3:Container>DE004</ns3:Container>
                  <ns3:ConstructionYear origin="dat">987</ns3:ConstructionYear>
                  <ns3:ConstructionTime>5260</ns3:ConstructionTime>
                  <ns3:InitialRegistration>2013-10-21+02:00</ns3:InitialRegistration>
                  <ns3:MileageEstimated>52766</ns3:MileageEstimated>
                  <ns3:SalesDescription>Golf VII 1.6 TDI Trendline BMT</ns3:SalesDescription>
                  <ns3:VehicleTypeName>Pkw, SUV, Kleintransporter</ns3:VehicleTypeName>
                  <ns3:ManufacturerName origin="dat">Volkswagen</ns3:ManufacturerName>
                  <ns3:BaseModelName origin="dat">Golf VII Lim. (5G1/BE1)(09.2012->)</ns3:BaseModelName>
                  <ns3:SubModelName origin="dat">Trendline BMT</ns3:SubModelName>
                  <ns3:ContainerName>DE - LimS5 1.6 TDI BMT EU5, Trendline, 2012 - 2014</ns3:ContainerName>
                  <ns3:VehicleType>1</ns3:VehicleType>
                  <ns3:Manufacturer>905</ns3:Manufacturer>
                  <ns3:BaseModel>105</ns3:BaseModel>
                  <ns3:SubModel>2</ns3:SubModel>
                  <ns3:IdentificationSource>KBA</ns3:IdentificationSource>
                  <ns3:Country>DE</ns3:Country>
                  <ns3:SubModelVariant>5</ns3:SubModelVariant>
                  <ns3:RegistrationData>
                     <ns3:KbaCode>0603/BJH</ns3:KbaCode>
                  </ns3:RegistrationData>
                  <ns3:Engine/>
                  <ns3:TechInfo>
                     <ns3:GearboxType>manual</ns3:GearboxType>
                     <ns3:InsuranceTypeClassLiability>16</ns3:InsuranceTypeClassLiability>
                     <ns3:InsuranceTypeClassCascoPartial>21</ns3:InsuranceTypeClassCascoPartial>
                     <ns3:InsuranceTypeClassCascoComplete>17</ns3:InsuranceTypeClassCascoComplete>
                     <ns3:ProductGroupName/>
                  </ns3:TechInfo>
                  <ns3:Equipment>
                     <ns3:EquipmentValue origin="dat">0</ns3:EquipmentValue>
                     <ns3:EquipmentValueGross origin="dat">0.00</ns3:EquipmentValueGross>
                     <ns3:OriginalEquipmentValue origin="dat">0</ns3:OriginalEquipmentValue>
                     <ns3:OriginalEquipmentValueGross origin="dat">0.00</ns3:OriginalEquipmentValueGross>
                     <ns3:EquipmentValueType>calculated value</ns3:EquipmentValueType>
                     <ns3:SeriesEquipment>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>2904</ns3:DatEquipmentId>
                           <ns3:Description>Nichtraucher-Paket</ns3:Description>
                        </ns3:EquipmentPosition>
                        ...
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>75005</ns3:DatEquipmentId>
                           <ns3:Description>Getriebe 5-Gang</ns3:Description>
                           <ns3:EquipmentGroup>SG5</ns3:EquipmentGroup>
                           <ns3:EquipmentType>glass</ns3:EquipmentType>
                           <ns3:GearBoxType>manual</ns3:GearBoxType>
                           <ns3:NrOfGears>5</ns3:NrOfGears>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>96530</ns3:DatEquipmentId>
                           <ns3:Description>Motor 1,6 Ltr. - 77 kW TDI DPF</ns3:Description>
                           <ns3:EquipmentType>engine</ns3:EquipmentType>
                           <ns3:ContainedEquipmentPositions>
                              <ns3:EquipmentPosition>
                                 <ns3:DatEquipmentId>77602</ns3:DatEquipmentId>
                                 <ns3:Description>Rußpartikelfilter</ns3:Description>
                                 <ns3:EquipmentGroup>DPF</ns3:EquipmentGroup>
                              </ns3:EquipmentPosition>
                           </ns3:ContainedEquipmentPositions>
                        </ns3:EquipmentPosition>
                     </ns3:SeriesEquipment>
                  </ns3:Equipment>
                  <ns3:Tires>
                     <ns3:Axles/>
                  </ns3:Tires>
                  <ns3:DATECodeEquipment>
                     <ns3:EquipmentPosition>
                        <ns3:DatEquipmentId>96530</ns3:DatEquipmentId>
                        <ns3:Description>Motor 1,6 Ltr. - 77 kW TDI DPF</ns3:Description>
                     </ns3:EquipmentPosition>
                     <ns3:EquipmentPosition>
                        <ns3:DatEquipmentId>10004</ns3:DatEquipmentId>
                        <ns3:Description>Karosserie: 4-türig</ns3:Description>
                     </ns3:EquipmentPosition>
                     <ns3:EquipmentPosition>
                        <ns3:DatEquipmentId>75005</ns3:DatEquipmentId>
                        <ns3:Description>Getriebe 5-Gang</ns3:Description>
                     </ns3:EquipmentPosition>
                  </ns3:DATECodeEquipment>
               </ns3:Vehicle>
               <ns3:VAT>
                  <ns3:VatType>difference</ns3:VatType>
                  <ns3:VatAtConstructionTime origin="dat">19</ns3:VatAtConstructionTime>
                  <ns3:VatAtValuationTime origin="dat">19</ns3:VatAtValuationTime>
               </ns3:VAT>
               <ns3:Valuation>
                  <ns3:OriginalPrice origin="dat">18382</ns3:OriginalPrice>
                  <ns3:OriginalPriceGross origin="dat">21875</ns3:OriginalPriceGross>
                  <ns3:BasePrice origin="dat">10138.00</ns3:BasePrice>
                  <ns3:ReferenceMileage>57000</ns3:ReferenceMileage>
                  <ns3:MileageCorr origin="dat">142.07</ns3:MileageCorr>
                  <ns3:InitialRegistrationCorr origin="dat">102.29</ns3:InitialRegistrationCorr>
                  <ns3:BasePrice2 origin="dat">10382.36</ns3:BasePrice2>
                  <!-- EquipmentSign = flat-rate value when using flat rate option -->
                  <ns3:EquipmentSign>calculated value</ns3:EquipmentSign>
                  <!-- when using flat rate option the additional element ManualEquipmentOrignalPrice will occur -->
                  <!-- ns3:ManualEquipmentOrignalPrice>1300</ns3:ManualEquipmentOrignalPrice -->
                  <ns3:EquipmentOriginalPrice origin="dat">0</ns3:EquipmentOriginalPrice>
                  <ns3:EquipmentPrice origin="dat">0</ns3:EquipmentPrice>
                  <ns3:ValuationCorrection origin="dat">0.00</ns3:ValuationCorrection>
                  <ns3:BasePrice3 origin="dat">10382.36</ns3:BasePrice3>
                  <ns3:SalesPrice origin="dat">12055.6100</ns3:SalesPrice>
                  <ns3:SalesPriceGross origin="dat">12355.0100</ns3:SalesPriceGross>
                  <ns3:Margin origin="dat">1575.8000</ns3:Margin>
                  <ns3:MarginGross origin="dat">1875.2049</ns3:MarginGross>
                  <ns3:PurchasePrice origin="dat">10479.8051</ns3:PurchasePrice>
                  <ns3:PurchasePriceGross origin="dat">10479.8051</ns3:PurchasePriceGross>
                  <ns3:LastValuationDataYear>2016</ns3:LastValuationDataYear>
                  <ns3:LastValuationDataMonth>6</ns3:LastValuationDataMonth>
                  <ns3:LastValuationDate>2016-06-03T11:53:24.245+02:00</ns3:LastValuationDate>
                  <ns1:Currency>EUR</ns1:Currency>
                  <ns3:DefaultTiresPrice origin="dat">160.00</ns3:DefaultTiresPrice>
                  <ns3:ValuationType>valuation</ns3:ValuationType>
                  <ns3:Parameters/>
               </ns3:Valuation>
            </ns3:Dossier>
         </VXS>
      </ns2:getVehicleApproximateValueResponse>
   </S:Body>
</S:Envelope>
```
