---
title: "Response calculateN"
topic_id: "18898"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > Reparaturkostenkalkulation ohne Speicherung > Response calculateN"
---

# Response calculateN

<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns10:calculateNResponse xmlns:ns10="http://www.dat.eu/myClaim/soap/v2/VehicleRepairService">
         <calculationResult source="SD3" type="VehicleRepairOnline">
            <ns1:Dossier xmlns:ns1="http://www.dat.de/vxs">
               <ns1:Description>TestCalculationInMemory</ns1:Description>
               <ns1:UUID>7b3265aa-2313-4f42-b6aa-9f39f49a0941</ns1:UUID>
               <ns1:Country>DE</ns1:Country>
               <ns1:Language>de_DE</ns1:Language>
               <ns1:DataVersion>1</ns1:DataVersion>
               <ns1:Currency>EUR</ns1:Currency>
               <ns1:DatCustomerId>9999999</ns1:DatCustomerId>
               <ns1:DossierType>myClaim</ns1:DossierType>
               <ns1:CreateDate>2023-12-22T14:38:58.376+01:00</ns1:CreateDate>
               <ns1:ChangeDate>2023-12-22T14:38:58.539+01:00</ns1:ChangeDate>
               <ns1:DatCustomerAddress>
                  <ns1:Title>titleCompany</ns1:Title>
                  <ns1:CompanyName>PL-C-S</ns1:CompanyName>
                  <ns1:NameLong>DAT intern</ns1:NameLong>
                  <ns1:Country>DE</ns1:Country>
                  <ns1:TaxNumber>123123</ns1:TaxNumber>
                  <ns1:CustomerNumber>9999999</ns1:CustomerNumber>
                  <ns1:CustomerType>9999999</ns1:CustomerType>
                  <ns1:Street>Hellmuth-Hirth-Str.</ns1:Street>
                  <ns1:StreetNumber>1</ns1:StreetNumber>
                  <ns1:StreetZipCode>73630</ns1:StreetZipCode>
                  <ns1:StreetCity>Ostfildern</ns1:StreetCity>
                  <ns1:EMail>Email@dat.de</ns1:EMail>
                  <ns1:BIC>123123</ns1:BIC>
                  <ns1:IBAN>DE123123123</ns1:IBAN>
                  <ns1:UsageFlag>9</ns1:UsageFlag>
               </ns1:DatCustomerAddress>
               <ns1:Vehicle>
                  <ns1:VehicleIdentNumber>WBADEXTESTSTUB001</ns1:VehicleIdentNumber>
                  <ns1:DatECode>011301110300002</ns1:DatECode>
                  <ns1:Container>DE006</ns1:Container>
                  <ns1:ConstructionTime>5297</ns1:ConstructionTime>
                  <ns1:VehicleTypeName origin="dat">Passenger car, SUV, small van</ns1:VehicleTypeName>
                  <ns1:VehicleTypeNameN origin="dat">Passenger car, SUV, small van</ns1:VehicleTypeNameN>
                  <ns1:ManufacturerName origin="dat">BMW</ns1:ManufacturerName>
                  <ns1:BaseModelName origin="dat">Serie 5 Touring (F11)(2010->)</ns1:BaseModelName>
                  <ns1:SubModelName origin="dat">520d</ns1:SubModelName>
                  <ns1:ContainerName>DE - Kb5 520 d EU6, Touring DPF (Euro 6), (Facelift) 2013 - 2014</ns1:ContainerName>
                  <ns1:ContainerNameN origin="dat">DE - Kb5 520 d EU6, Touring DPF (Euro 6), (Facelift) 2013 - 2014</ns1:ContainerNameN>
                  <ns1:VehicleType>1</ns1:VehicleType>
                  <ns1:Manufacturer>130</ns1:Manufacturer>
                  <ns1:BaseModel>111</ns1:BaseModel>
                  <ns1:SubModel>30</ns1:SubModel>
                  <ns1:IdentificationSource>IDENTIFICATIONSOURCE_VIN</ns1:IdentificationSource>
                  <ns1:Country>DE</ns1:Country>
                  <ns1:SubModelVariant>2</ns1:SubModelVariant>
                  <ns1:RegistrationData/>
                  <ns1:Engine/>
                  <ns1:TechInfo>
                     <ns1:FillingQuantities>
                        <ns1:Fluid code="N47D20" desc="Engine" type="1">
                           <ns1:Capacity condition="Service filling" desc="Filling amount (total)" min="5.20" unit="Litre"/>
                           <ns1:Recommendation>
                              <ns1:Usage type="0">Normal</ns1:Usage>
                              <ns1:Interval type="1">Change 30000 km/ 24 months</ns1:Interval>
                              <ns1:Product>TITAN GT1 PRO FLEX SAE 5W-30 (XTL-Technology)</ns1:Product>
                              <ns1:Product>TITAN GT1 PRO C-3 SAE 5W-30 (XTL-Technology)</ns1:Product>
                              <ns1:Product>TITAN GT1 SAE 5W-40 (XTL-Technology)</ns1:Product>
                           </ns1:Recommendation>
                        </ns1:Fluid>
                        <ns1:Fluid desc="Cooling system" type="8">
                           <ns1:Capacity desc="Filling amount (total)" max="7.50" min="7.20" unit="Litre"/>
                           <ns1:Recommendation>
                              <ns1:Usage type="0">Normal</ns1:Usage>
                              <ns1:Product>MAINTAIN FRICOFIN</ns1:Product>
                           </ns1:Recommendation>
                        </ns1:Fluid>
                        <ns1:Fluid code="205AL" desc="Rear differential" type="3">
                           <ns1:Capacity desc="Filling amount (total)" min="0.80" unit="Litre"/>
                           <ns1:Recommendation>
                              <ns1:Usage type="0">Normal</ns1:Usage>
                              <ns1:Product>TITAN SINTOPOID LS SAE 75W-90</ns1:Product>
                           </ns1:Recommendation>
                        </ns1:Fluid>
                        <ns1:Fluid code="ZF GA8HP 8/1" desc="Automatic transmission" type="3">
                           <ns1:Capacity desc="Filling amount (total)" min="8.50" unit="Litre"/>
                           <ns1:Recommendation>
                              <ns1:Usage type="0">Normal</ns1:Usage>
                              <ns1:Product>TITAN ATF 6009</ns1:Product>
                              <ns1:Product>TITAN ATF 6008</ns1:Product>
                           </ns1:Recommendation>
                        </ns1:Fluid>
                     </ns1:FillingQuantities>
                     <ns1:GearboxType>automatic</ns1:GearboxType>
                     <ns1:ProductGroupName/>
                     <ns1:TechInfoWltp/>
                  </ns1:TechInfo>
                  <ns1:Equipment>
                     <ns1:SeriesEquipment>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26909</ns1:DatEquipmentId>
                           <ns1:Description>airbag passenger side deactivatable</ns1:Description>
                           <ns1:EquipmentGroup>AIR2</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26803</ns1:DatEquipmentId>
                           <ns1:Description>airbag driver side/passenger side</ns1:Description>
                           <ns1:EquipmentGroup>AIR1</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>34704</ns1:DatEquipmentId>
                           <ns1:Description>active headrests</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>10715</ns1:DatEquipmentId>
                           <ns1:Description>active hood</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40000</ns1:DatEquipmentId>
                           <ns1:Description>antilock braking system (ABS)</ns1:Description>
                           <ns1:EquipmentGroup>ABS</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18604</ns1:DatEquipmentId>
                           <ns1:Description>automatic headlight control</ns1:Description>
                           <ns1:EquipmentGroup>AUFL</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>24999</ns1:DatEquipmentId>
                           <ns1:Description>AUX-IN interface (AUX-IN)</ns1:Description>
                           <ns1:EquipmentGroup>MP3A</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>15200</ns1:DatEquipmentId>
                           <ns1:Description>exterior mirror electrically adjustable and heated</ns1:Description>
                           <ns1:EquipmentGroup>AUSP</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25702</ns1:DatEquipmentId>
                           <ns1:Description>outside temperature display</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18505</ns1:DatEquipmentId>
                           <ns1:Description>bi-xenon headlights</ns1:Description>
                           <ns1:EquipmentGroup>XELI</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>19000</ns1:DatEquipmentId>
                                 <ns1:Description>headlight washer system (headlight washer system)</ns1:Description>
                                 <ns1:EquipmentGroup>SWRA</ns1:EquipmentGroup>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>18913</ns1:DatEquipmentId>
                                 <ns1:Description>daytime running lights LED</ns1:Description>
                                 <ns1:EquipmentGroup>TFAL</ns1:EquipmentGroup>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>18940</ns1:DatEquipmentId>
                                 <ns1:Description>turn signal lights LED</ns1:Description>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25508</ns1:DatEquipmentId>
                           <ns1:Description>trip computer</ns1:Description>
                           <ns1:EquipmentGroup>COMP</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40801</ns1:DatEquipmentId>
                           <ns1:Description>brake assistant</ns1:Description>
                           <ns1:EquipmentGroup>FA01</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40050</ns1:DatEquipmentId>
                           <ns1:Description>braking energy recovery (recovery system)</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25606</ns1:DatEquipmentId>
                           <ns1:Description>Check-Control system</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25300</ns1:DatEquipmentId>
                           <ns1:Description>tachometer</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18898</ns1:DatEquipmentId>
                           <ns1:Description>dynamic brake light</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>70100</ns1:DatEquipmentId>
                           <ns1:Description>dynamic stability control (DSC)</ns1:Description>
                           <ns1:EquipmentGroup>ESP</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>11406</ns1:DatEquipmentId>
                           <ns1:Description>exterior scopes vehicle colour</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>70518</ns1:DatEquipmentId>
                           <ns1:Description>driver assistance system: driving-experience switch</ns1:Description>
                           <ns1:EquipmentGroup>FA22</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35003</ns1:DatEquipmentId>
                           <ns1:Description>window lifter electric front + rear</ns1:Description>
                           <ns1:EquipmentGroup>FH4</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>24833</ns1:DatEquipmentId>
                           <ns1:Description>hands-free system with USB port</ns1:Description>
                           <ns1:EquipmentGroup>TEL3</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>28402</ns1:DatEquipmentId>
                           <ns1:Description>floor mats velours</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27605</ns1:DatEquipmentId>
                           <ns1:Description>cargo space partition (net)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27400</ns1:DatEquipmentId>
                           <ns1:Description>cargo space cover / roll-up cover</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26710</ns1:DatEquipmentId>
                           <ns1:Description>cruise control with brake function</ns1:Description>
                           <ns1:EquipmentGroup>TEMP</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39402</ns1:DatEquipmentId>
                           <ns1:Description>beverage holder front and rear</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35506</ns1:DatEquipmentId>
                           <ns1:Description>liftgate control automatic</ns1:Description>
                           <ns1:EquipmentGroup>HKEL</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>19300</ns1:DatEquipmentId>
                           <ns1:Description>rear window wiper</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39308</ns1:DatEquipmentId>
                           <ns1:Description>Isofix mounts for child seat at rear seat</ns1:Description>
                           <ns1:EquipmentGroup>KISI</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                           <ns1:Description>body: 5-door</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26805</ns1:DatEquipmentId>
                           <ns1:Description>head airbag system rear</ns1:Description>
                           <ns1:EquipmentGroup>AIR4</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26804</ns1:DatEquipmentId>
                           <ns1:Description>head airbag system front</ns1:Description>
                           <ns1:EquipmentGroup>AIR4</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>69007</ns1:DatEquipmentId>
                           <ns1:Description>steering wheel (leather) with multiple function</ns1:Description>
                           <ns1:EquipmentGroup>LEN2</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>69505</ns1:DatEquipmentId>
                                 <ns1:Description>steering column (steering wheel) mechanic. adjustable</ns1:Description>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>69505</ns1:DatEquipmentId>
                           <ns1:Description>steering column (steering wheel) mechanic. adjustable</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>48535</ns1:DatEquipmentId>
                           <ns1:Description>light alloy rims 8x17 (V-spoke 236)</ns1:Description>
                           <ns1:EquipmentGroup>ALU</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>42905</ns1:DatEquipmentId>
                           <ns1:Description>air suspension rear axle</ns1:Description>
                           <ns1:EquipmentGroup>LUFT</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>42805</ns1:DatEquipmentId>
                                 <ns1:Description>ride-level control</ns1:Description>
                                 <ns1:EquipmentGroup>NIV</ns1:EquipmentGroup>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27300</ns1:DatEquipmentId>
                           <ns1:Description>center armrest rear</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27202</ns1:DatEquipmentId>
                           <ns1:Description>center armrest front</ns1:Description>
                           <ns1:EquipmentGroup>MALV</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>87410</ns1:DatEquipmentId>
                           <ns1:Description>engine 2,0 liter - 135 kW turbo diesel catalyst (N 47 T)</ns1:Description>
                           <ns1:EquipmentType>engine</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>96508</ns1:DatEquipmentId>
                                 <ns1:Description>engine 2,0 liter - 135 kW turbo diesel</ns1:Description>
                                 <ns1:EquipmentType>engine</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27309</ns1:DatEquipmentId>
                           <ns1:Description>multi-functional armrest in rear-seat area</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>42805</ns1:DatEquipmentId>
                           <ns1:Description>ride-level control</ns1:Description>
                           <ns1:EquipmentGroup>NIV</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>77015</ns1:DatEquipmentId>
                           <ns1:Description>NOx adsorber catalyst (BMW Blue Performance)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40803</ns1:DatEquipmentId>
                           <ns1:Description>parking brake electric</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>62004</ns1:DatEquipmentId>
                           <ns1:Description>tire 225/55 R17 ..Z</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>68802</ns1:DatEquipmentId>
                           <ns1:Description>tire repair kit (Mobility-Pack)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25906</ns1:DatEquipmentId>
                           <ns1:Description>tire puncture indicator</ns1:Description>
                           <ns1:EquipmentGroup>RDK</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>77602</ns1:DatEquipmentId>
                           <ns1:Description>diesel particulate filter</ns1:Description>
                           <ns1:EquipmentGroup>DPF</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>33508</ns1:DatEquipmentId>
                           <ns1:Description>rear seat backrest split/folding</ns1:Description>
                           <ns1:EquipmentGroup>SITH</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>77227</ns1:DatEquipmentId>
                           <ns1:Description>low emissions according to emission standard Euro 6</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>19102</ns1:DatEquipmentId>
                           <ns1:Description>windshield washer jets heated</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>19101</ns1:DatEquipmentId>
                           <ns1:Description>windshield wiper with rain sensor</ns1:Description>
                           <ns1:EquipmentGroup>SWRE</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>19000</ns1:DatEquipmentId>
                           <ns1:Description>headlight washer system (headlight washer system)</ns1:Description>
                           <ns1:EquipmentGroup>SWRA</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26903</ns1:DatEquipmentId>
                           <ns1:Description>sidebag front</ns1:Description>
                           <ns1:EquipmentGroup>AIR3</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25151</ns1:DatEquipmentId>
                           <ns1:Description>Service system: intelligent emergency call incl. TeleServices</ns1:Description>
                           <ns1:EquipmentGroup>FA10</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>69811</ns1:DatEquipmentId>
                           <ns1:Description>power steering Servotronic</ns1:Description>
                           <ns1:EquipmentGroup>SL</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>32811</ns1:DatEquipmentId>
                           <ns1:Description>seats front semi-electrically adjustable</ns1:Description>
                           <ns1:EquipmentGroup>SITE</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35408</ns1:DatEquipmentId>
                           <ns1:Description>soft-close automatic for trunk / liftgate</ns1:Description>
                           <ns1:EquipmentGroup>HKEL</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35513</ns1:DatEquipmentId>
                           <ns1:Description>start-stop button</ns1:Description>
                           <ns1:EquipmentGroup>MSSA</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>77601</ns1:DatEquipmentId>
                           <ns1:Description>start/stop system (function)</ns1:Description>
                           <ns1:EquipmentGroup>MSSA</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39016</ns1:DatEquipmentId>
                           <ns1:Description>power outlet (12V outlet) 3-fold</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>73017</ns1:DatEquipmentId>
                           <ns1:Description>absorbed glass mat (AGM) battery 80 Ah (AGM)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>38105</ns1:DatEquipmentId>
                           <ns1:Description>immobilizer</ns1:Description>
                           <ns1:EquipmentGroup>WFS</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>22218</ns1:DatEquipmentId>
                           <ns1:Description>heat/sun protection glazing combined (rear darkened)</ns1:Description>
                           <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35301</ns1:DatEquipmentId>
                           <ns1:Description>central locking system with remote control</ns1:Description>
                           <ns1:EquipmentGroup>ZV</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>96508</ns1:DatEquipmentId>
                           <ns1:Description>engine 2,0 liter - 135 kW turbo diesel</ns1:Description>
                           <ns1:EquipmentType>engine</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18913</ns1:DatEquipmentId>
                           <ns1:Description>daytime running lights LED</ns1:Description>
                           <ns1:EquipmentGroup>TFAL</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18940</ns1:DatEquipmentId>
                           <ns1:Description>turn signal lights LED</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                     </ns1:SeriesEquipment>
                     <ns1:DeselectedSeriesEquipment>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>24115</ns1:DatEquipmentId>
                           <ns1:Description>audio system BMW Professional (radio/CD player MP3-compatible)</ns1:Description>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25699</ns1:DatEquipmentId>
                           <ns1:Description>shift point indicator</ns1:Description>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25924</ns1:DatEquipmentId>
                           <ns1:Description>control display with colour monitor (6,5 inch)</ns1:Description>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26302</ns1:DatEquipmentId>
                           <ns1:Description>interior equipment interior trim strips, black high-gloss</ns1:Description>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>29003</ns1:DatEquipmentId>
                           <ns1:Description>automatic air-conditioning system 2-zone</ns1:Description>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>30470</ns1:DatEquipmentId>
                           <ns1:Description>seat covers/upholstery: cloth diagonal</ns1:Description>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>75205</ns1:DatEquipmentId>
                           <ns1:Description>transmission 6-speed</ns1:Description>
                        </ns1:EquipmentPosition>
                     </ns1:DeselectedSeriesEquipment>
                     <ns1:SpecialEquipment>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>37603</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>ambient lighting</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25804</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>audio navigation system Professional</ns1:Description>
                           <ns1:EquipmentGroup>GPS</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>24709</ns1:DatEquipmentId>
                                 <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                 <ns1:Description>voice-command system</ns1:Description>
                                 <ns1:EquipmentGroup>TEL4</ns1:EquipmentGroup>
                                 <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>8702</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>exterior equipment: Shadow-Line high-gloss</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25930</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>control display with colour monitor (9,2 inch)</ns1:Description>
                           <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27810</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>roof liner anthracite (BMW Individual)</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>16198</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>roof rails high-gloss Shadow-Line</ns1:Description>
                           <ns1:EquipmentGroup>DARE</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25704</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>driver assistance system: speed limit display</ns1:Description>
                           <ns1:EquipmentGroup>FA28</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>22505</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>windshield (variant: climate comfort)</ns1:Description>
                           <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>75914</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>automatic transmission - with Steptronic (8-speed)</ns1:Description>
                           <ns1:EquipmentGroup>AG2</ns1:EquipmentGroup>
                           <ns1:GearBoxType>automatic</ns1:GearBoxType>
                           <ns1:NrOfGears>8</ns1:NrOfGears>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25204</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>head-up display</ns1:Description>
                           <ns1:EquipmentGroup>HUD</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>25930</ns1:DatEquipmentId>
                                 <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                 <ns1:Description>control display with colour monitor (9,2 inch)</ns1:Description>
                                 <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>25413</ns1:DatEquipmentId>
                                 <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                 <ns1:Description>instrument combination (extended scope)</ns1:Description>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>24607</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>HiFi speaker system</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>31408</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>interior equipment interior trim strips aluminium fine-grain straight-brushed</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>37901</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>interior mirror with automatic dimming</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25413</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>instrument combination (extended scope)</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>25930</ns1:DatEquipmentId>
                                 <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                 <ns1:Description>control display with colour monitor (9,2 inch)</ns1:Description>
                                 <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>28982</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>automatic air-conditioning system 2-zone with automatic recirculation control, extended scope</ns1:Description>
                           <ns1:EquipmentGroup>KLI2</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>33403</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>lumbar support seat front left and right, electrically adjustable</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>77240</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>model variant CO2 scope (code 1CB)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18313</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>front fog lights LED</ns1:Description>
                           <ns1:EquipmentGroup>BEL</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>16302</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>panoramic roof (glass)</ns1:Description>
                           <ns1:EquipmentGroup>SD2</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25802</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Park-Distance-Control (PDC)</ns1:Description>
                           <ns1:EquipmentGroup>PDC1</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>30301</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>seat covers/upholstery: leather Dakota</ns1:Description>
                           <ns1:EquipmentGroup>LEDE</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>29500</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>seat heating front</ns1:Description>
                           <ns1:EquipmentGroup>SITB</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>22102</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>sun protection glazing (rear darkened, BMW Individual)</ns1:Description>
                           <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>24709</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>voice-command system</ns1:Description>
                           <ns1:EquipmentGroup>TEL4</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                     </ns1:SpecialEquipment>
                  </ns1:Equipment>
                  <ns1:Tires>
                     <ns1:Axles/>
                  </ns1:Tires>
                  <ns1:DATECodeEquipment>
                     <ns1:EquipmentPosition>
                        <ns1:DatEquipmentId>96508</ns1:DatEquipmentId>
                        <ns1:Description>engine 2,0 liter - 135 kW turbo diesel</ns1:Description>
                        <ns1:EquipmentClass>1</ns1:EquipmentClass>
                     </ns1:EquipmentPosition>
                     <ns1:EquipmentPosition>
                        <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                        <ns1:Description>body: 5-door</ns1:Description>
                        <ns1:EquipmentClass>2</ns1:EquipmentClass>
                     </ns1:EquipmentPosition>
                     <ns1:EquipmentPosition>
                        <ns1:DatEquipmentId>75914</ns1:DatEquipmentId>
                        <ns1:Description>automatic transmission - with Steptronic (8-speed)</ns1:Description>
                        <ns1:EquipmentClass>11</ns1:EquipmentClass>
                     </ns1:EquipmentPosition>
                  </ns1:DATECodeEquipment>
               </ns1:Vehicle>
               <ns1:VAT>
                  <ns1:VatAtCalculationTime>19.0</ns1:VatAtCalculationTime>
               </ns1:VAT>
               <ns1:TradingData>
                  <ns1:ClientContactAddresses>
                     <ns1:ClientContactAddress>
                        <ns1:Title>titleCompany</ns1:Title>
                        <ns1:CompanyName>Firma</ns1:CompanyName>
                        <ns1:NameLong>Name2</ns1:NameLong>
                        <ns1:Country>DE</ns1:Country>
                        <ns1:TaxNumber>123123</ns1:TaxNumber>
                        <ns1:CustomerNumber>9999999</ns1:CustomerNumber>
                        <ns1:CustomerType>9999999</ns1:CustomerType>
                        <ns1:Street>Hellmuth-Hirth-Str.</ns1:Street>
                        <ns1:StreetNumber>1</ns1:StreetNumber>
                        <ns1:StreetZipCode>73630</ns1:StreetZipCode>
                        <ns1:StreetCity>Ostfildern</ns1:StreetCity>
                        <ns1:EMail>ST@dat.de</ns1:EMail>
                        <ns1:BIC>123123</ns1:BIC>
                        <ns1:IBAN>DE123123123</ns1:IBAN>
                        <ns1:UsageFlag>9</ns1:UsageFlag>
                     </ns1:ClientContactAddress>
                  </ns1:ClientContactAddresses>
               </ns1:TradingData>
               <ns1:RepairCalculation>
                  <ns1:Vehicle>
                     <ns1:VehicleIdentNumber>WBADEXTESTSTUB001</ns1:VehicleIdentNumber>
                     <ns1:DatECode>011301110300002</ns1:DatECode>
                     <ns1:Container>DE006</ns1:Container>
                     <ns1:ConstructionTime>5297</ns1:ConstructionTime>
                     <ns1:VehicleTypeName origin="dat">Passenger car, SUV, small van</ns1:VehicleTypeName>
                     <ns1:VehicleTypeNameN origin="dat">Passenger car, SUV, small van</ns1:VehicleTypeNameN>
                     <ns1:ManufacturerName origin="dat">BMW</ns1:ManufacturerName>
                     <ns1:BaseModelName origin="dat">Serie 5 Touring (F11)(2010->)</ns1:BaseModelName>
                     <ns1:SubModelName origin="dat">520d</ns1:SubModelName>
                     <ns1:ContainerName>DE - Kb5 520 d EU6, Touring DPF (Euro 6), (Facelift) 2013 - 2014</ns1:ContainerName>
                     <ns1:ContainerNameN origin="dat">DE - Kb5 520 d EU6, Touring DPF (Euro 6), (Facelift) 2013 - 2014</ns1:ContainerNameN>
                     <ns1:VehicleType>1</ns1:VehicleType>
                     <ns1:Manufacturer>130</ns1:Manufacturer>
                     <ns1:BaseModel>111</ns1:BaseModel>
                     <ns1:SubModel>30</ns1:SubModel>
                     <ns1:IdentificationSource>IDENTIFICATIONSOURCE_VIN</ns1:IdentificationSource>
                     <ns1:Country>DE</ns1:Country>
                     <ns1:SubModelVariant>2</ns1:SubModelVariant>
                     <ns1:RegistrationData/>
                     <ns1:Engine/>
                     <ns1:TechInfo>
                        <ns1:FillingQuantities>
                           <ns1:Fluid code="N47D20" desc="Engine" type="1">
                              <ns1:Capacity condition="Service filling" desc="Filling amount (total)" min="5.20" unit="Litre"/>
                              <ns1:Recommendation>
                                 <ns1:Usage type="0">Normal</ns1:Usage>
                                 <ns1:Interval type="1">Change 30000 km/ 24 months</ns1:Interval>
                                 <ns1:Product>TITAN GT1 PRO FLEX SAE 5W-30 (XTL-Technology)</ns1:Product>
                                 <ns1:Product>TITAN GT1 PRO C-3 SAE 5W-30 (XTL-Technology)</ns1:Product>
                                 <ns1:Product>TITAN GT1 SAE 5W-40 (XTL-Technology)</ns1:Product>
                              </ns1:Recommendation>
                           </ns1:Fluid>
                           <ns1:Fluid desc="Cooling system" type="8">
                              <ns1:Capacity desc="Filling amount (total)" max="7.50" min="7.20" unit="Litre"/>
                              <ns1:Recommendation>
                                 <ns1:Usage type="0">Normal</ns1:Usage>
                                 <ns1:Product>MAINTAIN FRICOFIN</ns1:Product>
                              </ns1:Recommendation>
                           </ns1:Fluid>
                           <ns1:Fluid code="205AL" desc="Rear differential" type="3">
                              <ns1:Capacity desc="Filling amount (total)" min="0.80" unit="Litre"/>
                              <ns1:Recommendation>
                                 <ns1:Usage type="0">Normal</ns1:Usage>
                                 <ns1:Product>TITAN SINTOPOID LS SAE 75W-90</ns1:Product>
                              </ns1:Recommendation>
                           </ns1:Fluid>
                           <ns1:Fluid code="ZF GA8HP 8/1" desc="Automatic transmission" type="3">
                              <ns1:Capacity desc="Filling amount (total)" min="8.50" unit="Litre"/>
                              <ns1:Recommendation>
                                 <ns1:Usage type="0">Normal</ns1:Usage>
                                 <ns1:Product>TITAN ATF 6009</ns1:Product>
                                 <ns1:Product>TITAN ATF 6008</ns1:Product>
                              </ns1:Recommendation>
                           </ns1:Fluid>
                        </ns1:FillingQuantities>
                        <ns1:GearboxType>automatic</ns1:GearboxType>
                        <ns1:ProductGroupName/>
                        <ns1:TechInfoWltp/>
                     </ns1:TechInfo>
                     <ns1:Equipment>
                        <ns1:SeriesEquipment>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>26909</ns1:DatEquipmentId>
                              <ns1:Description>airbag passenger side deactivatable</ns1:Description>
                              <ns1:EquipmentGroup>AIR2</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>26803</ns1:DatEquipmentId>
                              <ns1:Description>airbag driver side/passenger side</ns1:Description>
                              <ns1:EquipmentGroup>AIR1</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>34704</ns1:DatEquipmentId>
                              <ns1:Description>active headrests</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>10715</ns1:DatEquipmentId>
                              <ns1:Description>active hood</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>40000</ns1:DatEquipmentId>
                              <ns1:Description>antilock braking system (ABS)</ns1:Description>
                              <ns1:EquipmentGroup>ABS</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>18604</ns1:DatEquipmentId>
                              <ns1:Description>automatic headlight control</ns1:Description>
                              <ns1:EquipmentGroup>AUFL</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>24999</ns1:DatEquipmentId>
                              <ns1:Description>AUX-IN interface (AUX-IN)</ns1:Description>
                              <ns1:EquipmentGroup>MP3A</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>15200</ns1:DatEquipmentId>
                              <ns1:Description>exterior mirror electrically adjustable and heated</ns1:Description>
                              <ns1:EquipmentGroup>AUSP</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25702</ns1:DatEquipmentId>
                              <ns1:Description>outside temperature display</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>18505</ns1:DatEquipmentId>
                              <ns1:Description>bi-xenon headlights</ns1:Description>
                              <ns1:EquipmentGroup>XELI</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>19000</ns1:DatEquipmentId>
                                    <ns1:Description>headlight washer system (headlight washer system)</ns1:Description>
                                    <ns1:EquipmentGroup>SWRA</ns1:EquipmentGroup>
                                    <ns1:EquipmentType>glass</ns1:EquipmentType>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>18913</ns1:DatEquipmentId>
                                    <ns1:Description>daytime running lights LED</ns1:Description>
                                    <ns1:EquipmentGroup>TFAL</ns1:EquipmentGroup>
                                    <ns1:EquipmentType>glass</ns1:EquipmentType>
                                    <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>18940</ns1:DatEquipmentId>
                                    <ns1:Description>turn signal lights LED</ns1:Description>
                                    <ns1:EquipmentType>glass</ns1:EquipmentType>
                                    <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25508</ns1:DatEquipmentId>
                              <ns1:Description>trip computer</ns1:Description>
                              <ns1:EquipmentGroup>COMP</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>40801</ns1:DatEquipmentId>
                              <ns1:Description>brake assistant</ns1:Description>
                              <ns1:EquipmentGroup>FA01</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>40050</ns1:DatEquipmentId>
                              <ns1:Description>braking energy recovery (recovery system)</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25606</ns1:DatEquipmentId>
                              <ns1:Description>Check-Control system</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25300</ns1:DatEquipmentId>
                              <ns1:Description>tachometer</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>18898</ns1:DatEquipmentId>
                              <ns1:Description>dynamic brake light</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>70100</ns1:DatEquipmentId>
                              <ns1:Description>dynamic stability control (DSC)</ns1:Description>
                              <ns1:EquipmentGroup>ESP</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>11406</ns1:DatEquipmentId>
                              <ns1:Description>exterior scopes vehicle colour</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>70518</ns1:DatEquipmentId>
                              <ns1:Description>driver assistance system: driving-experience switch</ns1:Description>
                              <ns1:EquipmentGroup>FA22</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>35003</ns1:DatEquipmentId>
                              <ns1:Description>window lifter electric front + rear</ns1:Description>
                              <ns1:EquipmentGroup>FH4</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>24833</ns1:DatEquipmentId>
                              <ns1:Description>hands-free system with USB port</ns1:Description>
                              <ns1:EquipmentGroup>TEL3</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>28402</ns1:DatEquipmentId>
                              <ns1:Description>floor mats velours</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27605</ns1:DatEquipmentId>
                              <ns1:Description>cargo space partition (net)</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27400</ns1:DatEquipmentId>
                              <ns1:Description>cargo space cover / roll-up cover</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>26710</ns1:DatEquipmentId>
                              <ns1:Description>cruise control with brake function</ns1:Description>
                              <ns1:EquipmentGroup>TEMP</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>39402</ns1:DatEquipmentId>
                              <ns1:Description>beverage holder front and rear</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>35506</ns1:DatEquipmentId>
                              <ns1:Description>liftgate control automatic</ns1:Description>
                              <ns1:EquipmentGroup>HKEL</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>19300</ns1:DatEquipmentId>
                              <ns1:Description>rear window wiper</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>39308</ns1:DatEquipmentId>
                              <ns1:Description>Isofix mounts for child seat at rear seat</ns1:Description>
                              <ns1:EquipmentGroup>KISI</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                              <ns1:Description>body: 5-door</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>26805</ns1:DatEquipmentId>
                              <ns1:Description>head airbag system rear</ns1:Description>
                              <ns1:EquipmentGroup>AIR4</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>26804</ns1:DatEquipmentId>
                              <ns1:Description>head airbag system front</ns1:Description>
                              <ns1:EquipmentGroup>AIR4</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>69007</ns1:DatEquipmentId>
                              <ns1:Description>steering wheel (leather) with multiple function</ns1:Description>
                              <ns1:EquipmentGroup>LEN2</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>69505</ns1:DatEquipmentId>
                                    <ns1:Description>steering column (steering wheel) mechanic. adjustable</ns1:Description>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>69505</ns1:DatEquipmentId>
                              <ns1:Description>steering column (steering wheel) mechanic. adjustable</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>48535</ns1:DatEquipmentId>
                              <ns1:Description>light alloy rims 8x17 (V-spoke 236)</ns1:Description>
                              <ns1:EquipmentGroup>ALU</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>42905</ns1:DatEquipmentId>
                              <ns1:Description>air suspension rear axle</ns1:Description>
                              <ns1:EquipmentGroup>LUFT</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>42805</ns1:DatEquipmentId>
                                    <ns1:Description>ride-level control</ns1:Description>
                                    <ns1:EquipmentGroup>NIV</ns1:EquipmentGroup>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27300</ns1:DatEquipmentId>
                              <ns1:Description>center armrest rear</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27202</ns1:DatEquipmentId>
                              <ns1:Description>center armrest front</ns1:Description>
                              <ns1:EquipmentGroup>MALV</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>87410</ns1:DatEquipmentId>
                              <ns1:Description>engine 2,0 liter - 135 kW turbo diesel catalyst (N 47 T)</ns1:Description>
                              <ns1:EquipmentType>engine</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>96508</ns1:DatEquipmentId>
                                    <ns1:Description>engine 2,0 liter - 135 kW turbo diesel</ns1:Description>
                                    <ns1:EquipmentType>engine</ns1:EquipmentType>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27309</ns1:DatEquipmentId>
                              <ns1:Description>multi-functional armrest in rear-seat area</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>42805</ns1:DatEquipmentId>
                              <ns1:Description>ride-level control</ns1:Description>
                              <ns1:EquipmentGroup>NIV</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>77015</ns1:DatEquipmentId>
                              <ns1:Description>NOx adsorber catalyst (BMW Blue Performance)</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>40803</ns1:DatEquipmentId>
                              <ns1:Description>parking brake electric</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>62004</ns1:DatEquipmentId>
                              <ns1:Description>tire 225/55 R17 ..Z</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>68802</ns1:DatEquipmentId>
                              <ns1:Description>tire repair kit (Mobility-Pack)</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25906</ns1:DatEquipmentId>
                              <ns1:Description>tire puncture indicator</ns1:Description>
                              <ns1:EquipmentGroup>RDK</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>77602</ns1:DatEquipmentId>
                              <ns1:Description>diesel particulate filter</ns1:Description>
                              <ns1:EquipmentGroup>DPF</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>33508</ns1:DatEquipmentId>
                              <ns1:Description>rear seat backrest split/folding</ns1:Description>
                              <ns1:EquipmentGroup>SITH</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>77227</ns1:DatEquipmentId>
                              <ns1:Description>low emissions according to emission standard Euro 6</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>19102</ns1:DatEquipmentId>
                              <ns1:Description>windshield washer jets heated</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>19101</ns1:DatEquipmentId>
                              <ns1:Description>windshield wiper with rain sensor</ns1:Description>
                              <ns1:EquipmentGroup>SWRE</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>19000</ns1:DatEquipmentId>
                              <ns1:Description>headlight washer system (headlight washer system)</ns1:Description>
                              <ns1:EquipmentGroup>SWRA</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>26903</ns1:DatEquipmentId>
                              <ns1:Description>sidebag front</ns1:Description>
                              <ns1:EquipmentGroup>AIR3</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25151</ns1:DatEquipmentId>
                              <ns1:Description>Service system: intelligent emergency call incl. TeleServices</ns1:Description>
                              <ns1:EquipmentGroup>FA10</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>69811</ns1:DatEquipmentId>
                              <ns1:Description>power steering Servotronic</ns1:Description>
                              <ns1:EquipmentGroup>SL</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>32811</ns1:DatEquipmentId>
                              <ns1:Description>seats front semi-electrically adjustable</ns1:Description>
                              <ns1:EquipmentGroup>SITE</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>35408</ns1:DatEquipmentId>
                              <ns1:Description>soft-close automatic for trunk / liftgate</ns1:Description>
                              <ns1:EquipmentGroup>HKEL</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>35513</ns1:DatEquipmentId>
                              <ns1:Description>start-stop button</ns1:Description>
                              <ns1:EquipmentGroup>MSSA</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>77601</ns1:DatEquipmentId>
                              <ns1:Description>start/stop system (function)</ns1:Description>
                              <ns1:EquipmentGroup>MSSA</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>39016</ns1:DatEquipmentId>
                              <ns1:Description>power outlet (12V outlet) 3-fold</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>73017</ns1:DatEquipmentId>
                              <ns1:Description>absorbed glass mat (AGM) battery 80 Ah (AGM)</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>38105</ns1:DatEquipmentId>
                              <ns1:Description>immobilizer</ns1:Description>
                              <ns1:EquipmentGroup>WFS</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>22218</ns1:DatEquipmentId>
                              <ns1:Description>heat/sun protection glazing combined (rear darkened)</ns1:Description>
                              <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>35301</ns1:DatEquipmentId>
                              <ns1:Description>central locking system with remote control</ns1:Description>
                              <ns1:EquipmentGroup>ZV</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>96508</ns1:DatEquipmentId>
                              <ns1:Description>engine 2,0 liter - 135 kW turbo diesel</ns1:Description>
                              <ns1:EquipmentType>engine</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>18913</ns1:DatEquipmentId>
                              <ns1:Description>daytime running lights LED</ns1:Description>
                              <ns1:EquipmentGroup>TFAL</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>18940</ns1:DatEquipmentId>
                              <ns1:Description>turn signal lights LED</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                        </ns1:SeriesEquipment>
                        <ns1:DeselectedSeriesEquipment>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>24115</ns1:DatEquipmentId>
                              <ns1:Description>audio system BMW Professional (radio/CD player MP3-compatible)</ns1:Description>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25699</ns1:DatEquipmentId>
                              <ns1:Description>shift point indicator</ns1:Description>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25924</ns1:DatEquipmentId>
                              <ns1:Description>control display with colour monitor (6,5 inch)</ns1:Description>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>26302</ns1:DatEquipmentId>
                              <ns1:Description>interior equipment interior trim strips, black high-gloss</ns1:Description>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>29003</ns1:DatEquipmentId>
                              <ns1:Description>automatic air-conditioning system 2-zone</ns1:Description>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>30470</ns1:DatEquipmentId>
                              <ns1:Description>seat covers/upholstery: cloth diagonal</ns1:Description>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>75205</ns1:DatEquipmentId>
                              <ns1:Description>transmission 6-speed</ns1:Description>
                           </ns1:EquipmentPosition>
                        </ns1:DeselectedSeriesEquipment>
                        <ns1:SpecialEquipment>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>37603</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>ambient lighting</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25804</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>audio navigation system Professional</ns1:Description>
                              <ns1:EquipmentGroup>GPS</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>24709</ns1:DatEquipmentId>
                                    <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                    <ns1:Description>voice-command system</ns1:Description>
                                    <ns1:EquipmentGroup>TEL4</ns1:EquipmentGroup>
                                    <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>8702</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>exterior equipment: Shadow-Line high-gloss</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25930</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>control display with colour monitor (9,2 inch)</ns1:Description>
                              <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27810</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>roof liner anthracite (BMW Individual)</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>16198</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>roof rails high-gloss Shadow-Line</ns1:Description>
                              <ns1:EquipmentGroup>DARE</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25704</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>driver assistance system: speed limit display</ns1:Description>
                              <ns1:EquipmentGroup>FA28</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>22505</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>windshield (variant: climate comfort)</ns1:Description>
                              <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>75914</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>automatic transmission - with Steptronic (8-speed)</ns1:Description>
                              <ns1:EquipmentGroup>AG2</ns1:EquipmentGroup>
                              <ns1:GearBoxType>automatic</ns1:GearBoxType>
                              <ns1:NrOfGears>8</ns1:NrOfGears>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25204</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>head-up display</ns1:Description>
                              <ns1:EquipmentGroup>HUD</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>25930</ns1:DatEquipmentId>
                                    <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                    <ns1:Description>control display with colour monitor (9,2 inch)</ns1:Description>
                                    <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                                    <ns1:EquipmentType>glass</ns1:EquipmentType>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>25413</ns1:DatEquipmentId>
                                    <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                    <ns1:Description>instrument combination (extended scope)</ns1:Description>
                                    <ns1:EquipmentType>glass</ns1:EquipmentType>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>24607</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>HiFi speaker system</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>31408</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>interior equipment interior trim strips aluminium fine-grain straight-brushed</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>37901</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>interior mirror with automatic dimming</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25413</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>instrument combination (extended scope)</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>25930</ns1:DatEquipmentId>
                                    <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                    <ns1:Description>control display with colour monitor (9,2 inch)</ns1:Description>
                                    <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                                    <ns1:EquipmentType>glass</ns1:EquipmentType>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>28982</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>automatic air-conditioning system 2-zone with automatic recirculation control, extended scope</ns1:Description>
                              <ns1:EquipmentGroup>KLI2</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>33403</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>lumbar support seat front left and right, electrically adjustable</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>77240</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>model variant CO2 scope (code 1CB)</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>18313</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>front fog lights LED</ns1:Description>
                              <ns1:EquipmentGroup>BEL</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>16302</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>panoramic roof (glass)</ns1:Description>
                              <ns1:EquipmentGroup>SD2</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25802</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Park-Distance-Control (PDC)</ns1:Description>
                              <ns1:EquipmentGroup>PDC1</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>30301</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>seat covers/upholstery: leather Dakota</ns1:Description>
                              <ns1:EquipmentGroup>LEDE</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>29500</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>seat heating front</ns1:Description>
                              <ns1:EquipmentGroup>SITB</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>22102</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>sun protection glazing (rear darkened, BMW Individual)</ns1:Description>
                              <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>24709</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>voice-command system</ns1:Description>
                              <ns1:EquipmentGroup>TEL4</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                        </ns1:SpecialEquipment>
                     </ns1:Equipment>
                     <ns1:Tires>
                        <ns1:Axles/>
                     </ns1:Tires>
                     <ns1:DATECodeEquipment>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>96508</ns1:DatEquipmentId>
                           <ns1:Description>engine 2,0 liter - 135 kW turbo diesel</ns1:Description>
                           <ns1:EquipmentClass>1</ns1:EquipmentClass>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                           <ns1:Description>body: 5-door</ns1:Description>
                           <ns1:EquipmentClass>2</ns1:EquipmentClass>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>75914</ns1:DatEquipmentId>
                           <ns1:Description>automatic transmission - with Steptronic (8-speed)</ns1:Description>
                           <ns1:EquipmentClass>11</ns1:EquipmentClass>
                        </ns1:EquipmentPosition>
                     </ns1:DATECodeEquipment>
                  </ns1:Vehicle>
                  <ns1:RepairParameters>
                     <ns1:PhantomCalculation>false</ns1:PhantomCalculation>
                     <ns1:LacquerType>Metallic (2-layer)</ns1:LacquerType>
                     <ns1:LacquerTypeLayers>2</ns1:LacquerTypeLayers>
                     <ns1:TimeUnitsOfManufacturer>true</ns1:TimeUnitsOfManufacturer>
                     <ns1:WithDomusCalculation>false</ns1:WithDomusCalculation>
                     <ns1:DMSCalculation>false</ns1:DMSCalculation>
                  </ns1:RepairParameters>
                  <ns1:ProcedureRelatedParameters>
                     <ns1:ProcedureRelatedParameter attribute="vatRate" factor="CalculationFactor" type="Double">19.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="referenceSetName" factor="CalculationFactor" type="String">DAT-Default-CalcPro</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="biwOptimizationMode" factor="CalculationFactor" type="BiwOptimizationMode">AUTOMATIC</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="showLongWorkStrings" factor="CalculationFactor" type="Boolean">true</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="selectedLacquerMethod" factor="CalculationFactor" type="LacquerMethod">EURO_LACQUER</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="crossSeries" factor="CalculationFactor" type="CrossSeriesState">NO</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="withoutValuesOfAdditionallyRequiredPositions" factor="CalculationFactor" type="Boolean">false</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnit" factor="CalculationFactor" type="TimeUnitSystem">AW</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="CalculationFactor" type="Integer">12</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="dataCurrency" factor="CalculationFactor" type="String">EUR</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="smallSparePartCalculationModel" factor="SparePartFactor" type="SmallPartsCalculationModel">FLAT</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="priceDate" factor="SparePartFactor" type="Date">2022-09-01</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="priceSource" factor="SparePartFactor" type="PriceSource">DAT</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="smallSparePartPercentOfPart" factor="SparePartFactor" type="Double">2.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="mechanicWage1" factor="LabourCostFactor" mode="PER_TIME_SYSTEM" type="Price">0.0833</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="electricWage1" factor="LabourCostFactor" mode="PER_TIME_SYSTEM" type="Price">0.0833</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnit" factor="LabourCostFactor" type="TimeUnitSystem">AW</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="LabourCostFactor" type="Integer">12</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="bodyWage1" factor="LabourCostFactor" mode="PER_TIME_SYSTEM" type="Price">0.0833</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="preparationTimePercent" factor="EuroLacquerFactor" type="Double">100.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="preparationTimePlasticPercent" factor="EuroLacquerFactor" type="Double">100.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="materialMode" factor="EuroLacquerFactor" type="LacquerMaterialMode">LACQUER_METHOD</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="type" description="Metallic (2-layer)" factor="EuroLacquerFactor" type="String">12</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wage" factor="EuroLacquerFactor" mode="PER_TIME_SYSTEM" type="Price">0.0833</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="materialIndex" factor="EuroLacquerFactor" type="Double">100.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="typeSaved" factor="EuroLacquerFactor" type="Boolean">false</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wageMode" factor="EuroLacquerFactor" type="LacquerWageMode">PER_TIME</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wageInclMaterialMode" factor="EuroLacquerFactor" type="LacquerWageMode">PER_TIME</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="calculationType" factor="EuroLacquerFactor" type="LacquerCalculationMode">WAGE_MATERIAL_SEPARATELY</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="disposalCostPercent" factor="EuroLacquerFactor" type="Double">0.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnit" factor="EuroLacquerFactor" type="TimeUnitSystem">AW</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="EuroLacquerFactor" type="Integer">12</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="preparationTimePercent" factor="ManufacturerLacquerFactor" type="Double">100.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="materialMode" factor="ManufacturerLacquerFactor" type="LacquerMaterialMode">LACQUER_METHOD</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="typeSaved" factor="ManufacturerLacquerFactor" type="Boolean">true</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wageMode" factor="ManufacturerLacquerFactor" type="LacquerWageMode">PER_TIME</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wageInclMaterialMode" factor="ManufacturerLacquerFactor" type="LacquerWageMode">PER_TIME</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="calculationType" factor="ManufacturerLacquerFactor" type="LacquerCalculationMode">WAGE_MATERIAL_SEPARATELY</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnit" factor="ManufacturerLacquerFactor" type="TimeUnitSystem">AW</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="ManufacturerLacquerFactor" type="Integer">12</ns1:ProcedureRelatedParameter>
                  </ns1:ProcedureRelatedParameters>
                  <ns1:RepairPositions>
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>44910</ns1:DATProcessId>
                        <ns1:RepairType>replace</ns1:RepairType>
                        <ns1:Description>windshield</ns1:Description>
                        <ns1:IsManualDescription>false</ns1:IsManualDescription>
                        <ns1:ConstructionGroupId>1</ns1:ConstructionGroupId>
                        <ns1:ConstructionGroup>FRONT END MODULE OUTSIDE</ns1:ConstructionGroup>
                        <ns1:ConstructionGroupPolygon>65</ns1:ConstructionGroupPolygon>
                        <ns1:PositionEntryType>graphical</ns1:PositionEntryType>
                        <ns1:IsRepairExtension>false</ns1:IsRepairExtension>
                        <ns1:PreDamage>false</ns1:PreDamage>
                     </ns1:RepairPosition>
                  </ns1:RepairPositions>
                  <ns1:CalcResultToUse>common</ns1:CalcResultToUse>
                  <ns1:CalcResultCommon>
                     <ns1:MaterialPositions>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>44910</ns1:DATProcessId>
                           <ns1:PartNumber>51317333835</ns1:PartNumber>
                           <ns1:DATPartNumber>51317333835</ns1:DATPartNumber>
                           <ns1:Description>WINDSHIELD</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>797.82</ns1:ValuePerUnit>
                           <ns1:ValueTotal>797.82</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>797.82</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>40270</ns1:DATProcessId>
                           <ns1:PartNumber>51489162739</ns1:PartNumber>
                           <ns1:DATPartNumber>51489162739</ns1:DATPartNumber>
                           <ns1:Description>SOUND INSULATION WINDSHIELD COWL</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>49.34</ns1:ValuePerUnit>
                           <ns1:ValueTotal>49.34</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>49.34</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>44931</ns1:DATProcessId>
                           <ns1:PartNumber>51317203121</ns1:PartNumber>
                           <ns1:DATPartNumber>51317203121</ns1:DATPartNumber>
                           <ns1:Description>COVER WINDSHIELD TOP</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>23.69</ns1:ValuePerUnit>
                           <ns1:ValueTotal>23.69</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>23.69</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>44940</ns1:DATProcessId>
                           <ns1:PartNumber>83192289285</ns1:PartNumber>
                           <ns1:DATPartNumber>83192289285</ns1:DATPartNumber>
                           <ns1:Description>REPAIR KIT GLAZING WINDSHIELD</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>60.16</ns1:ValuePerUnit>
                           <ns1:ValueTotal>60.16</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>60.16</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:PartNumber>51317288462</ns1:PartNumber>
                           <ns1:DATPartNumber>51317288462</ns1:DATPartNumber>
                           <ns1:Description>BUFFER</ns1:Description>
                           <ns1:Amount>11</ns1:Amount>
                           <ns1:ValuePerUnit>1.77</ns1:ValuePerUnit>
                           <ns1:ValueTotal>19.47</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>19.47</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:PartNumber>83192211217</ns1:PartNumber>
                           <ns1:DATPartNumber>83192211217</ns1:DATPartNumber>
                           <ns1:Description>CLEANER (100 ML)</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>10.50</ns1:ValuePerUnit>
                           <ns1:ValueTotal>10.50</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>10.50</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:PartNumber>51317288462</ns1:PartNumber>
                           <ns1:DATPartNumber>51317288462</ns1:DATPartNumber>
                           <ns1:Description>BUFFER</ns1:Description>
                           <ns1:Amount>6</ns1:Amount>
                           <ns1:ValuePerUnit>1.77</ns1:ValuePerUnit>
                           <ns1:ValueTotal>10.62</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>10.62</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                     </ns1:MaterialPositions>
                     <ns1:ExtensionPositions>
                        <ns1:ExtensionPosition>
                           <ns1:DATProcessId>45335</ns1:DATProcessId>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:Description>SILICONE FILM RAIN/LIGHT SENSOR</ns1:Description>
                           <ns1:PartsSum>24.62</ns1:PartsSum>
                        </ns1:ExtensionPosition>
                     </ns1:ExtensionPositions>
                     <ns1:LabourPositions>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>44910</ns1:DATProcessId>
                           <ns1:LabourPositionKind>1</ns1:LabourPositionKind>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:LabourPosId>51 31 013</ns1:LabourPosId>
                           <ns1:Description>R+I/REPL. WINDSHIELD
