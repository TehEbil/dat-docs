---
title: "Response getNewVehicleForecast"
topic_id: "2200"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Standardbewertung und Standard Restwertprognose > Standard Restwertprognose Neufahrzeuge > Response getNewVehicleForecast"
---

# Response getNewVehicleForecast

Eine Beschreibung aller Response-Parameter finden Sie unter [Datenaustauschformat VXS](../../../vxs/aktenzeichenvo-1369.md).

```
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns2:getNewVehicleForecastResponse xmlns:ns2="http://sphinx.dat.de/services/Evaluation" xmlns:ns3="http://www.dat.de/vxs">
         <VXS source="SD3" type="singleEvaluation">
            <ns3:Dossier>
               <ns3:Country>DE</ns3:Country>
               <ns3:Language>de_DE</ns3:Language>
               <ns3:DatCustomerId>XXXX</ns3:DatCustomerId>
               <ns3:Vehicle>
                  <ns3:DatECode>011301200190002</ns3:DatECode>
                  <ns3:Container>DE002</ns3:Container>
                  <ns3:ConstructionTime>4990</ns3:ConstructionTime>
                  <ns3:ManufacturerName>BMW</ns3:ManufacturerName>
                  <ns3:VehicleTypeName>Pkw, SUV, Kleintransporter</ns3:VehicleTypeName>
                  <ns3:BaseModelName>MINI COUNTRYMAN (R60) (2010->)</ns3:BaseModelName>
                  <ns3:SubModelName>Cooper D All4</ns3:SubModelName>
                  <ns3:ContainerName>DE - SUV5 Cooper D (2.0 Ltr.) Euro-Norm 5, All4, 2011 - 2013</ns3:ContainerName>
                  <ns3:IdentificationSource>DATECODE</ns3:IdentificationSource>
                  <ns3:Country>DE</ns3:Country>
                  <ns3:RegistrationData/>
                  <ns3:TechInfo/>
                  <ns3:Equipment>
                     <ns3:OriginalEquipmentValue origin="dat">0</ns3:OriginalEquipmentValue>
                     <ns3:OriginalEquipmentValueGross origin="dat">0.00</ns3:OriginalEquipmentValueGross>
                     <ns3:EquipmentValueType>calculated value</ns3:EquipmentValueType>
                     <ns3:SeriesEquipment>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>11309</ns3:DatEquipmentId>
                           <ns3:Description>Uni-Lackierung</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>11704</ns3:DatEquipmentId>
                           <ns3:Description>Dach Wagenfarbe</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>15106</ns3:DatEquipmentId>
                           <ns3:Description>Außenspiegel elektr. verstellbar</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>15807</ns3:DatEquipmentId>
                           <ns3:Description>Außenspiegel Wagenfarbe</ns3:Description>
                           <ns3:OriginalPrice>42</ns3:OriginalPrice>
                           <ns3:OriginalPriceGross>49.98</ns3:OriginalPriceGross>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>19300</ns3:DatEquipmentId>
                           <ns3:Description>Heckscheibenwischer</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>24112</ns3:DatEquipmentId>
                           <ns3:Description>Audiosystem MINI CD (Radio/CD-Player)</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>24999</ns3:DatEquipmentId>
                           <ns3:Description>AUX-IN-Anschluss (AUX-IN)</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>25300</ns3:DatEquipmentId>
                           <ns3:Description>Drehzahlmesser</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>25699</ns3:DatEquipmentId>
                           <ns3:Description>Schaltpunktanzeige</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>25903</ns3:DatEquipmentId>
                           <ns3:Description>Reifendruck-Kontrollsystem</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>26803</ns3:DatEquipmentId>
                           <ns3:Description>Airbag Fahrer-/Beifahrerseite</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>26804</ns3:DatEquipmentId>
                           <ns3:Description>Kopf-Airbag-System vorn</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>26805</ns3:DatEquipmentId>
                           <ns3:Description>Kopf-Airbag-System hinten</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>26903</ns3:DatEquipmentId>
                           <ns3:Description>Seitenairbag vorn</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>26909</ns3:DatEquipmentId>
                           <ns3:Description>Airbag Beifahrerseite abschaltbar</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>28900</ns3:DatEquipmentId>
                           <ns3:Description>Klimaanlage</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>29850</ns3:DatEquipmentId>
                           <ns3:Description>Sitzbezug / Polsterung: Stoff Cosmos</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>32707</ns3:DatEquipmentId>
                           <ns3:Description>Sitz vorn links mechanisch höhenverstellbar</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>33603</ns3:DatEquipmentId>
                           <ns3:Description>Rücksitz geteilt/klappbar</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>33801</ns3:DatEquipmentId>
                           <ns3:Description>Einzelsitze im Fond</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>34805</ns3:DatEquipmentId>
                           <ns3:Description>Kopfstützen hinten</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>35003</ns3:DatEquipmentId>
                           <ns3:Description>Fensterheber elektrisch vorn + hinten</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>35301</ns3:DatEquipmentId>
                           <ns3:Description>Zentralverriegelung mit Fernbedienung</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>38890</ns3:DatEquipmentId>
                           <ns3:Description>Schienensystem Innenraum, durchgehend (Center Rail)</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>38908</ns3:DatEquipmentId>
                           <ns3:Description>Getränkehalter</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>39308</ns3:DatEquipmentId>
                           <ns3:Description>Isofix-Aufnahmen für Kindersitz an Rücksitz</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>40000</ns3:DatEquipmentId>
                           <ns3:Description>Anti-Blockier-System (ABS)</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>40050</ns3:DatEquipmentId>
                           <ns3:Description>Bremsenergierückgewinnung</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>40307</ns3:DatEquipmentId>
                           <ns3:Description>Elektron. Bremskraftverteiler</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>40801</ns3:DatEquipmentId>
                           <ns3:Description>Bremsassistent</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>47560</ns3:DatEquipmentId>
                           <ns3:Description>LM-Felgen 6,5x16 (5-Star Single Spoke)</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>68802</ns3:DatEquipmentId>
                           <ns3:Description>Reifen-Reparaturset (Mobility-Pack)</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>69505</ns3:DatEquipmentId>
                           <ns3:Description>Lenksäule (Lenkrad) mechan. verstellbar</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>69801</ns3:DatEquipmentId>
                           <ns3:Description>Servolenkung elektronisch gesteuert</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>70100</ns3:DatEquipmentId>
                           <ns3:Description>Dynamische Stabilitäts-Control (DSC)</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>70105</ns3:DatEquipmentId>
                           <ns3:Description>Dynamische Tractions Control (DTC)</ns3:Description>
                           <ns3:OriginalPrice>134</ns3:OriginalPrice>
                           <ns3:OriginalPriceGross>159.46</ns3:OriginalPriceGross>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>73015</ns3:DatEquipmentId>
                           <ns3:Description>Vlies-Batterie 70 Ah (AGM)</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>77225</ns3:DatEquipmentId>
                           <ns3:Description>Schadstoffarm nach Abgasnorm Euro 5</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>77602</ns3:DatEquipmentId>
                           <ns3:Description>Rußpartikelfilter</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>10005</ns3:DatEquipmentId>
                           <ns3:Description>Karosserie: 5-türig</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>70420</ns3:DatEquipmentId>
                           <ns3:Description>Antriebsart: Allradantrieb</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>71906</ns3:DatEquipmentId>
                           <ns3:Description>Radstand 2595 mm</ns3:Description>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>75904</ns3:DatEquipmentId>
                           <ns3:Description>Getriebe Automatik - mit Steptronic (6-Stufen)</ns3:Description>
                           <ns3:OriginalPrice>1294</ns3:OriginalPrice>
                           <ns3:OriginalPriceGross>1539.86</ns3:OriginalPriceGross>
                        </ns3:EquipmentPosition>
                        <ns3:EquipmentPosition>
                           <ns3:DatEquipmentId>86420</ns3:DatEquipmentId>
                           <ns3:Description>Motor 2,0 Ltr. - 82 kW Turbodiesel KAT</ns3:Description>
                        </ns3:EquipmentPosition>
                     </ns3:SeriesEquipment>
                  </ns3:Equipment>
                  <ns3:DATECodeEquipment>
                     <ns3:EquipmentPosition>
                        <ns3:DatEquipmentId>86420</ns3:DatEquipmentId>
                        <ns3:Description>Motor 2,0 Ltr. - 82 kW Turbodiesel KAT</ns3:Description>
                     </ns3:EquipmentPosition>
                     <ns3:EquipmentPosition>
                        <ns3:DatEquipmentId>10005</ns3:DatEquipmentId>
                        <ns3:Description>Karosserie: 5-türig</ns3:Description>
                     </ns3:EquipmentPosition>
                     <ns3:EquipmentPosition>
                        <ns3:DatEquipmentId>71906</ns3:DatEquipmentId>
                        <ns3:Description>Radstand 2595 mm</ns3:Description>
                     </ns3:EquipmentPosition>
                     <ns3:EquipmentPosition>
                        <ns3:DatEquipmentId>70420</ns3:DatEquipmentId>
                        <ns3:Description>Antriebsart: Allradantrieb</ns3:Description>
                     </ns3:EquipmentPosition>
                     <ns3:EquipmentPosition>
                        <ns3:DatEquipmentId>75904</ns3:DatEquipmentId>
                        <ns3:Description>Getriebe Automatik - mit Steptronic (6-Stufen)</ns3:Description>
                     </ns3:EquipmentPosition>
                  </ns3:DATECodeEquipment>
               </ns3:Vehicle>
               <ns3:VAT>
                  <ns3:VatAtConstructionTime>19</ns3:VatAtConstructionTime>
               </ns3:VAT>
               <ns3:Valuation>
                  <ns3:OriginalPrice origin="dat">23059</ns3:OriginalPrice>
                  <ns3:OriginalPriceGross origin="dat">27440</ns3:OriginalPriceGross>
                  <ns3:EquipmentSign>calculated value</ns3:EquipmentSign>
                  <ns3:EquipmentOriginalPrice origin="dat">0</ns3:EquipmentOriginalPrice>
                  <ns3:LastValuationDataYear>2013</ns3:LastValuationDataYear>
                  <ns3:LastValuationDataMonth>1</ns3:LastValuationDataMonth>
                  <ns3:LastValuationDate>2013-01-16T14:15:40.244+01:00</ns3:LastValuationDate>
                  <ns1:Currency>EUR</ns1:Currency>
                  <ns3:ValuationType>residual value new vehicle</ns3:ValuationType>
                  <ns3:Condition/>
                  <ns3:Parameters/>
                  <ns3:Forecasts>
                     <ns3:Forecast>
                        <ns3:ForecastType>new car</ns3:ForecastType>
                        <ns3:PriceType>sales</ns3:PriceType>
                        <ns3:IncludeVat>true</ns3:IncludeVat>
                        <ns3:CurveType>maximum</ns3:CurveType>
                        <ns3:DecreaseType>residual value</ns3:DecreaseType>
                        <ns3:StartType>initial registration</ns3:StartType>
                        <ns3:ValueType>monetary</ns3:ValueType>
                        <ns3:MileageType>year</ns3:MileageType>
                        <ns3:ForecastItems>
                           <ns3:ForecastItem>
                              <ns3:Months>36</ns3:Months>
                              <ns3:MileagePerYear>2147</ns3:MileagePerYear>
                              <ns3:MileageTotal>6441</ns3:MileageTotal>
                              <ns3:Value>19559.14</ns3:Value>
                              <ns3:Percentage>71.2800</ns3:Percentage>
                              <ns3:PercentageGross>71.2800</ns3:PercentageGross>
                           </ns3:ForecastItem>
                        </ns3:ForecastItems>
                     </ns3:Forecast>
                  </ns3:Forecasts>
               </ns3:Valuation>
            </ns3:Dossier>
         </VXS>
      </ns2:getNewVehicleForecastResponse>
   </S:Body>
</S:Envelope>
```
