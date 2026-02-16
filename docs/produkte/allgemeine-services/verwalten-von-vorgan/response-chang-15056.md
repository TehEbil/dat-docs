---
title: "Response changeDossierN"
topic_id: "15056"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Aendern eines Vorgangs > Response changeDossierN"
---

# Response changeDossierN

Eine Beschreibung aller Response-Parameter finden Sie unter [Datenaustauschformat VXS](../../../vxs/aktenzeichenvorgange-doss/index.md).

```
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns4:changeDossierNResponse xmlns:ns4="http://www.dat.de/services/Dossier1N">
         <VXS source="SD3" type="completeEvaluation">
            <ns1:Dossier xmlns:ns1="http://www.dat.de/vxs">
               <ns1:Name>name change</ns1:Name>
               <ns1:UUID>9bf37207-5210-4eeb-b155-e09959c651f8</ns1:UUID>
               <ns1:DossierId>2539149</ns1:DossierId>
               <ns1:IdSD3Network>2539149</ns1:IdSD3Network>
               <ns1:Country>DE</ns1:Country>
               <ns1:Language>de_DE</ns1:Language>
               <ns1:DataVersion>1</ns1:DataVersion>
               <ns1:DatCustomerId>XXXXXXX</ns1:DatCustomerId>
               <ns1:DossierType>valuateExpert</ns1:DossierType>
               <ns1:CreateDate>2024-12-19T08:50:19+01:00</ns1:CreateDate>
               <ns1:CreateUser>XXX</ns1:CreateUser>
               <ns1:ChangeDate>2024-12-19T08:50:19.758+01:00</ns1:ChangeDate>
               <ns1:ChangeUser>XXX</ns1:ChangeUser>
               <ns1:CDYear>2025</ns1:CDYear>
               <ns1:CDMonth>1</ns1:CDMonth>
               <ns1:ProcedureType>EVALUATION</ns1:ProcedureType>
               <ns1:DatCustomerAddress>
                  <ns1:Title>titleCompany</ns1:Title>
                  <ns1:CompanyName>DAT Intern</ns1:CompanyName>
                  <ns1:Country>DE</ns1:Country>
                  <ns1:TaxNumber>123</ns1:TaxNumber>
                  <ns1:CustomerNumber>XXXXXXX</ns1:CustomerNumber>
                  <ns1:Street>Hellmuth-Hirth-Str.</ns1:Street>
                  <ns1:StreetNumber>1</ns1:StreetNumber>
                  <ns1:StreetZipCode>73760</ns1:StreetZipCode>
                  <ns1:StreetCity>Ostfildern</ns1:StreetCity>
                  <ns1:Bank>Test bank</ns1:Bank>
                  <ns1:BLZ>NA</ns1:BLZ>
                  <ns1:AccountNo>NA</ns1:AccountNo>
                  <ns1:UsageFlag>9</ns1:UsageFlag>
               </ns1:DatCustomerAddress>
               <ns1:Vehicle>
                  <ns1:DatECode>010400850080003</ns1:DatECode>
                  <ns1:Container>DE003</ns1:Container>
                  <ns1:ConstructionYear origin="dat">986</ns1:ConstructionYear>
                  <ns1:ConstructionTime>5410</ns1:ConstructionTime>
                  <ns1:InitialRegistration>2014-06-01+02:00</ns1:InitialRegistration>
                  <ns1:MileageEstimated>50000</ns1:MileageEstimated>
                  <ns1:MileageType>Estimated</ns1:MileageType>
                  <ns1:SalesDescription>Giulietta 1,6 JTDM 16V Turismo</ns1:SalesDescription>
                  <ns1:VehicleTypeNameN origin="dat">Pkw, SUV, Kleintransporter</ns1:VehicleTypeNameN>
                  <ns1:ManufacturerName origin="dat">Alfa Romeo</ns1:ManufacturerName>
                  <ns1:BaseModelName origin="dat">Giulietta (191)(2010->)</ns1:BaseModelName>
                  <ns1:SubModelName origin="dat">Turismo</ns1:SubModelName>
                  <ns1:ContainerNameN origin="dat">DE - LimS5 1.6 JTDM 16V EU5, Turismo, 2010 - 2015</ns1:ContainerNameN>
                  <ns1:VehicleType>1</ns1:VehicleType>
                  <ns1:Manufacturer>40</ns1:Manufacturer>
                  <ns1:BaseModel>85</ns1:BaseModel>
                  <ns1:SubModel>8</ns1:SubModel>
                  <ns1:Country>DE</ns1:Country>
                  <ns1:VinEquipmentChanged>false</ns1:VinEquipmentChanged>
                  <ns1:ReleaseIndicator>APPRAISAL</ns1:ReleaseIndicator>
                  <ns1:SubModelVariant>3</ns1:SubModelVariant>
                  <ns1:RegistrationData/>
                  <ns1:Engine>
                     <ns1:FuelMethod origin="dat">diesel</ns1:FuelMethod>
                     <ns1:EnginePowerKw origin="dat">77</ns1:EnginePowerKw>
                     <ns1:EnginePowerHp origin="dat">104</ns1:EnginePowerHp>
                     <ns1:Cylinders origin="dat">4</ns1:Cylinders>
                     <ns1:Capacity origin="dat">1598</ns1:Capacity>
                     <ns1:Consumption>4.4</ns1:Consumption>
                     <ns1:Co2Emission>117.0</ns1:Co2Emission>
                  </ns1:Engine>
                  <ns1:TechInfo>
                     <ns1:StructureType>LimHb</ns1:StructureType>
                     <ns1:StructureDescription origin="dat">Lim. Schrägheck</ns1:StructureDescription>
                     <ns1:CountOfAxles origin="dat">2</ns1:CountOfAxles>
                     <ns1:CountOfDrivedAxles origin="dat">1</ns1:CountOfDrivedAxles>
                     <ns1:WheelBase origin="dat">2634</ns1:WheelBase>
                     <ns1:Length origin="dat">4351</ns1:Length>
                     <ns1:Width origin="dat">1798</ns1:Width>
                     <ns1:Height origin="dat">1465</ns1:Height>
                     <ns1:RoofLoad origin="dat">50</ns1:RoofLoad>
                     <ns1:TrailerLoadBraked origin="dat">1300</ns1:TrailerLoadBraked>
                     <ns1:TrailerLoadUnbraked origin="dat">500</ns1:TrailerLoadUnbraked>
                     <ns1:VehicleSeats origin="dat">5</ns1:VehicleSeats>
                     <ns1:VehicleDoors origin="dat">5</ns1:VehicleDoors>
                     <ns1:Acceleration origin="dat">11.3</ns1:Acceleration>
                     <ns1:SpeedMax origin="dat">185</ns1:SpeedMax>
                     <ns1:PowerHp origin="dat">105</ns1:PowerHp>
                     <ns1:PowerKw origin="dat">77</ns1:PowerKw>
                     <ns1:Capacity origin="dat">1598</ns1:Capacity>
                     <ns1:Cylinder origin="dat">4</ns1:Cylinder>
                     <ns1:CylinderArrangement origin="dat">R</ns1:CylinderArrangement>
                     <ns1:RotationsOnMaxPower origin="dat">5000</ns1:RotationsOnMaxPower>
                     <ns1:RotationsOnMaxTorque origin="dat">1500</ns1:RotationsOnMaxTorque>
                     <ns1:Torque origin="dat">280</ns1:Torque>
                     <ns1:GearboxType>manual</ns1:GearboxType>
                     <ns1:NrOfGears>6</ns1:NrOfGears>
                     <ns1:OriginalTireSizeAxle1>205/55R16</ns1:OriginalTireSizeAxle1>
                     <ns1:OriginalTireSizeAxle2>205/55R16</ns1:OriginalTireSizeAxle2>
                     <ns1:TankVolume origin="dat">60</ns1:TankVolume>
                     <ns1:ConsumptionInTown origin="dat">5.5</ns1:ConsumptionInTown>
                     <ns1:ConsumptionOutOfTown origin="dat">3.7</ns1:ConsumptionOutOfTown>
                     <ns1:Consumption origin="dat">4.4</ns1:Consumption>
                     <ns1:Co2Emission origin="dat">117</ns1:Co2Emission>
                     <ns1:EmissionClassN>
                        <ns1:EmissionClassItemN description="E5" type="EU"/>
                     </ns1:EmissionClassN>
                     <ns1:DriveN origin="dat">Frontantrieb</ns1:DriveN>
                     <ns1:DriveCode>FA</ns1:DriveCode>
                     <ns1:EngineCycle origin="dat">4</ns1:EngineCycle>
                     <ns1:FuelMethod origin="dat">Diesel</ns1:FuelMethod>
                     <ns1:FuelMethodCode>D</ns1:FuelMethodCode>
                     <ns1:FuelMethodType origin="dat">D</ns1:FuelMethodType>
                     <ns1:UnloadedWeight origin="dat">1385</ns1:UnloadedWeight>
                     <ns1:PermissableTotalWeight origin="dat">1815</ns1:PermissableTotalWeight>
                     <ns1:Payload origin="dat">430</ns1:Payload>
                     <ns1:LoadingSpace origin="dat">350</ns1:LoadingSpace>
                     <ns1:LoadingSpaceMax origin="dat">1150</ns1:LoadingSpaceMax>
                     <ns1:InsuranceTypeClassLiability>19</ns1:InsuranceTypeClassLiability>
                     <ns1:InsuranceTypeClassCascoPartial>20</ns1:InsuranceTypeClassCascoPartial>
                     <ns1:InsuranceTypeClassCascoComplete>17</ns1:InsuranceTypeClassCascoComplete>
                     <ns1:ProductGroupName>untere Mittelklasse / Kompaktklasse</ns1:ProductGroupName>
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
                           <ns1:DatEquipmentId>11108</ns1:DatEquipmentId>
                           <ns1:Description>Pastell-Lackierung</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>13781</ns1:DatEquipmentId>
                           <ns1:Description>Rahmen Frontscheinwerfer und Heckleuchten Chrom, mattiert</ns1:Description>
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
                           <ns1:DatEquipmentId>15807</ns1:DatEquipmentId>
                           <ns1:Description>Außenspiegel Wagenfarbe</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18300</ns1:DatEquipmentId>
                           <ns1:Description>Nebelscheinwerfer</ns1:Description>
                           <ns1:EquipmentGroup>BEL</ns1:EquipmentGroup>
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
                           <ns1:DatEquipmentId>18913</ns1:DatEquipmentId>
                           <ns1:Description>Tagfahrlicht LED</ns1:Description>
                           <ns1:EquipmentGroup>TFAL</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>19300</ns1:DatEquipmentId>
                           <ns1:Description>Heckscheibenwischer</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>20606</ns1:DatEquipmentId>
                           <ns1:Description>Heckspoiler Wagenfarbe</ns1:Description>
                           <ns1:EquipmentGroup>SPOI</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>21300</ns1:DatEquipmentId>
                           <ns1:Description>Stoßfänger Wagenfarbe</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>22300</ns1:DatEquipmentId>
                           <ns1:Description>Wärmeschutzverglasung</ns1:Description>
                           <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>24409</ns1:DatEquipmentId>
                           <ns1:Description>Radiovorbereitung, 6 Lautsprecher</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25604</ns1:DatEquipmentId>
                           <ns1:Description>Bordcomputer / Check-Control</ns1:Description>
                           <ns1:EquipmentGroup>COMP</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25611</ns1:DatEquipmentId>
                           <ns1:Description>Multi-Funktions-Display</ns1:Description>
                           <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>25699</ns1:DatEquipmentId>
                                 <ns1:Description>Schaltpunktanzeige (Gear Shift Indicator)</ns1:Description>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25620</ns1:DatEquipmentId>
                           <ns1:Description>Infotainment-System: UConnect mit CD- und MP3-Player</ns1:Description>
                           <ns1:EquipmentGroup>CD</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>24827</ns1:DatEquipmentId>
                                 <ns1:Description>Blue &amp; Me Bluetooth-Freisprecheinrichtung mit Spracherkennung und USB-Anschluss</ns1:Description>
                                 <ns1:EquipmentGroup>TEL4</ns1:EquipmentGroup>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25702</ns1:DatEquipmentId>
                           <ns1:Description>Außentemperaturanzeige</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26708</ns1:DatEquipmentId>
                           <ns1:Description>Geschwindigkeits-Regelanlage (Tempomat)</ns1:Description>
                           <ns1:EquipmentGroup>TEMP</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26803</ns1:DatEquipmentId>
                           <ns1:Description>Airbag Fahrer-/Beifahrerseite</ns1:Description>
                           <ns1:EquipmentGroup>AIR1</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26901</ns1:DatEquipmentId>
                           <ns1:Description>Kopf-Airbag-System</ns1:Description>
                           <ns1:EquipmentGroup>AIR4</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26905</ns1:DatEquipmentId>
                           <ns1:Description>Seitenairbag</ns1:Description>
                           <ns1:EquipmentGroup>AIR3</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26909</ns1:DatEquipmentId>
                           <ns1:Description>Airbag Beifahrerseite abschaltbar</ns1:Description>
                           <ns1:EquipmentGroup>AIR2</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27300</ns1:DatEquipmentId>
                           <ns1:Description>Mittelarmlehne hinten</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>33901</ns1:DatEquipmentId>
                                 <ns1:Description>Durchladeeinrichtung (Mittelarmlehne hinten)</ns1:Description>
                                 <ns1:EquipmentGroup>DULA</ns1:EquipmentGroup>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>38909</ns1:DatEquipmentId>
                                 <ns1:Description>Getränkehalter hinten</ns1:Description>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>28399</ns1:DatEquipmentId>
                           <ns1:Description>Fußmatten</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>29003</ns1:DatEquipmentId>
                           <ns1:Description>Klimaautomatik 2-Zonen</ns1:Description>
                           <ns1:EquipmentGroup>KLI2</ns1:EquipmentGroup>
                          <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>29393</ns1:DatEquipmentId>
                                 <ns1:Description>Luftdüsen im Fond</ns1:Description>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>29401</ns1:DatEquipmentId>
                           <ns1:Description>Zusatzheizung</ns1:Description>
                           <ns1:EquipmentGroup>ZUHE</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>30014</ns1:DatEquipmentId>
                           <ns1:Description>Sitzbezug / Polsterung: Stoff Competizione</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>32704</ns1:DatEquipmentId>
                           <ns1:Description>Sitz vorn links höhenverstellbar</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>33603</ns1:DatEquipmentId>
                           <ns1:Description>Rücksitz geteilt/klappbar</ns1:Description>
                           <ns1:EquipmentGroup>SITH</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>34704</ns1:DatEquipmentId>
                           <ns1:Description>Aktive Kopfstützen vorn</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>34807</ns1:DatEquipmentId>
                           <ns1:Description>Kopfstützen hinten (3-fach)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35001</ns1:DatEquipmentId>
                           <ns1:Description>Fensterheber elektrisch vorn</ns1:Description>
                           <ns1:EquipmentGroup>FH2</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35002</ns1:DatEquipmentId>
                           <ns1:Description>Fensterheber elektrisch hinten</ns1:Description>
                           <ns1:EquipmentGroup>FH4</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35301</ns1:DatEquipmentId>
                           <ns1:Description>Zentralverriegelung mit Fernbedienung</ns1:Description>
                           <ns1:EquipmentGroup>ZV</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>38106</ns1:DatEquipmentId>
                           <ns1:Description>Wegfahrsperre (elektronisch)</ns1:Description>
                           <ns1:EquipmentGroup>WFS</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39307</ns1:DatEquipmentId>
                           <ns1:Description>Isofix-Aufnahmen für Kindersitz</ns1:Description>
                           <ns1:EquipmentGroup>KISI</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39408</ns1:DatEquipmentId>
                           <ns1:Description>Schalt-/Wählhebelgriff Aluminium</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40000</ns1:DatEquipmentId>
                           <ns1:Description>Anti-Blockier-System (ABS)</ns1:Description>
                           <ns1:EquipmentGroup>ABS</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40307</ns1:DatEquipmentId>
                           <ns1:Description>Elektron. Bremskraftverteiler (EBD)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40801</ns1:DatEquipmentId>
                           <ns1:Description>Bremsassistent (HBA / EBA)</ns1:Description>
                          <ns1:EquipmentGroup>FA01</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40925</ns1:DatEquipmentId>
                           <ns1:Description>Kurvenbremskontrolle (CBC / ESBS)</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>42607</ns1:DatEquipmentId>
                           <ns1:Description>Vehicle-Dynamic-Control (ESP / VDC)</ns1:Description>
                           <ns1:EquipmentGroup>FARS</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>47802</ns1:DatEquipmentId>
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
                           <ns1:DatEquipmentId>69108</ns1:DatEquipmentId>
                           <ns1:Description>Lenkrad (Leder) + Schalt-/Wählhebelgriff Leder</ns1:Description>
                           <ns1:EquipmentGroup>LEN1</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>69009</ns1:DatEquipmentId>
                                 <ns1:Description>Lenkrad (Leder)</ns1:Description>
                                 <ns1:EquipmentGroup>LEN1</ns1:EquipmentGroup>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>69502</ns1:DatEquipmentId>
                           <ns1:Description>Lenksäule (Lenkrad) verstellbar (vertikal / axial)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>69800</ns1:DatEquipmentId>
                           <ns1:Description>Servolenkung</ns1:Description>
                           <ns1:EquipmentGroup>SL</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>70042</ns1:DatEquipmentId>
                           <ns1:Description>Elektron. Differentialsperre (Q2)</ns1:Description>
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
                           <ns1:DatEquipmentId>70516</ns1:DatEquipmentId>
                           <ns1:Description>Fahrassistenz-System: Alfa Romeo D.N.A.-Fahrdynamik-System</ns1:Description>
                           <ns1:EquipmentGroup>FA40</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>70603</ns1:DatEquipmentId>
                           <ns1:Description>Fahrassistenz-System: Berganfahrhilfe (Hill-Holder)</ns1:Description>
                           <ns1:EquipmentGroup>FA16</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>77225</ns1:DatEquipmentId>
                           <ns1:Description>Schadstoffarm nach Abgasnorm Euro 5</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>77601</ns1:DatEquipmentId>
                           <ns1:Description>Start/Stop-Anlage</ns1:Description>
                           <ns1:EquipmentGroup>MSSA</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>77602</ns1:DatEquipmentId>
                           <ns1:Description>Rußpartikelfilter</ns1:Description>
                           <ns1:EquipmentGroup>DPF</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>77716</ns1:DatEquipmentId>
                           <ns1:Description>Auspuffendrohr verchromt</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>79706</ns1:DatEquipmentId>
                           <ns1:Description>Motor-Schleppmoment-Regulator (MSR / EDC)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                           <ns1:Description>Karosserie: 5-türig</ns1:Description>
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
                           <ns1:DatEquipmentId>83402</ns1:DatEquipmentId>
                           <ns1:Description>Motor 1,6 Ltr. - 77 kW JTDM KAT</ns1:Description>
                           <ns1:EquipmentType>engine</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                     </ns1:SeriesEquipment>
                     <ns1:DeselectedSeriesEquipment>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>74900</ns1:DatEquipmentId>
                           <ns1:Description>Getriebe 6-Gang - Doppelkupplungsgetriebe TCT</ns1:Description>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>47801</ns1:DatEquipmentId>
                           <ns1:Description>LM-Felgen</ns1:Description>
                        </ns1:EquipmentPosition>
                     </ns1:DeselectedSeriesEquipment>
                  </ns1:Equipment>
                  <ns1:Tires>
                     <ns1:Axles>
                        <ns1:Axle>
                           <ns1:AxleNo>1</ns1:AxleNo>
                           <ns1:TireId>10000382</ns1:TireId>
                           <ns1:TireState>mounted</ns1:TireState>
                           <ns1:NrOfTires>2</ns1:NrOfTires>
                           <ns1:TireOriginalPrice origin="dat">100</ns1:TireOriginalPrice>
                           <ns1:TireSpeedIndex></ns1:TireSpeedIndex>
                           <ns1:TireSize>205/55R16</ns1:TireSize>
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
                           <ns1:TireId>10000382</ns1:TireId>
                           <ns1:TireState>mounted</ns1:TireState>
                           <ns1:NrOfTires>2</ns1:NrOfTires>
                           <ns1:TireOriginalPrice origin="dat">100</ns1:TireOriginalPrice>
                           <ns1:TireSpeedIndex></ns1:TireSpeedIndex>
                           <ns1:TireSize>205/55R16</ns1:TireSize>
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
                        <ns1:DatEquipmentId>83402</ns1:DatEquipmentId>
                        <ns1:Description>Motor 1,6 Ltr. - 77 kW JTDM KAT</ns1:Description>
                        <ns1:EquipmentClass>1</ns1:EquipmentClass>
                     </ns1:EquipmentPosition>
                     <ns1:EquipmentPosition>
                        <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                        <ns1:Description>Karosserie: 5-türig</ns1:Description>
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
                  <ns1:VatType>regular</ns1:VatType>
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
                  <ns1:OriginalPrice origin="dat">20672</ns1:OriginalPrice>
                  <ns1:OriginalPriceGross origin="dat">24600</ns1:OriginalPriceGross>
                  <ns1:BasePrice origin="dat">5787.00</ns1:BasePrice>
                  <ns1:ReferenceMileage>162000</ns1:ReferenceMileage>
                  <ns1:MileageCorr origin="dat">1258.86</ns1:MileageCorr>
                  <ns1:ResidualValueModel>dat</ns1:ResidualValueModel>
                  <ns1:InitialRegistrationCorr origin="dat">35.23</ns1:InitialRegistrationCorr>
                  <ns1:BasePrice2 origin="dat">7081.09</ns1:BasePrice2>
                  <ns1:EquipmentSign>calculated value</ns1:EquipmentSign>
                  <ns1:EquipmentOriginalPrice origin="dat">0</ns1:EquipmentOriginalPrice>
                  <ns1:EquipmentPrice origin="dat">0</ns1:EquipmentPrice>
                  <ns1:ValuationCorrection origin="dat">-354.05</ns1:ValuationCorrection>
                  <ns1:BasePrice3 origin="dat">7081.09</ns1:BasePrice3>
                  <ns1:ConditionCorrectionPerc origin="dat">95.00</ns1:ConditionCorrectionPerc>
                  <ns1:SalesPrice origin="dat">6727.04</ns1:SalesPrice>
                  <ns1:SalesPriceRounded origin="dat">6725</ns1:SalesPriceRounded>
                  <ns1:SalesPriceGross origin="dat">8005.18</ns1:SalesPriceGross>
                  <ns1:SalesPriceGrossRounded origin="dat">8000</ns1:SalesPriceGrossRounded>
                  <ns1:Margin origin="dat">1297.42</ns1:Margin>
                  <ns1:MarginRounded origin="dat">1300</ns1:MarginRounded>
                  <ns1:MarginGross origin="dat">1543.93</ns1:MarginGross>
                  <ns1:MarginGrossRounded origin="dat">1550</ns1:MarginGrossRounded>
                  <ns1:MarginPerc>19.29</ns1:MarginPerc>
                  <ns1:PurchasePrice origin="dat">5429.62</ns1:PurchasePrice>
                  <ns1:PurchasePriceRounded origin="dat">5425</ns1:PurchasePriceRounded>
                  <ns1:PurchasePriceGross origin="dat">6461.25</ns1:PurchasePriceGross>
                  <ns1:PurchasePriceGrossRounded origin="dat">6450</ns1:PurchasePriceGrossRounded>
                  <ns1:LastValuationDataYear>2025</ns1:LastValuationDataYear>
                  <ns1:LastValuationDataMonth>1</ns1:LastValuationDataMonth>
                  <ns1:LastValuationDate>2024-12-19T08:50:19.697+01:00</ns1:LastValuationDate>
                  <ns1:Currency>EUR</ns1:Currency>
                  <ns1:SignMilageUnit>kilometers</ns1:SignMilageUnit>
                  <ns1:Obsolete>up to date</ns1:Obsolete>
                  <ns1:DisplayGross>true</ns1:DisplayGross>
                  <ns1:DisplayRounded>true</ns1:DisplayRounded>
                  <ns1:DefaultTiresPrice origin="dat">200.00</ns1:DefaultTiresPrice>
                  <ns1:SignDeterminatedDate>true</ns1:SignDeterminatedDate>
                  <ns1:DeterminatedDate>2024-12-19+01:00</ns1:DeterminatedDate>
                  <ns1:ValuationType>valuation</ns1:ValuationType>
                  <ns1:ExtendedMileageCorrection>true</ns1:ExtendedMileageCorrection>
                  <ns1:Condition>
                     <ns1:OwnerCorrectionPerc origin="dat">5.0</ns1:OwnerCorrectionPerc>
                     <ns1:OwnerCorrectionAmount>-354.05</ns1:OwnerCorrectionAmount>
                     <ns1:OwnerCorrectionAmountGross>-421.32</ns1:OwnerCorrectionAmountGross>
                     <ns1:ConditionCorrectionFactorPerc origin="dat">100</ns1:ConditionCorrectionFactorPerc>
                     <ns1:ConditionCorrectionAmount>0.00</ns1:ConditionCorrectionAmount>
                     <ns1:ConditionCorrectionAmountGross>0.00</ns1:ConditionCorrectionAmountGross>
                     <ns1:NumberOfOwnersN>5</ns1:NumberOfOwnersN>
                     <ns1:ConditionSubTotal1>7081.09</ns1:ConditionSubTotal1>
                     <ns1:ConditionSubTotal1Gross>8426.50</ns1:ConditionSubTotal1Gross>
                     <ns1:ConditionSubTotal2>6727.04</ns1:ConditionSubTotal2>
                     <ns1:ConditionSubTotal2Gross>8005.18</ns1:ConditionSubTotal2Gross>
                     <ns1:RepairCostsInTradeMargin>false</ns1:RepairCostsInTradeMargin>
                  </ns1:Condition>
                  <ns1:Parameters/>
               </ns1:Valuation>
            </ns1:Dossier>
         </VXS>
      </ns4:changeDossierNResponse>
   </S:Body>
</S:Envelope>
```