SOUND INSULATION WINDSHIELD COWL, COVER WINDSHIELD TOP</ns1:Description>
                           <ns1:WageType>mechanic</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>33</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>2.75</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>2.75</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:IncludedPositions>
                              <ns1:IncludedPosition>
                                 <ns1:DATProcessId>40270</ns1:DATProcessId>
                                 <ns1:RepairType>replace</ns1:RepairType>
                                 <ns1:Description>SOUND INSULATION WINDSHIELD COWL</ns1:Description>
                              </ns1:IncludedPosition>
                              <ns1:IncludedPosition>
                                 <ns1:DATProcessId>44931</ns1:DATProcessId>
                                 <ns1:RepairType>replace</ns1:RepairType>
                                 <ns1:Description>COVER WINDSHIELD TOP</ns1:Description>
                              </ns1:IncludedPosition>
                           </ns1:IncludedPositions>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>51 31 013</ns1:WorkNumber>
                           <ns1:SparePartNumber>51317333835</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>14449</ns1:DATProcessId>
                           <ns1:LabourPositionKind>4</ns1:LabourPositionKind>
                           <ns1:RepairType>adjust</ns1:RepairType>
                           <ns1:LabourPosId>66 51 525</ns1:LabourPosId>
                           <ns1:Description>CALIBRATE CAMERA DRIVER ASSISTANCE SYSTEMS</ns1:Description>
                           <ns1:WageType>electric</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>4</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>0.33</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>0.33</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>true</ns1:hasRequiredByPosition>
                           <ns1:RequiredByPosition>
                              <ns1:DATProcessId>44910</ns1:DATProcessId>
                              <ns1:RepairType>replace</ns1:RepairType>
                           </ns1:RequiredByPosition>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>66 51 525</ns1:WorkNumber>
                           <ns1:SparePartNumber>66519458736</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                     </ns1:LabourPositions>
                     <ns1:PriceDate>2023-12-01+01:00</ns1:PriceDate>
                     <ns1:RepairCalculationSummary>
                        <ns1:SparePartsCosts>
                           <ns1:AllSum>971.60</ns1:AllSum>
                           <ns1:TotalSum>971.60</ns1:TotalSum>
                        </ns1:SparePartsCosts>
                        <ns1:AuxiliaryCosts/>
                        <ns1:LabourCosts>
                           <ns1:AllSum>3.08</ns1:AllSum>
                           <ns1:Bodywork>
                              <ns1:Type>CAR BODY</ns1:Type>
                              <ns1:Units>0</ns1:Units>
                              <ns1:Price>0</ns1:Price>
                           </ns1:Bodywork>
                           <ns1:Electric>
                              <ns1:Type>ELECTRICS</ns1:Type>
                              <ns1:Units>4.00</ns1:Units>
                              <ns1:PricePerUnit>0.0833</ns1:PricePerUnit>
                              <ns1:Price>0.33</ns1:Price>
                           </ns1:Electric>
                           <ns1:Mechanic>
                              <ns1:Type>MECHANICS</ns1:Type>
                              <ns1:Units>33.00</ns1:Units>
                              <ns1:PricePerUnit>0.0833</ns1:PricePerUnit>
                              <ns1:Price>2.75</ns1:Price>
                           </ns1:Mechanic>
                           <ns1:TotalSum>3.08</ns1:TotalSum>
                           <ns1:Wages/>
                           <ns1:Works>
                              <ns1:Work>
                                 <ns1:Type>ELECTRICS</ns1:Type>
                                 <ns1:WageLevel>1</ns1:WageLevel>
                                 <ns1:Units>4.00</ns1:Units>
                                 <ns1:PricePerUnit>0.0833</ns1:PricePerUnit>
                                 <ns1:Price>0.33</ns1:Price>
                              </ns1:Work>
                              <ns1:Work>
                                 <ns1:Type>MECHANICS</ns1:Type>
                                 <ns1:WageLevel>1</ns1:WageLevel>
                                 <ns1:Units>33.00</ns1:Units>
                                 <ns1:PricePerUnit>0.0833</ns1:PricePerUnit>
                                 <ns1:Price>2.75</ns1:Price>
                              </ns1:Work>
                           </ns1:Works>
                        </ns1:LabourCosts>
                        <ns1:LacquerCosts>
                           <ns1:Material/>
                           <ns1:TotalSum>0.00</ns1:TotalSum>
                        </ns1:LacquerCosts>
                        <ns1:TotalNetCosts>974.68</ns1:TotalNetCosts>
                        <ns1:TotalVAT>185.19</ns1:TotalVAT>
                        <ns1:TotalGrossCosts>1159.87</ns1:TotalGrossCosts>
                        <ns1:TotalNetCorrected>974.68</ns1:TotalNetCorrected>
                        <ns1:TotalVATCorrected>185.19</ns1:TotalVATCorrected>
                        <ns1:TotalGrossCorrected>1159.87</ns1:TotalGrossCorrected>
                        <ns1:SumNet>974.68</ns1:SumNet>
                        <ns1:SumGross>1159.87</ns1:SumGross>
                        <ns1:SumSparePartCosts>971.60</ns1:SumSparePartCosts>
                        <ns1:SumLabourCosts>3.08</ns1:SumLabourCosts>
                        <ns1:MetaPositions>
                           <ns1:MetaPosition key="TOTAL_NET_RISK" value="24.62"/>
                           <ns1:MetaPosition key="VAT_RISK" value="4.68"/>
                           <ns1:MetaPosition key="TOTAL_GROSS_RISK" value="29.30"/>
                           <ns1:MetaPosition key="TIME_UNIT_SYSTEM" value="AW"/>
                           <ns1:MetaPosition key="LACQUER_TIME_UNIT_SYSTEM" value="AW"/>
                           <ns1:MetaPosition key="DAT_EUROLACQUER_IN_HOURS" value="false"/>
                           <ns1:MetaPosition key="TOTAL_PRICE_SPARE_PARTS_RISK" value="24.62"/>
                           <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EQUIPMENT" value="false"/>
                           <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EXTENSION" value="false"/>
                        </ns1:MetaPositions>
                     </ns1:RepairCalculationSummary>
                     <ns1:CalcProtocol>
                        <ns1:ProtocolHints>
                           <ns1:ProtocolHint>
                              <ns1:Identifier>H001</ns1:Identifier>
                              <ns1:Description>series-specific calculation</ns1:Description>
                           </ns1:ProtocolHint>
                        </ns1:ProtocolHints>
                     </ns1:CalcProtocol>
                  </ns1:CalcResultCommon>
                  <ns1:CalcResultExtension>
                     <ns1:MaterialPositions>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>44910</ns1:DATProcessId>
                           <ns1:PartNumber>51317333835</ns1:PartNumber>
                           <ns1:DATPartNumber>51317333835</ns1:DATPartNumber>
                           <ns1:Description>WINDSHIELD</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>797.82</ns1:ValuePerUnit>
                           <ns1:ValueTotal>797.82</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>797.82</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>40270</ns1:DATProcessId>
                           <ns1:PartNumber>51489162739</ns1:PartNumber>
                           <ns1:DATPartNumber>51489162739</ns1:DATPartNumber>
                           <ns1:Description>SOUND INSULATION WINDSHIELD COWL</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>49.34</ns1:ValuePerUnit>
                           <ns1:ValueTotal>49.34</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>49.34</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>44931</ns1:DATProcessId>
                           <ns1:PartNumber>51317203121</ns1:PartNumber>
                           <ns1:DATPartNumber>51317203121</ns1:DATPartNumber>
                           <ns1:Description>COVER WINDSHIELD TOP</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>23.69</ns1:ValuePerUnit>
                           <ns1:ValueTotal>23.69</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>23.69</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>44940</ns1:DATProcessId>
                           <ns1:PartNumber>83192289285</ns1:PartNumber>
                           <ns1:DATPartNumber>83192289285</ns1:DATPartNumber>
                           <ns1:Description>REPAIR KIT GLAZING WINDSHIELD</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>60.16</ns1:ValuePerUnit>
                           <ns1:ValueTotal>60.16</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>60.16</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>45335</ns1:DATProcessId>
                           <ns1:PartNumber>61359856157</ns1:PartNumber>
                           <ns1:DATPartNumber>61359856157</ns1:DATPartNumber>
                           <ns1:Description>SILICONE FILM RAIN/LIGHT SENSOR</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>24.62</ns1:ValuePerUnit>
                           <ns1:ValueTotal>24.62</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>24.62</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:PartNumber>51317288462</ns1:PartNumber>
                           <ns1:DATPartNumber>51317288462</ns1:DATPartNumber>
                           <ns1:Description>BUFFER</ns1:Description>
                           <ns1:Amount>11</ns1:Amount>
                           <ns1:ValuePerUnit>1.77</ns1:ValuePerUnit>
                           <ns1:ValueTotal>19.47</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>19.47</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:PartNumber>83192211217</ns1:PartNumber>
                           <ns1:DATPartNumber>83192211217</ns1:DATPartNumber>
                           <ns1:Description>CLEANER (100 ML)</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>10.50</ns1:ValuePerUnit>
                           <ns1:ValueTotal>10.50</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>10.50</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:PartNumber>51317288462</ns1:PartNumber>
                           <ns1:DATPartNumber>51317288462</ns1:DATPartNumber>
                           <ns1:Description>BUFFER</ns1:Description>
                           <ns1:Amount>6</ns1:Amount>
                           <ns1:ValuePerUnit>1.77</ns1:ValuePerUnit>
                           <ns1:ValueTotal>10.62</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>10.62</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                     </ns1:MaterialPositions>
                     <ns1:LabourPositions>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>44910</ns1:DATProcessId>
                           <ns1:LabourPositionKind>1</ns1:LabourPositionKind>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:LabourPosId>51 31 013</ns1:LabourPosId>
                           <ns1:Description>R+I/REPL. WINDSHIELD
