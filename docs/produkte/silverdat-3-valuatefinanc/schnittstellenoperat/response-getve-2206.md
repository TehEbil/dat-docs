---
title: "Response getVehicleTargetDateEvaluationHistory"
topic_id: "2206"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Stichtagsbezogene Bewertung durchführen (Historische Bewertung) > Response getVehicleTargetDateEvaluationHistory"
---

# Response getVehicleTargetDateEvaluationHistory

Eine Beschreibung aller Response-Parameter finden Sie unter [Datenaustauschformat VXS](../../../vxs/aktenzeichenvorgange-doss/index.md).

```
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns4:getVehicleTargetDateEvaluationHistoryResponse xmlns:ns4="http://sphinx.dat.de/services/Evaluation">
         <VXS source="SD3" type="singleEvaluation">
            <ns1:Dossier xmlns:ns1="http://www.dat.de/vxs">
               <ns1:UUID>789a92f7-a1f2-4f68-b501-5a127595c87c</ns1:UUID>
               <ns1:Country>DE</ns1:Country>
               <ns1:Language>de_DE</ns1:Language>
               <ns1:DataVersion>1</ns1:DataVersion>
               <ns1:DatCustomerId>XXXX</ns1:DatCustomerId>
               <ns1:DossierType>historic evaluation</ns1:DossierType>
               <ns1:CreateDate>2024-07-25T14:35:50.412+02:00</ns1:CreateDate>
               <ns1:ChangeDate>2024-07-25T14:35:50.412+02:00</ns1:ChangeDate>
               <ns1:ProcedureType>EVALUATION</ns1:ProcedureType>
               <ns1:Vehicle>
                  <ns1:DatECode>019051080040002</ns1:DatECode>
                  <ns1:Container>DE002</ns1:Container>
                  <ns1:ConstructionYear origin="dat">982</ns1:ConstructionYear>
                  <ns1:ConstructionTime>5419</ns1:ConstructionTime>
                  <ns1:InitialRegistration>2018-11-01+01:00</ns1:InitialRegistration>
                  <ns1:MileageEstimated>50000</ns1:MileageEstimated>
                  <ns1:SalesDescription>Golf VII Alltrack 2.0 TDI 4Motion BMT</ns1:SalesDescription>
                  <ns1:VehicleTypeName>Pkw, SUV, Kleintransporter</ns1:VehicleTypeName>
                  <ns1:VehicleTypeNameN origin="dat">Pkw, SUV, Kleintransporter</ns1:VehicleTypeNameN>
                  <ns1:ManufacturerName origin="dat">Volkswagen</ns1:ManufacturerName>
                  <ns1:BaseModelName origin="dat">Golf VII Alltrack Variant (BA5)(11.2014->2017)</ns1:BaseModelName>
                  <ns1:SubModelName origin="dat">Basis BMT 4Motion</ns1:SubModelName>
                  <ns1:ContainerName>DE - Kb5 2.0 TDI 4Motion BMT/Start-Stopp EU6, 2014 - 2017</ns1:ContainerName>
                  <ns1:ContainerNameN origin="dat">DE - Kb5 2.0 TDI 4Motion BMT/Start-Stopp EU6, 2014 - 2017</ns1:ContainerNameN>
                  <ns1:VehicleType>1</ns1:VehicleType>
                  <ns1:Manufacturer>905</ns1:Manufacturer>
                  <ns1:BaseModel>108</ns1:BaseModel>
                  <ns1:SubModel>4</ns1:SubModel>
                  <ns1:IdentificationSource>DATECODE</ns1:IdentificationSource>
                  <ns1:Country>DE</ns1:Country>
                  <ns1:ReleaseIndicator>APPRAISAL</ns1:ReleaseIndicator>
                  <ns1:SubModelVariant>2</ns1:SubModelVariant>
                  <ns1:RegistrationData>
                     <ns1:LicenseNumber>ES DAT 123</ns1:LicenseNumber>
                  </ns1:RegistrationData>
                  <ns1:Engine>
                     <ns1:FuelMethod origin="dat">diesel</ns1:FuelMethod>
                     <ns1:EnginePowerKw origin="dat">110</ns1:EnginePowerKw>
                     <ns1:EnginePowerHp origin="dat">149</ns1:EnginePowerHp>
                     <ns1:Cylinders origin="dat">4</ns1:Cylinders>
                     <ns1:Capacity origin="dat">1968</ns1:Capacity>
                     <ns1:Consumption>4.9</ns1:Consumption>
                     <ns1:Co2Emission>127.0</ns1:Co2Emission>
                  </ns1:Engine>
                  <ns1:TechInfo>
                     <ns1:StructureType>Kb</ns1:StructureType>
                     <ns1:StructureDescription origin="dat">Kombi</ns1:StructureDescription>
                     <ns1:CountOfAxles origin="dat">2</ns1:CountOfAxles>
                     <ns1:CountOfDrivedAxles origin="dat">2</ns1:CountOfDrivedAxles>
                     <ns1:WheelBase origin="dat">2630</ns1:WheelBase>
                     <ns1:Length origin="dat">4578</ns1:Length>
                     <ns1:Width origin="dat">1799</ns1:Width>
                     <ns1:Height origin="dat">1515</ns1:Height>
                     <ns1:RoofLoad origin="dat">75</ns1:RoofLoad>
                     <ns1:TrailerLoadBraked origin="dat">2000</ns1:TrailerLoadBraked>
                     <ns1:TrailerLoadUnbraked origin="dat">750</ns1:TrailerLoadUnbraked>
                     <ns1:VehicleSeats origin="dat">5</ns1:VehicleSeats>
                     <ns1:VehicleDoors origin="dat">5</ns1:VehicleDoors>
                     <ns1:CountOfAirbags origin="dat">5</ns1:CountOfAirbags>
                     <ns1:Acceleration origin="dat">8.9</ns1:Acceleration>
                     <ns1:SpeedMax origin="dat">207</ns1:SpeedMax>
                     <ns1:PowerHp origin="dat">150</ns1:PowerHp>
                     <ns1:PowerKw origin="dat">110.0</ns1:PowerKw>
                     <ns1:Capacity origin="dat">1968</ns1:Capacity>
                     <ns1:Cylinder origin="dat">4</ns1:Cylinder>
                     <ns1:CylinderArrangement origin="dat">R</ns1:CylinderArrangement>
                     <ns1:RotationsOnMaxPower origin="dat">3500</ns1:RotationsOnMaxPower>
                     <ns1:RotationsOnMaxTorque origin="dat">1750</ns1:RotationsOnMaxTorque>
                     <ns1:Torque origin="dat">340</ns1:Torque>
                     <ns1:GearboxType>manual</ns1:GearboxType>
                     <ns1:OriginalTireSizeAxle1>205/55R17</ns1:OriginalTireSizeAxle1>
                     <ns1:OriginalTireSizeAxle2>205/55R17</ns1:OriginalTireSizeAxle2>
                     <ns1:TankVolume origin="dat">55</ns1:TankVolume>
                     <ns1:ConsumptionInTown origin="dat">5.9</ns1:ConsumptionInTown>
                     <ns1:ConsumptionOutOfTown origin="dat">4.4</ns1:ConsumptionOutOfTown>
                     <ns1:Consumption origin="dat">4.9</ns1:Consumption>
                     <ns1:Co2Emission origin="dat">127.0</ns1:Co2Emission>
                     <ns1:EmissionClass origin="dat">EU6</ns1:EmissionClass>
                     <ns1:Drive origin="dat">A</ns1:Drive>
                     <ns1:DriveN origin="dat">Allradantrieb</ns1:DriveN>
                     <ns1:DriveCode>A</ns1:DriveCode>
                     <ns1:EngineCycle origin="dat">4</ns1:EngineCycle>
                     <ns1:FuelMethod origin="dat">Diesel</ns1:FuelMethod>
                     <ns1:FuelMethodCode>D</ns1:FuelMethodCode>
                     <ns1:FuelMethodType origin="dat">D</ns1:FuelMethodType>
                     <ns1:UnloadedWeight origin="dat">1555</ns1:UnloadedWeight>
                     <ns1:PermissableTotalWeight origin="dat">2050</ns1:PermissableTotalWeight>
                     <ns1:Payload origin="dat">570</ns1:Payload>
                     <ns1:LoadingSpace origin="dat">605</ns1:LoadingSpace>
                     <ns1:LoadingSpaceMax origin="dat">1620</ns1:LoadingSpaceMax>
                     <ns1:ProductGroupName>untere Mittelklasse / Kompaktklasse</ns1:ProductGroupName>
                     <ns1:FuelmethodAbbr>D</ns1:FuelmethodAbbr>
                     <ns1:WidthForGarage origin="dat">2027</ns1:WidthForGarage>
                     <ns1:TechInfoWltp/>
                  </ns1:TechInfo>
                  <ns1:Equipment>
                     <ns1:ColorVariant origin="user">Normal</ns1:ColorVariant>
                     <ns1:LacquerType origin="user">Normal</ns1:LacquerType>
                     <ns1:EquipmentValue origin="dat">0</ns1:EquipmentValue>
                     <ns1:EquipmentValueGross origin="dat">0.00</ns1:EquipmentValueGross>
                     <ns1:OriginalEquipmentValue origin="dat">0</ns1:OriginalEquipmentValue>
                     <ns1:OriginalEquipmentValueGross origin="dat">0.00</ns1:OriginalEquipmentValueGross>
                     <ns1:EquipmentValueType>calculated value</ns1:EquipmentValueType>
                     <ns1:SeriesEquipment>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>1100</ns1:DatEquipmentId>
                           <ns1:Description>Chrom-Paket (1)</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>25260</ns1:DatEquipmentId>
                                 <ns1:Description>Chromeinfassung Lichtschalter</ns1:Description>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>25265</ns1:DatEquipmentId>
                                 <ns1:Description>Chromeinfassung Spiegelverstellung</ns1:Description>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>2904</ns1:DatEquipmentId>
                           <ns1:Description>Nichtraucher-Paket</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>12501</ns1:DatEquipmentId>
                           <ns1:Description>Unterfahrschutz vorn</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>12507</ns1:DatEquipmentId>
                           <ns1:Description>Unterfahrschutz Triebwerk (Motor und Getriebe)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>12877</ns1:DatEquipmentId>
                           <ns1:Description>Kühlergrill schwarz mit Chromleiste unten, matt</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>13002</ns1:DatEquipmentId>
                           <ns1:Description>Chromleisten an Seitenfenstern</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>13106</ns1:DatEquipmentId>
                           <ns1:Description>Einstiegsleisten (Edelstahl)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>15201</ns1:DatEquipmentId>
                           <ns1:Description>Außenspiegel elektr. verstell- und heizbar, beide</ns1:Description>
                           <ns1:EquipmentGroup>AUSP</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>15804</ns1:DatEquipmentId>
                           <ns1:Description>Außenspiegel asphärisch, links</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>15806</ns1:DatEquipmentId>
                           <ns1:Description>Außenspiegel verchromt</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>16205</ns1:DatEquipmentId>
                           <ns1:Description>Dachreling silber eloxiert</ns1:Description>
                           <ns1:EquipmentGroup>DARE</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18205</ns1:DatEquipmentId>
                           <ns1:Description>Leuchtweitenregelung</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18207</ns1:DatEquipmentId>
                           <ns1:Description>Blinkleuchte in Außenspiegel integriert</ns1:Description>
                           <ns1:EquipmentGroup>AUSP</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18617</ns1:DatEquipmentId>
                           <ns1:Description>Nebelscheinwerfer mit integriertem Abbiegelicht</ns1:Description>
                           <ns1:EquipmentGroup>AKLI</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>18618</ns1:DatEquipmentId>
                                 <ns1:Description>Abbiegelicht</ns1:Description>
                                 <ns1:EquipmentGroup>AKLI</ns1:EquipmentGroup>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18700</ns1:DatEquipmentId>
                           <ns1:Description>Nebelschlussleuchte</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18804</ns1:DatEquipmentId>
                           <ns1:Description>Heckleuchten dunkel getönt</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18830</ns1:DatEquipmentId>
                           <ns1:Description>Kennzeichenbeleuchtung LED</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18904</ns1:DatEquipmentId>
                           <ns1:Description>Tagfahrlicht</ns1:Description>
                           <ns1:EquipmentGroup>TFAL</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>19009</ns1:DatEquipmentId>
                           <ns1:Description>Scheibenwischer mit Intervallschaltung, regulierbar</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>19300</ns1:DatEquipmentId>
                           <ns1:Description>Heckscheibenwischer</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>22304</ns1:DatEquipmentId>
                           <ns1:Description>Wärmeschutzverglasung grün getönt</ns1:Description>
                           <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>22508</ns1:DatEquipmentId>
                           <ns1:Description>Frontscheibe Verbundglas getönt</ns1:Description>
                           <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>24153</ns1:DatEquipmentId>
                           <ns1:Description>Audiosystem Composition Touch (Touchscreen, MP3, SD-Karten-Schnittstelle, AUX-IN)</ns1:Description>
                           <ns1:EquipmentGroup>CD</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>25016</ns1:DatEquipmentId>
                                 <ns1:Description>Multimediabuchse AUX-IN</ns1:Description>
                                 <ns1:EquipmentGroup>MP3A</ns1:EquipmentGroup>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25603</ns1:DatEquipmentId>
                           <ns1:Description>Multifunktionsanzeige Plus</ns1:Description>
                           <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25800</ns1:DatEquipmentId>
                           <ns1:Description>Einparkhilfe vorn und hinten</ns1:Description>
                           <ns1:EquipmentGroup>PDC3</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>15897</ns1:DatEquipmentId>
                                 <ns1:Description>Außenspiegel mit autom. Absenkfunktion, rechts</ns1:Description>
                                 <ns1:EquipmentGroup>AUSP</ns1:EquipmentGroup>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25906</ns1:DatEquipmentId>
                           <ns1:Description>Reifenkontroll-Anzeige</ns1:Description>
                           <ns1:EquipmentGroup>RDK</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26167</ns1:DatEquipmentId>
                           <ns1:Description>Innenausstattung: Dekoreinlagen Dark Magnesium</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26603</ns1:DatEquipmentId>
                           <ns1:Description>Pedale Edelstahl / Aluminium-Design</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26701</ns1:DatEquipmentId>
                           <ns1:Description>Knieairbag Fahrerseite</ns1:Description>
                           <ns1:EquipmentGroup>AIR5</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26803</ns1:DatEquipmentId>
                           <ns1:Description>Airbag Fahrer-/Beifahrerseite</ns1:Description>
                           <ns1:EquipmentGroup>AIR1</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26909</ns1:DatEquipmentId>
                           <ns1:Description>Airbag Beifahrerseite abschaltbar</ns1:Description>
                           <ns1:EquipmentGroup>AIR2</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26913</ns1:DatEquipmentId>
                           <ns1:Description>Kopf-Airbag-System vorn und hinten inkl. Seitenairbag vorn</ns1:Description>
                           <ns1:EquipmentGroup>AIR4</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27104</ns1:DatEquipmentId>
                           <ns1:Description>Ablagefach am Dachhimmel</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27207</ns1:DatEquipmentId>
                           <ns1:Description>Mittelarmlehne vorn klappbar</ns1:Description>
                           <ns1:EquipmentGroup>MALV</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27400</ns1:DatEquipmentId>
                           <ns1:Description>Gepäckraumabdeckung / Rollo</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>28916</ns1:DatEquipmentId>
                           <ns1:Description>Klimaanlage Climatronic 2-Zonen</ns1:Description>
                           <ns1:EquipmentGroup>KLI2</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>29108</ns1:DatEquipmentId>
                           <ns1:Description>Innenraumfilter: Staub- und Pollenfilter</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>30500</ns1:DatEquipmentId>
                           <ns1:Description>Sitzbezug / Polsterung: Stoff</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>32704</ns1:DatEquipmentId>
                           <ns1:Description>Sitz vorn links höhenverstellbar</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>33005</ns1:DatEquipmentId>
                           <ns1:Description>Sitzlehne vorn rechts umklappbar</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>33302</ns1:DatEquipmentId>
                           <ns1:Description>Ablagetasche an Vordersitzlehnen</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>33305</ns1:DatEquipmentId>
                           <ns1:Description>Lendenwirbelstützen vorn</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>33502</ns1:DatEquipmentId>
                           <ns1:Description>Rücksitzlehne geteilt</ns1:Description>
                           <ns1:EquipmentGroup>SITH</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>33513</ns1:DatEquipmentId>
                                 <ns1:Description>Rücksitzlehnen mit Fernentriegelung umklappbar</ns1:Description>
                                 <ns1:EquipmentGroup>SITH</ns1:EquipmentGroup>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>34807</ns1:DatEquipmentId>
                           <ns1:Description>Kopfstützen hinten (3-fach)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35003</ns1:DatEquipmentId>
                           <ns1:Description>Fensterheber elektrisch vorn und hinten</ns1:Description>
                           <ns1:EquipmentGroup>FH4</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35301</ns1:DatEquipmentId>
                           <ns1:Description>Zentralverriegelung mit Fernbedienung</ns1:Description>
                           <ns1:EquipmentGroup>ZV</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>36404</ns1:DatEquipmentId>
                           <ns1:Description>Türgriffe außen Wagenfarbe</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>37008</ns1:DatEquipmentId>
                           <ns1:Description>3-Punkt-Sicherheitsgurt hinten mitte</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>37107</ns1:DatEquipmentId>
                           <ns1:Description>Warnanlage für Sicherheitsgurte vorn</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>37605</ns1:DatEquipmentId>
                           <ns1:Description>Ambiente-Beleuchtung Türverkleidung</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>37616</ns1:DatEquipmentId>
                           <ns1:Description>Fußraumbeleuchtung vorn</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>37719</ns1:DatEquipmentId>
                           <ns1:Description>Leseleuchten vorn und hinten LED</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>37900</ns1:DatEquipmentId>
                           <ns1:Description>Innenspiegel abblendbar</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>37905</ns1:DatEquipmentId>
                           <ns1:Description>Sonnenblenden mit Spiegel (beleuchtet)</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>38106</ns1:DatEquipmentId>
                           <ns1:Description>Wegfahrsperre (elektronisch)</ns1:Description>
                           <ns1:EquipmentGroup>WFS</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39003</ns1:DatEquipmentId>
                           <ns1:Description>Getränkehalter vorn</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39007</ns1:DatEquipmentId>
                           <ns1:Description>Steckdose 12V im Koffer-/Laderaum</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39205</ns1:DatEquipmentId>
                           <ns1:Description>Schalt-/Wählhebelgriff Leder</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39303</ns1:DatEquipmentId>
                           <ns1:Description>Fußmatten Textil</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39308</ns1:DatEquipmentId>
                           <ns1:Description>Isofix-Aufnahmen für Kindersitz an Rücksitz</ns1:Description>
                           <ns1:EquipmentGroup>KISI</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39502</ns1:DatEquipmentId>
                           <ns1:Description>Schublade / Ablagefach unter Sitz vorn rechts</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39504</ns1:DatEquipmentId>
                           <ns1:Description>Schublade / Ablagefach unter Sitz vorn links</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39506</ns1:DatEquipmentId>
                           <ns1:Description>Handschuhfach mit Kühlfunktion</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39531</ns1:DatEquipmentId>
                           <ns1:Description>Verbandkasten und Warndreieck</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40060</ns1:DatEquipmentId>
                           <ns1:Description>Bremsbelagverschleissanzeige</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40801</ns1:DatEquipmentId>
                           <ns1:Description>Bremsassistent</ns1:Description>
                           <ns1:EquipmentGroup>FA01</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40803</ns1:DatEquipmentId>
                           <ns1:Description>Parkbremse elektrisch</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>40906</ns1:DatEquipmentId>
                                 <ns1:Description>Auto-Hold-Funktion</ns1:Description>
                                 <ns1:EquipmentGroup>FA16</ns1:EquipmentGroup>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40959</ns1:DatEquipmentId>
                           <ns1:Description>Fahrassistenz-System: Multikollisionsbremse (Multi Collision Brake)</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>42205</ns1:DatEquipmentId>
                           <ns1:Description>Schlechtwege-Fahrwerk</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>42926</ns1:DatEquipmentId>
                           <ns1:Description>Fahrassistenz-System: Müdigkeitserkennung</ns1:Description>
                           <ns1:EquipmentGroup>FA41</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>48273</ns1:DatEquipmentId>
                           <ns1:Description>LM-Felgen</ns1:Description>
                           <ns1:EquipmentGroup>ALU</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>68802</ns1:DatEquipmentId>
                           <ns1:Description>Reifen-Reparaturkit (Tire Mobility Set)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>69009</ns1:DatEquipmentId>
                           <ns1:Description>Lenkrad (Leder)</ns1:Description>
                           <ns1:EquipmentGroup>LEN1</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>69502</ns1:DatEquipmentId>
                           <ns1:Description>Lenksäule (Lenkrad) mechan. verstellbar, Höhen-/Längsverstellung</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>69801</ns1:DatEquipmentId>
                           <ns1:Description>Servolenkung elektronisch gesteuert (Servotronic)</ns1:Description>
                           <ns1:EquipmentGroup>SL</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>70042</ns1:DatEquipmentId>
                           <ns1:Description>Elektron. Differentialsperre (XDS)</ns1:Description>
                           <ns1:EquipmentGroup>ASD</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>70311</ns1:DatEquipmentId>
                           <ns1:Description>Elektron. Stabilitäts-Programm (ESP) Bremsassistent, ASR/ABS, EDS</ns1:Description>
                           <ns1:EquipmentGroup>ESP</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>40000</ns1:DatEquipmentId>
                                 <ns1:Description>Anti-Blockier-System (ABS)</ns1:Description>
                                 <ns1:EquipmentGroup>ABS</ns1:EquipmentGroup>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>70108</ns1:DatEquipmentId>
                                 <ns1:Description>Elektron. Differentialsperre (EDS)</ns1:Description>
                                 <ns1:EquipmentGroup>ASD</ns1:EquipmentGroup>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>70303</ns1:DatEquipmentId>
                                 <ns1:Description>Antriebs-Schlupfregelung (ASR)</ns1:Description>
                                 <ns1:EquipmentGroup>ASR</ns1:EquipmentGroup>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>70308</ns1:DatEquipmentId>
                                 <ns1:Description>Elektron. Stabilitäts-Programm (ESP)</ns1:Description>
                                 <ns1:EquipmentGroup>ESP</ns1:EquipmentGroup>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>70420</ns1:DatEquipmentId>
                           <ns1:Description>Antriebsart: Allradantrieb</ns1:Description>
                           <ns1:EquipmentGroup>4WD</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>70510</ns1:DatEquipmentId>
                           <ns1:Description>Fahrassistenz-System: Off-Road-Fahrprogramm</ns1:Description>
                           <ns1:EquipmentGroup>FA22</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>70517</ns1:DatEquipmentId>
                           <ns1:Description>Fahrassistenz-System: Fahrprofilauswahl</ns1:Description>
                           <ns1:EquipmentGroup>FA22</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>77227</ns1:DatEquipmentId>
                           <ns1:Description>Schadstoffarm nach Abgasnorm Euro 6</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>77601</ns1:DatEquipmentId>
                           <ns1:Description>Start/Stop-Anlage</ns1:Description>
                           <ns1:EquipmentGroup>MSSA</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>77602</ns1:DatEquipmentId>
                           <ns1:Description>Rußpartikelfilter</ns1:Description>
                           <ns1:EquipmentGroup>DPF</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>10004</ns1:DatEquipmentId>
                           <ns1:Description>Karosserie: 4-türig</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>75205</ns1:DatEquipmentId>
                           <ns1:Description>Getriebe 6-Gang</ns1:Description>
                           <ns1:EquipmentGroup>SG6</ns1:EquipmentGroup>
                           <ns1:GearBoxType>manual</ns1:GearBoxType>
                           <ns1:NrOfGears>6</ns1:NrOfGears>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>96556</ns1:DatEquipmentId>
                           <ns1:Description>Motor 2,0 Ltr. - 110 kW TDI</ns1:Description>
                           <ns1:EquipmentType>engine</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                     </ns1:SeriesEquipment>
                     <ns1:DeselectedSeriesEquipment>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>74900</ns1:DatEquipmentId>
                           <ns1:Description>Getriebe 6-Gang - Doppelkupplungsgetriebe DSG</ns1:Description>
                        </ns1:EquipmentPosition>
                     </ns1:DeselectedSeriesEquipment>
                  </ns1:Equipment>
                  <ns1:Tires>
                     <ns1:Axles/>
                  </ns1:Tires>
                  <ns1:DATECodeEquipment>
                     <ns1:EquipmentPosition>
                        <ns1:DatEquipmentId>96556</ns1:DatEquipmentId>
                        <ns1:Description>Motor 2,0 Ltr. - 110 kW TDI</ns1:Description>
                        <ns1:EquipmentClass>1</ns1:EquipmentClass>
                     </ns1:EquipmentPosition>
                     <ns1:EquipmentPosition>
                        <ns1:DatEquipmentId>10004</ns1:DatEquipmentId>
                        <ns1:Description>Karosserie: 4-türig</ns1:Description>
                        <ns1:EquipmentClass>2</ns1:EquipmentClass>
                     </ns1:EquipmentPosition>
                     <ns1:EquipmentPosition>
                        <ns1:DatEquipmentId>75205</ns1:DatEquipmentId>
                        <ns1:Description>Getriebe 6-Gang</ns1:Description>
                        <ns1:EquipmentClass>11</ns1:EquipmentClass>
                     </ns1:EquipmentPosition>
                  </ns1:DATECodeEquipment>
               </ns1:Vehicle>
               <ns1:VAT>
                  <ns1:VatType>difference</ns1:VatType>
                  <ns1:VatAtConstructionTime origin="dat">19</ns1:VatAtConstructionTime>
                  <ns1:VatAtValuationTime origin="dat">19</ns1:VatAtValuationTime>
               </ns1:VAT>
               <ns1:Valuation>
                  <ns1:OriginalPrice origin="dat">27291</ns1:OriginalPrice>
                  <ns1:OriginalPriceGross origin="dat">32476</ns1:OriginalPriceGross>
                  <ns1:BasePrice origin="dat">17999.00</ns1:BasePrice>
                  <ns1:ReferenceMileage>29000</ns1:ReferenceMileage>
                  <ns1:MileageCorr origin="dat">-1252.73</ns1:MileageCorr>
                  <ns1:ResidualValueModel>dat</ns1:ResidualValueModel>
                  <ns1:InitialRegistrationCorr origin="dat">1183.49</ns1:InitialRegistrationCorr>
                  <ns1:BasePrice2 origin="dat">17929.76</ns1:BasePrice2>
                  <ns1:EquipmentSign>calculated value</ns1:EquipmentSign>
                  <ns1:EquipmentOriginalPrice origin="dat">0</ns1:EquipmentOriginalPrice>
                  <ns1:EquipmentPrice origin="dat">0</ns1:EquipmentPrice>
                  <ns1:ValuationCorrection origin="dat">-4944.89</ns1:ValuationCorrection>
                  <ns1:BasePrice3 origin="dat">17929.76</ns1:BasePrice3>
                  <ns1:SalesPrice origin="dat">15097.7600</ns1:SalesPrice>
                  <ns1:SalesPriceGross origin="dat">15452.0000</ns1:SalesPriceGross>
                  <ns1:Margin origin="dat">1864.4200</ns1:Margin>
                  <ns1:MarginGross origin="dat">2218.6637</ns1:MarginGross>
                  <ns1:PurchasePrice origin="dat">13233.3363</ns1:PurchasePrice>
                  <ns1:PurchasePriceGross origin="dat">13233.3363</ns1:PurchasePriceGross>
                  <ns1:LastValuationDataYear>2024</ns1:LastValuationDataYear>
                  <ns1:LastValuationDataMonth>8</ns1:LastValuationDataMonth>
                  <ns1:LastValuationDate>2024-07-25T14:35:50.706+02:00</ns1:LastValuationDate>
                  <ns1:Currency>EUR</ns1:Currency>
                  <ns1:DefaultTiresPrice origin="dat">260.00</ns1:DefaultTiresPrice>
                  <ns1:DeterminatedDate>2018-11-01+01:00</ns1:DeterminatedDate>
                  <ns1:ValuationType>valuation</ns1:ValuationType>
                  <ns1:ExtendedMileageCorrection>true</ns1:ExtendedMileageCorrection>
                  <ns1:Condition>
                     <ns1:OwnerCorrectionPerc origin="user">5</ns1:OwnerCorrectionPerc>
                     <ns1:DatOwnerCorrectionPerc>5.0</ns1:DatOwnerCorrectionPerc>
                     <ns1:OwnerCorrectionAmount>-881.46</ns1:OwnerCorrectionAmount>
                     <ns1:OwnerCorrectionAmountGross>-1048.94</ns1:OwnerCorrectionAmountGross>
                     <ns1:ConditionCorrectionFactorPerc origin="user">90</ns1:ConditionCorrectionFactorPerc>
                     <ns1:DatConditionCorrectionFactorPerc>100</ns1:DatConditionCorrectionFactorPerc>
                     <ns1:ConditionCorrectionAmount>-1762.93</ns1:ConditionCorrectionAmount>
                     <ns1:ConditionCorrectionAmountGross>-2097.89</ns1:ConditionCorrectionAmountGross>
                     <ns1:NumberOfOwners>3</ns1:NumberOfOwners>
                     <ns1:NumberOfOwnersN>3</ns1:NumberOfOwnersN>
                     <ns1:AccidentDamage>accident free</ns1:AccidentDamage>
                     <ns1:IncreaseInValue origin="user">300</ns1:IncreaseInValue>
                     <ns1:IncreaseInValueGross origin="user">357.00</ns1:IncreaseInValueGross>
                     <ns1:DecreaseInValue origin="user">500.50</ns1:DecreaseInValue>
                     <ns1:DecreaseInValueGross origin="user">595.60</ns1:DecreaseInValueGross>
                     <ns1:TiresMountedValue origin="user">-100</ns1:TiresMountedValue>
                     <ns1:TiresMountedValueGross origin="user">-119.00</ns1:TiresMountedValueGross>
                     <ns1:RepairCosts origin="user">2000</ns1:RepairCosts>
                     <ns1:RepairCostsGross origin="user">2380.00</ns1:RepairCostsGross>
                     <ns1:ConditionSubTotal1>17629.26</ns1:ConditionSubTotal1>
                     <ns1:ConditionSubTotal1Gross>20978.82</ns1:ConditionSubTotal1Gross>
                     <ns1:ConditionSubTotal2>14984.87</ns1:ConditionSubTotal2>
                     <ns1:ConditionSubTotal2Gross>17832.00</ns1:ConditionSubTotal2Gross>
                     <ns1:RepairCostsInTradeMargin>false</ns1:RepairCostsInTradeMargin>
                  </ns1:Condition>
                  <ns1:Parameters/>
               </ns1:Valuation>
            </ns1:Dossier>
         </VXS>
      </ns4:getVehicleTargetDateEvaluationHistoryResponse>
   </S:Body>
</S:Envelope>
```
