---
title: "Response resetDossierTechDataN"
topic_id: "25263"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Zurücksetzen von technischen Daten eines Vorgangs auf die DAT-Vorgaben > Response resetDossierTechDataN"
---

# Response resetDossierTechDataN

Eine Beschreibung aller Response-Parameter finden Sie unter [Datenaustauschformat VXS](#showid/1369 "Aktenzeichen/Vorgänge (Dossiers)").

```
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns4:resetDossierTechDataNResponse xmlns:ns4="http://www.dat.de/services/Dossier1N">
         <VXS source="SD3" type="completeEvaluation">
            <ns1:Dossier xmlns:ns1="http://www.dat.de/vxs">
               <ns1:Name>PLVS-1921_NameChange_SUV</ns1:Name>
               <ns1:UUID>e3e2bd9f-69ae-4ed4-a62a-ff9236ef876c</ns1:UUID>
               <ns1:DossierId>66463807</ns1:DossierId>
               <ns1:IdSD3Network>66463807</ns1:IdSD3Network>
               <ns1:Country>DE</ns1:Country>
               <ns1:Language>de_DE</ns1:Language>
               <ns1:DataVersion>1</ns1:DataVersion>
               <ns1:DatCustomerId>XXXX</ns1:DatCustomerId>
               <ns1:DossierType>valuateExpert</ns1:DossierType>
               <ns1:CreateDate>2024-03-26T09:58:22+01:00</ns1:CreateDate>
               <ns1:CreateUser>XXXX</ns1:CreateUser>
               <ns1:ChangeDate>2024-03-26T09:58:32.228+01:00</ns1:ChangeDate>
               <ns1:ChangeUser>XXXX</ns1:ChangeUser>
               <ns1:CDYear>2024</ns1:CDYear>
               <ns1:CDMonth>3</ns1:CDMonth>
               <ns1:DatCustomerAddress>
                  <ns1:Title>titleCompany</ns1:Title>
                  <ns1:CompanyName>DAT Intern</ns1:CompanyName>
                  <ns1:NameLong>XXXX</ns1:NameLong>
                  <ns1:Country>DE</ns1:Country>
                  <ns1:TaxNumber>123</ns1:TaxNumber>
                  <ns1:CustomerNumber>XXXX</ns1:CustomerNumber>
                  <ns1:CustomerType>XXXXX</ns1:CustomerType>
                  <ns1:Street>Hellmuth-Hirth-Str.</ns1:Street>
                  <ns1:StreetNumber>1</ns1:StreetNumber>
                  <ns1:StreetZipCode>73760</ns1:StreetZipCode>
                  <ns1:StreetCity>Ostfildern</ns1:StreetCity>
                  <ns1:Bank>Test bank</ns1:Bank>
                  <ns1:BIC>0</ns1:BIC>
                  <ns1:BLZ>NA</ns1:BLZ>
                  <ns1:AccountNo>NA</ns1:AccountNo>
                  <ns1:IBAN>0</ns1:IBAN>
                  <ns1:UsageFlag>9</ns1:UsageFlag>
               </ns1:DatCustomerAddress>
               <ns1:Vehicle>
                  <ns1:DatECode>010601450010001</ns1:DatECode>
                  <ns1:Container>DE001</ns1:Container>
                  <ns1:ConstructionYear origin="dat">986</ns1:ConstructionYear>
                  <ns1:ConstructionTime>5310</ns1:ConstructionTime>
                  <ns1:InitialRegistration>2014-01-16+01:00</ns1:InitialRegistration>
                  <ns1:MileageEstimated>45789</ns1:MileageEstimated>
                  <ns1:MileageType>Estimated</ns1:MileageType>
                  <ns1:SalesDescription>S1 2.0 TFSI quattro</ns1:SalesDescription>
                  <ns1:VehicleTypeNameN origin="dat">Pkw, SUV, Kleintransporter</ns1:VehicleTypeNameN>
                  <ns1:ManufacturerName origin="dat">Audi</ns1:ManufacturerName>
                  <ns1:BaseModelName origin="dat">S1 (8XK)(2014->)</ns1:BaseModelName>
                  <ns1:SubModelName origin="dat">2.0 TFSI quattro</ns1:SubModelName>
                  <ns1:ContainerNameN origin="dat">DE - LimS3 2.0 TFSI quattro EU6, quattro, 2014 - 2018</ns1:ContainerNameN>
                  <ns1:VehicleType>1</ns1:VehicleType>
                  <ns1:Manufacturer>60</ns1:Manufacturer>
                  <ns1:BaseModel>145</ns1:BaseModel>
                  <ns1:SubModel>1</ns1:SubModel>
                  <ns1:Country>DE</ns1:Country>
                  <ns1:VinActive>false</ns1:VinActive>
                  <ns1:VinEquipmentChanged>false</ns1:VinEquipmentChanged>
                  <ns1:ReleaseIndicator>APPRAISAL</ns1:ReleaseIndicator>
                  <ns1:SubModelVariant>1</ns1:SubModelVariant>
                  <ns1:RegistrationData>
                     <ns1:LicenseNumber>S DAT 123</ns1:LicenseNumber>
                  </ns1:RegistrationData>
                  <ns1:Engine>
                     <ns1:FuelMethod origin="dat">gasoline</ns1:FuelMethod>
                     <ns1:EnginePowerKw origin="dat">170</ns1:EnginePowerKw>
                     <ns1:EnginePowerHp origin="dat">231</ns1:EnginePowerHp>
                     <ns1:Cylinders origin="dat">4</ns1:Cylinders>
                     <ns1:Capacity origin="dat">1984</ns1:Capacity>
                     <ns1:Consumption>7.1</ns1:Consumption>
                     <ns1:Co2Emission>166.0</ns1:Co2Emission>
                  </ns1:Engine>
                  <ns1:TechInfo>
                     <ns1:StructureType>LimHb</ns1:StructureType>
                     <ns1:StructureDescription>Lim. Schrägheck</ns1:StructureDescription>
                     <ns1:CountOfAxles origin="dat">2</ns1:CountOfAxles>
                     <ns1:CountOfDrivedAxles origin="dat">2</ns1:CountOfDrivedAxles>
                     <ns1:WheelBase origin="dat">2469</ns1:WheelBase>
                     <ns1:Length origin="dat">3975</ns1:Length>
                     <ns1:Width origin="dat">1740</ns1:Width>
                     <ns1:Height origin="dat">1417</ns1:Height>
                     <ns1:VehicleSeats origin="dat">4</ns1:VehicleSeats>
                     <ns1:VehicleDoors origin="dat">3</ns1:VehicleDoors>
                     <ns1:CountOfAirbags origin="dat">4</ns1:CountOfAirbags>
                     <ns1:Acceleration origin="dat">5.8</ns1:Acceleration>
                     <ns1:SpeedMax origin="dat">250</ns1:SpeedMax>
                     <ns1:PowerHp origin="dat">231</ns1:PowerHp>
                     <ns1:PowerKw origin="dat">170</ns1:PowerKw>
                     <ns1:Capacity origin="dat">1984</ns1:Capacity>
                     <ns1:Cylinder origin="dat">4</ns1:Cylinder>
                     <ns1:CylinderArrangement origin="dat">R</ns1:CylinderArrangement>
                     <ns1:RotationsOnMaxPower origin="dat">6000</ns1:RotationsOnMaxPower>
                     <ns1:RotationsOnMaxTorque origin="dat">1600</ns1:RotationsOnMaxTorque>
                     <ns1:Torque origin="dat">370</ns1:Torque>
                     <ns1:GearboxType>manual</ns1:GearboxType>
                     <ns1:NrOfGears>6</ns1:NrOfGears>
                     <ns1:OriginalTireSizeAxle1>215/40R17</ns1:OriginalTireSizeAxle1>
                     <ns1:OriginalTireSizeAxle2>215/40R17</ns1:OriginalTireSizeAxle2>
                     <ns1:TankVolume origin="dat">45</ns1:TankVolume>
                     <ns1:ConsumptionInTown origin="dat">9.2</ns1:ConsumptionInTown>
                     <ns1:ConsumptionOutOfTown origin="dat">5.9</ns1:ConsumptionOutOfTown>
                     <ns1:Consumption origin="dat">7.1</ns1:Consumption>
                     <ns1:Co2Emission origin="dat">166</ns1:Co2Emission>
                     <ns1:EmissionClassN>
                        <ns1:EmissionClassItemN description="EU6" type="EU"/>
                     </ns1:EmissionClassN>
                     <ns1:DriveN origin="dat">Allradantrieb</ns1:DriveN>
                     <ns1:DriveCode>A</ns1:DriveCode>
                     <ns1:EngineCycle origin="dat">4</ns1:EngineCycle>
                     <ns1:FuelMethod origin="dat">Superbenzin</ns1:FuelMethod>
                     <ns1:FuelMethodCode>BS</ns1:FuelMethodCode>
                     <ns1:FuelMethodType origin="dat">B</ns1:FuelMethodType>
                     <ns1:UnloadedWeight origin="dat">1390</ns1:UnloadedWeight>
                     <ns1:PermissableTotalWeight origin="dat">1765</ns1:PermissableTotalWeight>
                     <ns1:Payload origin="dat">375</ns1:Payload>
                     <ns1:LoadingSpace origin="dat">210</ns1:LoadingSpace>
                     <ns1:LoadingSpaceMax origin="dat">860</ns1:LoadingSpaceMax>
                     <ns1:InsuranceTypeClassLiability>15</ns1:InsuranceTypeClassLiability>
                     <ns1:InsuranceTypeClassCascoPartial>23</ns1:InsuranceTypeClassCascoPartial>
                     <ns1:InsuranceTypeClassCascoComplete>20</ns1:InsuranceTypeClassCascoComplete>
                     <ns1:ProductGroupName>Kleinwagen</ns1:ProductGroupName>
                     <ns1:SuitableForE10 origin="dat">true</ns1:SuitableForE10>
                     <ns1:WidthForGarage origin="dat">1906</ns1:WidthForGarage>
                     <ns1:EnergyEfficiencyClass origin="dat">E</ns1:EnergyEfficiencyClass>
                     <ns1:TechInfoWltp/>
                 </ns1:TechInfo>
                  <ns1:Equipment>
                     <ns1:EquipmentValue origin="dat">0</ns1:EquipmentValue>
                     <ns1:EquipmentValueGross origin="dat">0.00</ns1:EquipmentValueGross>
                     <ns1:OriginalEquipmentValue origin="dat">0</ns1:OriginalEquipmentValue>
                     <ns1:OriginalEquipmentValueGross origin="dat">0.0</ns1:OriginalEquipmentValueGross>
                     <ns1:EquipmentValueType>calculated value</ns1:EquipmentValueType>
                     <ns1:SeriesEquipment>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>3915</ns1:DatEquipmentId>
                           <ns1:Description>Innenlicht-Paket LED</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>13133</ns1:DatEquipmentId>
                           <ns1:Description>Einstiegsleisten mit Aluminiumeinlage und Schriftzug</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>15106</ns1:DatEquipmentId>
                           <ns1:Description>Außenspiegel elektr. verstellbar</ns1:Description>
                           <ns1:EquipmentGroup>AUSP</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>15700</ns1:DatEquipmentId>
                           <ns1:Description>Außenspiegel asphärisch, rechts</ns1:Description>
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
                           <ns1:DatEquipmentId>15902</ns1:DatEquipmentId>
                           <ns1:Description>Außenspiegel Aluminium / Chromfarben</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18211</ns1:DatEquipmentId>
                           <ns1:Description>Blinkleuchten LED in Außenspiegel integriert</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18505</ns1:DatEquipmentId>
                           <ns1:Description>Xenon-Scheinwerfer Plus (Abblend- und Fernlicht)</ns1:Description>
                           <ns1:EquipmentGroup>XELI</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18625</ns1:DatEquipmentId>
                           <ns1:Description>Lichtsensor (Coming Home, Leaving Home)</ns1:Description>
                           <ns1:EquipmentGroup>FA32</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18700</ns1:DatEquipmentId>
                           <ns1:Description>Nebelschlussleuchte</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18802</ns1:DatEquipmentId>
                           <ns1:Description>Heckleuchten LED</ns1:Description>
                           <ns1:EquipmentGroup>LEDH</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18899</ns1:DatEquipmentId>
                           <ns1:Description>Adaptives Bremslicht</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18909</ns1:DatEquipmentId>
                           <ns1:Description>Licht- und Regensensor</ns1:Description>
                           <ns1:EquipmentGroup>SWRE</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>20935</ns1:DatEquipmentId>
                           <ns1:Description>Dachkantenspoiler S-line</ns1:Description>
                           <ns1:EquipmentGroup>SPOI</ns1:EquipmentGroup>
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
                           <ns1:DatEquipmentId>22506</ns1:DatEquipmentId>
                           <ns1:Description>Frontscheibe mit Bandfilter oben</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>22800</ns1:DatEquipmentId>
                           <ns1:Description>Heckscheibe heizbar</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>24110</ns1:DatEquipmentId>
                           <ns1:Description>Audiosystem chorus (Radio/CD-Player)</ns1:Description>
                           <ns1:EquipmentGroup>CD</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25805</ns1:DatEquipmentId>
                           <ns1:Description>Fahrer-Informations-System (FIS)</ns1:Description>
                           <ns1:EquipmentGroup>COMP</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25903</ns1:DatEquipmentId>
                           <ns1:Description>Reifendruck-Kontrollsystem</ns1:Description>
                           <ns1:EquipmentGroup>RDK</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26129</ns1:DatEquipmentId>
                           <ns1:Description>Innenausstattung: Ausströmer Hochglanz</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26604</ns1:DatEquipmentId>
                           <ns1:Description>Pedalkappen-Set Edelstahl</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26803</ns1:DatEquipmentId>
                           <ns1:Description>Airbag Fahrer-/Beifahrerseite</ns1:Description>
                           <ns1:EquipmentGroup>AIR1</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>26801</ns1:DatEquipmentId>
                                 <ns1:Description>Airbag Fahrerseite</ns1:Description>
                                 <ns1:EquipmentGroup>AIR</ns1:EquipmentGroup>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>26802</ns1:DatEquipmentId>
                                 <ns1:Description>Airbag Beifahrerseite</ns1:Description>
                                 <ns1:EquipmentGroup>AIR1</ns1:EquipmentGroup>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26901</ns1:DatEquipmentId>
                           <ns1:Description>Kopf-Airbag-System (Sideguard)</ns1:Description>
                           <ns1:EquipmentGroup>AIR4</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26903</ns1:DatEquipmentId>
                           <ns1:Description>Seitenairbag vorn</ns1:Description>
                           <ns1:EquipmentGroup>AIR3</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27805</ns1:DatEquipmentId>
                           <ns1:Description>Dachhimmel Stoff, schwarz</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>28409</ns1:DatEquipmentId>
                           <ns1:Description>Fußmatten Velours</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>28901</ns1:DatEquipmentId>
                           <ns1:Description>Klimaautomatik</ns1:Description>
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
                           <ns1:DatEquipmentId>29700</ns1:DatEquipmentId>
                           <ns1:Description>Einstiegshilfe Easy-Entry</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>30109</ns1:DatEquipmentId>
                           <ns1:Description>Sitzbezug / Polsterung: Stoff / Leder</ns1:Description>
                           <ns1:EquipmentGroup>LED1</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>31007</ns1:DatEquipmentId>
                           <ns1:Description>Innenausstattung: Aluminium-Optik</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>31221</ns1:DatEquipmentId>
                           <ns1:Description>Innenausstattung: farbig - erweiterte Ausstattung mono.pur</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>31901</ns1:DatEquipmentId>
                           <ns1:Description>Sportsitze vorn</ns1:Description>
                           <ns1:EquipmentGroup>SPSI</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>32704</ns1:DatEquipmentId>
                           <ns1:Description>Sitz vorn links höhenverstellbar</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>32705</ns1:DatEquipmentId>
                           <ns1:Description>Sitz vorn rechts höhenverstellbar</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>32706</ns1:DatEquipmentId>
                           <ns1:Description>Sitze vorn höhenverstellbar</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>33305</ns1:DatEquipmentId>
                           <ns1:Description>Lendenwirbelstützen vorn</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>33309</ns1:DatEquipmentId>
                           <ns1:Description>Lendenwirbelstützen verstellbar</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>33508</ns1:DatEquipmentId>
                           <ns1:Description>Rücksitzlehne geteilt/klappbar</ns1:Description>
                           <ns1:EquipmentGroup>SITH</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>34805</ns1:DatEquipmentId>
                           <ns1:Description>Kopfstützen hinten</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35000</ns1:DatEquipmentId>
                           <ns1:Description>Fensterheber elektrisch</ns1:Description>
                           <ns1:EquipmentGroup>FH2</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35301</ns1:DatEquipmentId>
                           <ns1:Description>Zentralverriegelung mit Fernbedienung</ns1:Description>
                           <ns1:EquipmentGroup>ZV</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>37603</ns1:DatEquipmentId>
                           <ns1:Description>Ambiente-Beleuchtung</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>37704</ns1:DatEquipmentId>
                           <ns1:Description>Make-up-Spiegel beleuchtet</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>37722</ns1:DatEquipmentId>
                           <ns1:Description>Leseleuchten im Fond zusätzlich</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>37901</ns1:DatEquipmentId>
                           <ns1:Description>Innenspiegel mit Abblendautomatik</ns1:Description>
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
                           <ns1:DatEquipmentId>38906</ns1:DatEquipmentId>
                           <ns1:Description>Getränkehalter in Mittelkonsole</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39010</ns1:DatEquipmentId>
                           <ns1:Description>Steckdose (12V-Anschluß) in Mittelkonsole vorn</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39205</ns1:DatEquipmentId>
                           <ns1:Description>Schalt-/Wählhebelgriff Leder</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39307</ns1:DatEquipmentId>
                           <ns1:Description>Isofix-Aufnahmen für Kindersitz</ns1:Description>
                           <ns1:EquipmentGroup>KISI</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40000</ns1:DatEquipmentId>
                           <ns1:Description>Anti-Blockier-System (ABS)</ns1:Description>
                           <ns1:EquipmentGroup>ABS</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40320</ns1:DatEquipmentId>
                           <ns1:Description>Bremsanlage mit Rekuperationssystem</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40595</ns1:DatEquipmentId>
                           <ns1:Description>Bremssättel lackiert, Farbe nach Wahl</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40799</ns1:DatEquipmentId>
                           <ns1:Description>Bremsassistent</ns1:Description>
                           <ns1:EquipmentGroup>FA01</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40801</ns1:DatEquipmentId>
                           <ns1:Description>Fahrassistenz-System: Bremsassistent (Audi pre sense front)</ns1:Description>
                           <ns1:EquipmentGroup>FA01</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>41909</ns1:DatEquipmentId>
                           <ns1:Description>Sport-Fahrwerk S / RS spezifisch</ns1:Description>
                           <ns1:EquipmentGroup>SPFW</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>42613</ns1:DatEquipmentId>
                           <ns1:Description>Audi Drive Select</ns1:Description>
                           <ns1:EquipmentGroup>FARS</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>48300</ns1:DatEquipmentId>
                           <ns1:Description>LM-Felgen</ns1:Description>
                           <ns1:EquipmentGroup>ALU</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>68802</ns1:DatEquipmentId>
                           <ns1:Description>Reifen-Reparaturkit</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>69300</ns1:DatEquipmentId>
                           <ns1:Description>Lenkrad (Sport/Leder - 3-Speichen)</ns1:Description>
                           <ns1:EquipmentGroup>LEN6</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>69800</ns1:DatEquipmentId>
                           <ns1:Description>Servolenkung</ns1:Description>
                           <ns1:EquipmentGroup>SL</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>70101</ns1:DatEquipmentId>
                           <ns1:Description>Elektron. Stabilitätskontrolle (ESC)</ns1:Description>
                           <ns1:EquipmentGroup>ESP</ns1:EquipmentGroup>
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
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>70420</ns1:DatEquipmentId>
                           <ns1:Description>Antriebsart: Allradantrieb</ns1:Description>
                           <ns1:EquipmentGroup>4WD</ns1:EquipmentGroup>
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
                           <ns1:DatEquipmentId>10002</ns1:DatEquipmentId>
                           <ns1:Description>Karosserie: 2-türig</ns1:Description>
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
                           <ns1:DatEquipmentId>96618</ns1:DatEquipmentId>
                           <ns1:Description>Motor 2,0 Ltr. - 170 kW 16V TFSI</ns1:Description>
                           <ns1:EquipmentType>engine</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                     </ns1:SeriesEquipment>
                  </ns1:Equipment>
                  <ns1:Tires>
                     <ns1:Axles>
                        <ns1:Axle>
                           <ns1:AxleNo>1</ns1:AxleNo>
                           <ns1:TireId>10002232</ns1:TireId>
                           <ns1:TireState>mounted</ns1:TireState>
                           <ns1:NrOfTires>2</ns1:NrOfTires>
                           <ns1:TireOriginalPrice origin="dat">127</ns1:TireOriginalPrice>
                           <ns1:TireSpeedIndex></ns1:TireSpeedIndex>
                           <ns1:TireSize>215/40R17</ns1:TireSize>
                           <ns1:TireSafetySystem></ns1:TireSafetySystem>
                           <ns1:TireOriginalTreadDepth>8</ns1:TireOriginalTreadDepth>
                           <ns1:TireLoadCapacityIndex>0</ns1:TireLoadCapacityIndex>
                           <ns1:TreadDepthLeftOuterPerc>50</ns1:TreadDepthLeftOuterPerc>
                           <ns1:TreadDepthRightOuterPerc>50</ns1:TreadDepthRightOuterPerc>
                           <ns1:TreadDepthLeftOuterMm>5</ns1:TreadDepthLeftOuterMm>
                           <ns1:TreadDepthRightOuterMm>5</ns1:TreadDepthRightOuterMm>
                           <ns1:ManualEntry>false</ns1:ManualEntry>
                        </ns1:Axle>
                        <ns1:Axle>
                           <ns1:AxleNo>2</ns1:AxleNo>
                           <ns1:TireId>10002232</ns1:TireId>
                           <ns1:TireState>mounted</ns1:TireState>
                           <ns1:NrOfTires>2</ns1:NrOfTires>
                           <ns1:TireOriginalPrice origin="dat">127</ns1:TireOriginalPrice>
                           <ns1:TireSpeedIndex></ns1:TireSpeedIndex>
                           <ns1:TireSize>215/40R17</ns1:TireSize>
                           <ns1:TireSafetySystem></ns1:TireSafetySystem>
                           <ns1:TireOriginalTreadDepth>8</ns1:TireOriginalTreadDepth>
                           <ns1:TireLoadCapacityIndex>0</ns1:TireLoadCapacityIndex>
                           <ns1:TreadDepthLeftOuterPerc>50</ns1:TreadDepthLeftOuterPerc>
                           <ns1:TreadDepthRightOuterPerc>50</ns1:TreadDepthRightOuterPerc>
                           <ns1:TreadDepthLeftOuterMm>5</ns1:TreadDepthLeftOuterMm>
                           <ns1:TreadDepthRightOuterMm>5</ns1:TreadDepthRightOuterMm>
                           <ns1:ManualEntry>false</ns1:ManualEntry>
                        </ns1:Axle>
                     </ns1:Axles>
                  </ns1:Tires>
                  <ns1:DATECodeEquipment>
                     <ns1:EquipmentPosition>
                        <ns1:DatEquipmentId>96618</ns1:DatEquipmentId>
                        <ns1:Description>Motor 2,0 Ltr. - 170 kW 16V TFSI</ns1:Description>
                        <ns1:EquipmentClass>1</ns1:EquipmentClass>
                     </ns1:EquipmentPosition>
                     <ns1:EquipmentPosition>
                        <ns1:DatEquipmentId>10002</ns1:DatEquipmentId>
                        <ns1:Description>Karosserie: 2-türig</ns1:Description>
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
                  <ns1:BaseVatAtConstructionTime origin="dat">19</ns1:BaseVatAtConstructionTime>
                  <ns1:AddOnTaxApplication>before vat</ns1:AddOnTaxApplication>
                  <ns1:VatAtValuationTime origin="dat">19</ns1:VatAtValuationTime>
               </ns1:VAT>
               <ns1:TradingData>
                  <ns1:AddonList>
                     <ns1:Addon name="LabellingPrice"/>
                     <ns1:Addon name="LabellingPriceGross"/>
                     <ns1:Addon name="ResellerPrice"/>
                     <ns1:Addon name="ResellerPriceGross"/>
                     <ns1:Addon name="SPMinimum"/>
                     <ns1:Addon name="SPMinimumGross"/>
                     <ns1:Addon name="DEVIATING_MARKETPLACE_PRICE">false</ns1:Addon>
                     <ns1:Addon name="MarketPriceLabelling"/>
                     <ns1:Addon name="MarketPriceLabellingGross"/>
                  </ns1:AddonList>
               </ns1:TradingData>
               <ns1:Valuation>
                  <ns1:OriginalPrice origin="dat">25168</ns1:OriginalPrice>
                  <ns1:OriginalPriceGross origin="dat">29950</ns1:OriginalPriceGross>
                  <ns1:BasePrice origin="dat">10594.00</ns1:BasePrice>
                  <ns1:ReferenceMileage>106000</ns1:ReferenceMileage>
                  <ns1:MileageCorr origin="user">1234</ns1:MileageCorr>
                  <ns1:DatMileageCorr>1660.07</ns1:DatMileageCorr>
                  <ns1:ResidualValueModel>dat</ns1:ResidualValueModel>
                  <ns1:InitialRegistrationCorr origin="user">345</ns1:InitialRegistrationCorr>
                  <ns1:DatInitialRegistrationCorr>-245.08</ns1:DatInitialRegistrationCorr>
                  <ns1:BasePrice2 origin="dat">12173.00</ns1:BasePrice2>
                  <ns1:EquipmentSign>calculated value</ns1:EquipmentSign>
                  <ns1:EquipmentOriginalPrice origin="dat">0</ns1:EquipmentOriginalPrice>
                  <ns1:EquipmentPrice origin="dat">0</ns1:EquipmentPrice>
                  <ns1:ValuationCorrection origin="dat">-1825.95</ns1:ValuationCorrection>
                  <ns1:BasePrice3 origin="dat">12173.00</ns1:BasePrice3>
                  <ns1:ConditionCorrectionPerc origin="dat">85.00</ns1:ConditionCorrectionPerc>
                  <ns1:SalesPrice origin="dat">12025.22</ns1:SalesPrice>
                  <ns1:SalesPriceRounded origin="dat">12025</ns1:SalesPriceRounded>
                  <ns1:SalesPriceGross origin="dat">12312.99</ns1:SalesPriceGross>
                  <ns1:SalesPriceGrossRounded origin="dat">12325</ns1:SalesPriceGrossRounded>
                  <ns1:Margin origin="dat">1514.58</ns1:Margin>
                  <ns1:MarginRounded origin="dat">1525</ns1:MarginRounded>
                  <ns1:MarginGross origin="dat">1802.34</ns1:MarginGross>
                  <ns1:MarginGrossRounded origin="dat">1800</ns1:MarginGrossRounded>
                  <ns1:PurchasePrice origin="dat">10510.65</ns1:PurchasePrice>
                  <ns1:PurchasePriceRounded origin="dat">10500</ns1:PurchasePriceRounded>
                  <ns1:PurchasePriceGross origin="dat">10510.65</ns1:PurchasePriceGross>
                  <ns1:PurchasePriceGrossRounded origin="dat">10525</ns1:PurchasePriceGrossRounded>
                  <ns1:LastValuationDataYear>2024</ns1:LastValuationDataYear>
                  <ns1:LastValuationDataMonth>3</ns1:LastValuationDataMonth>
                  <ns1:LastValuationDate>2024-03-26T09:58:32.187+01:00</ns1:LastValuationDate>
                  <ns1:Currency>EUR</ns1:Currency>
                  <ns1:SignMilageUnit>kilometers</ns1:SignMilageUnit>
                  <ns1:Obsolete>up to date</ns1:Obsolete>
                  <ns1:DisplayGross>true</ns1:DisplayGross>
                  <ns1:DisplayRounded>true</ns1:DisplayRounded>
                  <ns1:DefaultTiresPrice origin="dat">254.00</ns1:DefaultTiresPrice>
                  <ns1:SignDeterminatedDate>true</ns1:SignDeterminatedDate>
                  <ns1:DeterminatedDate>2024-03-26+01:00</ns1:DeterminatedDate>
                  <ns1:ValuationType>valuation</ns1:ValuationType>
                  <ns1:ExtendedMileageCorrection>true</ns1:ExtendedMileageCorrection>
                  <ns1:Condition>
                     <ns1:OwnerCorrectionPerc origin="user">15</ns1:OwnerCorrectionPerc>
                     <ns1:DatOwnerCorrectionPerc>5</ns1:DatOwnerCorrectionPerc>
                     <ns1:OwnerCorrectionAmount>-1825.95</ns1:OwnerCorrectionAmount>
                     <ns1:OwnerCorrectionAmountGross>-2172.88</ns1:OwnerCorrectionAmountGross>
                     <ns1:ConditionCorrectionFactorPerc origin="dat">100</ns1:ConditionCorrectionFactorPerc>
                     <ns1:ConditionCorrectionAmount>0.00</ns1:ConditionCorrectionAmount>
                     <ns1:ConditionCorrectionAmountGross>0.00</ns1:ConditionCorrectionAmountGross>
                     <ns1:NumberOfOwnersN>3</ns1:NumberOfOwnersN>
                     <ns1:ConditionSubTotal1>12173.00</ns1:ConditionSubTotal1>
                     <ns1:ConditionSubTotal1Gross>14485.87</ns1:ConditionSubTotal1Gross>
                     <ns1:ConditionSubTotal2>10347.05</ns1:ConditionSubTotal2>
                     <ns1:ConditionSubTotal2Gross>12312.99</ns1:ConditionSubTotal2Gross>
                     <ns1:RepairCostsInTradeMargin>false</ns1:RepairCostsInTradeMargin>
                  </ns1:Condition>
                  <ns1:Parameters/>
               </ns1:Valuation>
            </ns1:Dossier>
         </VXS>
      </ns4:resetDossierTechDataNResponse>
   </S:Body>
</S:Envelope>
```