SOUND INSULATION WINDSHIELD COWL, COVER WINDSHIELD TOP</ns1:Description>
                           <ns1:WageType>mechanic</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>33</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>2.75</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>2.75</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:IncludedPositions>
                              <ns1:IncludedPosition>
                                 <ns1:DATProcessId>40270</ns1:DATProcessId>
                                 <ns1:RepairType>replace</ns1:RepairType>
                                 <ns1:Description>SOUND INSULATION WINDSHIELD COWL</ns1:Description>
                              </ns1:IncludedPosition>
                              <ns1:IncludedPosition>
                                 <ns1:DATProcessId>44931</ns1:DATProcessId>
                                 <ns1:RepairType>replace</ns1:RepairType>
                                 <ns1:Description>COVER WINDSHIELD TOP</ns1:Description>
                              </ns1:IncludedPosition>
                           </ns1:IncludedPositions>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>51 31 013</ns1:WorkNumber>
                           <ns1:SparePartNumber>51317333835</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>14449</ns1:DATProcessId>
                           <ns1:LabourPositionKind>4</ns1:LabourPositionKind>
                           <ns1:RepairType>adjust</ns1:RepairType>
                           <ns1:LabourPosId>66 51 525</ns1:LabourPosId>
                           <ns1:Description>CALIBRATE CAMERA DRIVER ASSISTANCE SYSTEMS</ns1:Description>
                           <ns1:WageType>electric</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>4</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>0.33</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>0.33</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>true</ns1:hasRequiredByPosition>
                           <ns1:RequiredByPosition>
                              <ns1:DATProcessId>44910</ns1:DATProcessId>
                              <ns1:RepairType>replace</ns1:RepairType>
                           </ns1:RequiredByPosition>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>66 51 525</ns1:WorkNumber>
                           <ns1:SparePartNumber>66519458736</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                     </ns1:LabourPositions>
                     <ns1:PriceDate>2023-12-01+01:00</ns1:PriceDate>
                     <ns1:RepairCalculationSummary>
                        <ns1:SparePartsCosts>
                           <ns1:AllSum>996.22</ns1:AllSum>
                           <ns1:TotalSum>996.22</ns1:TotalSum>
                        </ns1:SparePartsCosts>
                        <ns1:AuxiliaryCosts/>
                        <ns1:LabourCosts>
                           <ns1:AllSum>3.08</ns1:AllSum>
                           <ns1:Bodywork>
                              <ns1:Type>CAR BODY</ns1:Type>
                              <ns1:Units>0</ns1:Units>
                              <ns1:Price>0</ns1:Price>
                           </ns1:Bodywork>
                           <ns1:Electric>
                              <ns1:Type>ELECTRICS</ns1:Type>
                              <ns1:Units>4.00</ns1:Units>
                              <ns1:PricePerUnit>0.0833</ns1:PricePerUnit>
                              <ns1:Price>0.33</ns1:Price>
                           </ns1:Electric>
                           <ns1:Mechanic>
                              <ns1:Type>MECHANICS</ns1:Type>
                              <ns1:Units>33.00</ns1:Units>
                              <ns1:PricePerUnit>0.0833</ns1:PricePerUnit>
                              <ns1:Price>2.75</ns1:Price>
                           </ns1:Mechanic>
                           <ns1:TotalSum>3.08</ns1:TotalSum>
                           <ns1:Wages/>
                           <ns1:Works>
                              <ns1:Work>
                                 <ns1:Type>ELECTRICS</ns1:Type>
                                 <ns1:WageLevel>1</ns1:WageLevel>
                                 <ns1:Units>4.00</ns1:Units>
                                 <ns1:PricePerUnit>0.0833</ns1:PricePerUnit>
                                 <ns1:Price>0.33</ns1:Price>
                              </ns1:Work>
                              <ns1:Work>
                                 <ns1:Type>MECHANICS</ns1:Type>
                                 <ns1:WageLevel>1</ns1:WageLevel>
                                 <ns1:Units>33.00</ns1:Units>
                                 <ns1:PricePerUnit>0.0833</ns1:PricePerUnit>
                                 <ns1:Price>2.75</ns1:Price>
                              </ns1:Work>
                           </ns1:Works>
                        </ns1:LabourCosts>
                        <ns1:LacquerCosts>
                           <ns1:Material/>
                           <ns1:TotalSum>0.00</ns1:TotalSum>
                        </ns1:LacquerCosts>
                        <ns1:TotalNetCosts>999.30</ns1:TotalNetCosts>
                        <ns1:TotalVAT>189.87</ns1:TotalVAT>
                        <ns1:TotalGrossCosts>1189.17</ns1:TotalGrossCosts>
                        <ns1:TotalNetCorrected>999.30</ns1:TotalNetCorrected>
                        <ns1:TotalVATCorrected>189.87</ns1:TotalVATCorrected>
                        <ns1:TotalGrossCorrected>1189.17</ns1:TotalGrossCorrected>
                        <ns1:SumNet>999.30</ns1:SumNet>
                        <ns1:SumGross>1189.17</ns1:SumGross>
                        <ns1:SumSparePartCosts>996.22</ns1:SumSparePartCosts>
                        <ns1:SumLabourCosts>3.08</ns1:SumLabourCosts>
                        <ns1:MetaPositions>
                           <ns1:MetaPosition key="TIME_UNIT_SYSTEM" value="AW"/>
                           <ns1:MetaPosition key="LACQUER_TIME_UNIT_SYSTEM" value="AW"/>
                           <ns1:MetaPosition key="DAT_EUROLACQUER_IN_HOURS" value="false"/>
                           <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EQUIPMENT" value="false"/>
                           <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EXTENSION" value="false"/>
                        </ns1:MetaPositions>
                     </ns1:RepairCalculationSummary>
                  </ns1:CalcResultExtension>
                  <ns1:CalculationSummary>
                     <ns1:SparePartsCosts>
                        <ns1:AllSum>971.60</ns1:AllSum>
                        <ns1:TotalSum>971.60</ns1:TotalSum>
                     </ns1:SparePartsCosts>
                     <ns1:AuxiliaryCosts/>
                     <ns1:LabourCosts>
                        <ns1:AllSum>3.08</ns1:AllSum>
                        <ns1:Bodywork>
                           <ns1:Type>CAR BODY</ns1:Type>
                           <ns1:Units>0</ns1:Units>
                           <ns1:Price>0</ns1:Price>
                        </ns1:Bodywork>
                        <ns1:Electric>
                           <ns1:Type>ELECTRICS</ns1:Type>
                           <ns1:Units>4.00</ns1:Units>
                           <ns1:PricePerUnit>0.0833</ns1:PricePerUnit>
                           <ns1:Price>0.33</ns1:Price>
                        </ns1:Electric>
                        <ns1:Mechanic>
                           <ns1:Type>MECHANICS</ns1:Type>
                           <ns1:Units>33.00</ns1:Units>
                           <ns1:PricePerUnit>0.0833</ns1:PricePerUnit>
                           <ns1:Price>2.75</ns1:Price>
                        </ns1:Mechanic>
                        <ns1:TotalSum>3.08</ns1:TotalSum>
                        <ns1:Wages/>
                        <ns1:Works>
                           <ns1:Work>
                              <ns1:Type>ELECTRICS</ns1:Type>
                              <ns1:WageLevel>1</ns1:WageLevel>
                              <ns1:Units>4.00</ns1:Units>
                              <ns1:PricePerUnit>0.0833</ns1:PricePerUnit>
                              <ns1:Price>0.33</ns1:Price>
                           </ns1:Work>
                           <ns1:Work>
                              <ns1:Type>MECHANICS</ns1:Type>
                              <ns1:WageLevel>1</ns1:WageLevel>
                              <ns1:Units>33.00</ns1:Units>
                              <ns1:PricePerUnit>0.0833</ns1:PricePerUnit>
                              <ns1:Price>2.75</ns1:Price>
                           </ns1:Work>
                        </ns1:Works>
                     </ns1:LabourCosts>
                     <ns1:LacquerCosts>
                        <ns1:Material/>
                        <ns1:TotalSum>0.00</ns1:TotalSum>
                     </ns1:LacquerCosts>
                     <ns1:TotalNetCosts>974.68</ns1:TotalNetCosts>
                     <ns1:TotalVAT>185.19</ns1:TotalVAT>
                     <ns1:TotalGrossCosts>1159.87</ns1:TotalGrossCosts>
                     <ns1:TotalNetCorrected>974.68</ns1:TotalNetCorrected>
                     <ns1:TotalVATCorrected>185.19</ns1:TotalVATCorrected>
                     <ns1:TotalGrossCorrected>1159.87</ns1:TotalGrossCorrected>
                     <ns1:SumNet>974.68</ns1:SumNet>
                     <ns1:SumGross>1159.87</ns1:SumGross>
                     <ns1:SumSparePartCosts>971.60</ns1:SumSparePartCosts>
                     <ns1:SumLabourCosts>3.08</ns1:SumLabourCosts>
                     <ns1:MetaPositions>
                        <ns1:MetaPosition key="TOTAL_NET_RISK" value="24.62"/>
                        <ns1:MetaPosition key="VAT_RISK" value="4.68"/>
                        <ns1:MetaPosition key="TOTAL_GROSS_RISK" value="29.30"/>
                        <ns1:MetaPosition key="TIME_UNIT_SYSTEM" value="AW"/>
                        <ns1:MetaPosition key="LACQUER_TIME_UNIT_SYSTEM" value="AW"/>
                        <ns1:MetaPosition key="DAT_EUROLACQUER_IN_HOURS" value="false"/>
                        <ns1:MetaPosition key="TOTAL_PRICE_SPARE_PARTS_RISK" value="24.62"/>
                        <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EQUIPMENT" value="false"/>
                        <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EXTENSION" value="false"/>
                     </ns1:MetaPositions>
                  </ns1:CalculationSummary>
                  <ns1:SurchargeSettings/>
                  <ns1:SettingsParameters>
                     <ns1:SettingsParameter key="VIN_AUTOMATIC_EXECUTION" level="company" name="GlobalSettings" value="true"/>
                     <ns1:SettingsParameter key="SHOW_FORD_FINIS_NUMBER" level="company" name="SparePartSettings" value="false"/>
                     <ns1:SettingsParameter key="SPARE_PART_INHERIT_DISCOUNTS" level="company" name="SparePartSettings" value="false"/>
                     <ns1:SettingsParameter key="MANUAL_TIME_IN_HOURS" level="company" name="LabourSettings" value="false"/>
                     <ns1:SettingsParameter key="EURO_LACQUER_IN_HOURS" level="company" name="LacquerSettings" value="false"/>
                  </ns1:SettingsParameters>
               </ns1:RepairCalculation>
               <ns1:RepairOrder>
                  <ns1:OrderNumber>20231222143858376</ns1:OrderNumber>
                  <ns1:InvoiceDate>2023-12-22T14:38:59.392+01:00</ns1:InvoiceDate>
               </ns1:RepairOrder>
               <ns1:InsuranceClaim>false</ns1:InsuranceClaim>
               <ns1:ProcessManagement/>
            </ns1:Dossier>
         </calculationResult>
      </ns10:calculateNResponse>
   </S:Body>
</S:Envelope>
