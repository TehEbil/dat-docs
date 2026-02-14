---
title: "Response getContract"
topic_id: "2458"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abrufen eines bestimmten Vorgangs > Response getContract"
---

# Response getContract

<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns4:getContractResponse xmlns:ns4="http://sphinx.dat.de/services/VehicleRepairService">
         <contractResult source="SD3" type="VehicleRepairOnline">
            <ns1:Dossier xmlns:ns1="http://www.dat.de/vxs">
               <ns1:Description>DAT-TEST_12:04:49,275</ns1:Description>
               <ns1:UUID>8b377208-37db-4e6c-9e0d-bf464abcc517</ns1:UUID>
               <ns1:DossierId>9999999</ns1:DossierId>
               <ns1:IdSD3Network>9999999</ns1:IdSD3Network>
               <ns1:Country>DE</ns1:Country>
               <ns1:Language>de_DE</ns1:Language>
               <ns1:DataVersion>1</ns1:DataVersion>
               <ns1:Currency>EUR</ns1:Currency>
               <ns1:DatCustomerId>111111111</ns1:DatCustomerId>
               <ns1:DossierType>repair</ns1:DossierType>
               <ns1:CreateDate>2023-12-22T12:04:49+01:00</ns1:CreateDate>
               <ns1:CreateUser>Anwender</ns1:CreateUser>
               <ns1:ChangeDate>2023-12-22T12:04:49+01:00</ns1:ChangeDate>
               <ns1:DatCustomerAddress>
                  <ns1:Title>titleCompany</ns1:Title>
                  <ns1:CompanyName>DAT - Intern</ns1:CompanyName>
                  <ns1:NameLong>Schulung SST-Partner</ns1:NameLong>
                  <ns1:Country>DE</ns1:Country>
                  <ns1:CustomerNumber>111111111</ns1:CustomerNumber>
                  <ns1:CustomerType>111111111</ns1:CustomerType>
                  <ns1:Street>Hellmuth-Hirth-Str.</ns1:Street>
                  <ns1:StreetNumber>1</ns1:StreetNumber>
                  <ns1:StreetZipCode>73760</ns1:StreetZipCode>
                  <ns1:StreetCity>Ostfildern</ns1:StreetCity>
                  <ns1:EMail>kundendienst@dat.de</ns1:EMail>
                  <ns1:PhoneBusiness>+49 711/4500000</ns1:PhoneBusiness>
                  <ns1:UsageFlag>9</ns1:UsageFlag>
               </ns1:DatCustomerAddress>
               <ns1:Vehicle>
                  <ns1:VehicleIdentNumber>WBADEXTESTSTUB001</ns1:VehicleIdentNumber>
                  <ns1:DatECode>011301110300002</ns1:DatECode>
                  <ns1:Container>DE006</ns1:Container>
                  <ns1:ConstructionTime>5297</ns1:ConstructionTime>
                  <ns1:InitialRegistration>2013-11-23+01:00</ns1:InitialRegistration>
                  <ns1:MileageEstimated>654321</ns1:MileageEstimated>
                  <ns1:MileageOdometer>654321</ns1:MileageOdometer>
                  <ns1:VehicleTypeName origin="dat">Pkw, SUV, Kleintransporter</ns1:VehicleTypeName>
                  <ns1:VehicleTypeNameN origin="dat">Pkw, SUV, Kleintransporter</ns1:VehicleTypeNameN>
                  <ns1:ManufacturerName origin="dat">BMW</ns1:ManufacturerName>
                  <ns1:BaseModelName origin="dat">Baureihe 5 Touring (F11)(2010->)</ns1:BaseModelName>
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
                  <ns1:RegistrationData>
                     <ns1:LicenseNumber>ES SM1122</ns1:LicenseNumber>
                  </ns1:RegistrationData>
                  <ns1:Engine/>
                  <ns1:TechInfo>
                     <ns1:FillingQuantities>
                        <ns1:Fluid code="N47D20" desc="Motor" type="1">
                           <ns1:Capacity condition="Servicebefüllung" desc="Füllmenge (gesamt)" min="5.20" unit="Liter"/>
                           <ns1:Recommendation>
                              <ns1:Usage type="0">Normal</ns1:Usage>
                              <ns1:Interval type="1">Wechseln 30000 km/ 24 Monate</ns1:Interval>
                              <ns1:Product>TITAN GT1 PRO FLEX SAE 5W-30 (XTL-Technology)</ns1:Product>
                              <ns1:Product>TITAN GT1 PRO C-3 SAE 5W-30 (XTL-Technology)</ns1:Product>
                              <ns1:Product>TITAN GT1 SAE 5W-40 (XTL-Technology)</ns1:Product>
                           </ns1:Recommendation>
                        </ns1:Fluid>
                        <ns1:Fluid desc="Kühlsystem" type="8">
                           <ns1:Capacity desc="Füllmenge (gesamt)" max="7.50" min="7.20" unit="Liter"/>
                           <ns1:Recommendation>
                              <ns1:Usage type="0">Normal</ns1:Usage>
                              <ns1:Product>MAINTAIN FRICOFIN</ns1:Product>
                           </ns1:Recommendation>
                        </ns1:Fluid>
                        <ns1:Fluid code="205AL" desc="Hinterachsgetriebe" type="3">
                           <ns1:Capacity desc="Füllmenge (gesamt)" min="0.80" unit="Liter"/>
                           <ns1:Recommendation>
                              <ns1:Usage type="0">Normal</ns1:Usage>
                              <ns1:Product>TITAN SINTOPOID LS SAE 75W-90</ns1:Product>
                           </ns1:Recommendation>
                        </ns1:Fluid>
                        <ns1:Fluid code="ZF GA8HP 8/1" desc="Automatikgetriebe" type="3">
                           <ns1:Capacity desc="Füllmenge (gesamt)" min="8.50" unit="Liter"/>
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
                           <ns1:Description>Airbag Beifahrerseite abschaltbar</ns1:Description>
                           <ns1:EquipmentGroup>AIR2</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26803</ns1:DatEquipmentId>
                           <ns1:Description>Airbag Fahrer-/Beifahrerseite</ns1:Description>
                           <ns1:EquipmentGroup>AIR1</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>34704</ns1:DatEquipmentId>
                           <ns1:Description>Aktive Kopfstützen</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>10715</ns1:DatEquipmentId>
                           <ns1:Description>Aktive Motorhaube</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40000</ns1:DatEquipmentId>
                           <ns1:Description>Anti-Blockier-System (ABS)</ns1:Description>
                           <ns1:EquipmentGroup>ABS</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18604</ns1:DatEquipmentId>
                           <ns1:Description>Automatische Fahrlichtschaltung</ns1:Description>
                           <ns1:EquipmentGroup>AUFL</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>24999</ns1:DatEquipmentId>
                           <ns1:Description>AUX-IN-Anschluss (AUX-IN)</ns1:Description>
                           <ns1:EquipmentGroup>MP3A</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>15200</ns1:DatEquipmentId>
                           <ns1:Description>Außenspiegel elektr. verstell- und heizbar</ns1:Description>
                           <ns1:EquipmentGroup>AUSP</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25702</ns1:DatEquipmentId>
                           <ns1:Description>Außentemperaturanzeige</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18505</ns1:DatEquipmentId>
                           <ns1:Description>Bi-Xenon-Scheinwerfer</ns1:Description>
                           <ns1:EquipmentGroup>XELI</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>19000</ns1:DatEquipmentId>
                                 <ns1:Description>Scheinwerfer-Reinigungsanlage (SRA)</ns1:Description>
                                 <ns1:EquipmentGroup>SWRA</ns1:EquipmentGroup>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>18913</ns1:DatEquipmentId>
                                 <ns1:Description>Tagfahrlicht LED</ns1:Description>
                                 <ns1:EquipmentGroup>TFAL</ns1:EquipmentGroup>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>18940</ns1:DatEquipmentId>
                                 <ns1:Description>Blinkleuchten LED</ns1:Description>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25508</ns1:DatEquipmentId>
                           <ns1:Description>Bordcomputer</ns1:Description>
                           <ns1:EquipmentGroup>COMP</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40801</ns1:DatEquipmentId>
                           <ns1:Description>Bremsassistent</ns1:Description>
                           <ns1:EquipmentGroup>FA01</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40050</ns1:DatEquipmentId>
                           <ns1:Description>Bremsenergierückgewinnung (Rekuperationssystem)</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25606</ns1:DatEquipmentId>
                           <ns1:Description>Check-Control-System</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25300</ns1:DatEquipmentId>
                           <ns1:Description>Drehzahlmesser</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18898</ns1:DatEquipmentId>
                           <ns1:Description>Dynamische Bremsleuchte</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>70100</ns1:DatEquipmentId>
                           <ns1:Description>Dynamische Stabilitäts-Control (DSC)</ns1:Description>
                           <ns1:EquipmentGroup>ESP</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>11406</ns1:DatEquipmentId>
                           <ns1:Description>Exterieurumfänge Wagenfarbe</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>70518</ns1:DatEquipmentId>
                           <ns1:Description>Fahrassistenz-System: Fahrerlebnisschalter</ns1:Description>
                           <ns1:EquipmentGroup>FA22</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35003</ns1:DatEquipmentId>
                           <ns1:Description>Fensterheber elektrisch vorn + hinten</ns1:Description>
                           <ns1:EquipmentGroup>FH4</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>24833</ns1:DatEquipmentId>
                           <ns1:Description>Freisprecheinrichtung mit USB-Schnittstelle</ns1:Description>
                           <ns1:EquipmentGroup>TEL3</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>28402</ns1:DatEquipmentId>
                           <ns1:Description>Fußmatten Velours</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27605</ns1:DatEquipmentId>
                           <ns1:Description>Gepäckraum-Abtrennung (Netz)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27400</ns1:DatEquipmentId>
                           <ns1:Description>Gepäckraumabdeckung / Rollo</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26710</ns1:DatEquipmentId>
                           <ns1:Description>Geschwindigkeits-Regelanlage mit Bremsfunktion</ns1:Description>
                           <ns1:EquipmentGroup>TEMP</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39402</ns1:DatEquipmentId>
                           <ns1:Description>Getränkehalter vorn und hinten</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35506</ns1:DatEquipmentId>
                           <ns1:Description>Heckklappenbetätigung automatisch</ns1:Description>
                           <ns1:EquipmentGroup>HKEL</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>19300</ns1:DatEquipmentId>
                           <ns1:Description>Heckscheibenwischer</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39308</ns1:DatEquipmentId>
                           <ns1:Description>Isofix-Aufnahmen für Kindersitz an Rücksitz</ns1:Description>
                           <ns1:EquipmentGroup>KISI</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                           <ns1:Description>Karosserie: 5-türig</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26805</ns1:DatEquipmentId>
                           <ns1:Description>Kopf-Airbag-System hinten</ns1:Description>
                           <ns1:EquipmentGroup>AIR4</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26804</ns1:DatEquipmentId>
                           <ns1:Description>Kopf-Airbag-System vorn</ns1:Description>
                           <ns1:EquipmentGroup>AIR4</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>69007</ns1:DatEquipmentId>
                           <ns1:Description>Lenkrad (Leder) mit Multifunktion</ns1:Description>
                           <ns1:EquipmentGroup>LEN2</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>69505</ns1:DatEquipmentId>
                                 <ns1:Description>Lenksäule (Lenkrad) mechan. verstellbar</ns1:Description>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>69505</ns1:DatEquipmentId>
                           <ns1:Description>Lenksäule (Lenkrad) mechan. verstellbar</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>48535</ns1:DatEquipmentId>
                           <ns1:Description>LM-Felgen 8x17 (V-Speiche 236)</ns1:Description>
                           <ns1:EquipmentGroup>ALU</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>42905</ns1:DatEquipmentId>
                           <ns1:Description>Luftfederung Hinterachse</ns1:Description>
                           <ns1:EquipmentGroup>LUFT</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>42805</ns1:DatEquipmentId>
                                 <ns1:Description>Niveauregulierung</ns1:Description>
                                 <ns1:EquipmentGroup>NIV</ns1:EquipmentGroup>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27300</ns1:DatEquipmentId>
                           <ns1:Description>Mittelarmlehne hinten</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27202</ns1:DatEquipmentId>
                           <ns1:Description>Mittelarmlehne vorn</ns1:Description>
                           <ns1:EquipmentGroup>MALV</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>87410</ns1:DatEquipmentId>
                           <ns1:Description>Motor 2,0 Ltr. - 135 kW Turbodiesel KAT (N 47 T)</ns1:Description>
                           <ns1:EquipmentType>engine</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>96508</ns1:DatEquipmentId>
                                 <ns1:Description>Motor 2,0 Ltr. - 135 kW Turbodiesel</ns1:Description>
                                 <ns1:EquipmentType>engine</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27309</ns1:DatEquipmentId>
                           <ns1:Description>Multifunktionsarmlehne im Fond</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>42805</ns1:DatEquipmentId>
                           <ns1:Description>Niveauregulierung</ns1:Description>
                           <ns1:EquipmentGroup>NIV</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>77015</ns1:DatEquipmentId>
                           <ns1:Description>NOx-Speicherkatalysator (BMW Blue Performance)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40803</ns1:DatEquipmentId>
                           <ns1:Description>Parkbremse elektrisch</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>62004</ns1:DatEquipmentId>
                           <ns1:Description>Reifen 225/55 R17 ..Z</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>68802</ns1:DatEquipmentId>
                           <ns1:Description>Reifen-Reparaturset (Mobility-Pack)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25906</ns1:DatEquipmentId>
                           <ns1:Description>Reifenpannen-Anzeige</ns1:Description>
                           <ns1:EquipmentGroup>RDK</ns1:EquipmentGroup>
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
                           <ns1:DatEquipmentId>33508</ns1:DatEquipmentId>
                           <ns1:Description>Rücksitzlehne geteilt/klappbar</ns1:Description>
                           <ns1:EquipmentGroup>SITH</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>77227</ns1:DatEquipmentId>
                           <ns1:Description>Schadstoffarm nach Abgasnorm Euro 6</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>19102</ns1:DatEquipmentId>
                           <ns1:Description>Scheibenwaschdüsen heizbar</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>19101</ns1:DatEquipmentId>
                           <ns1:Description>Scheibenwischer mit Regensensor</ns1:Description>
                           <ns1:EquipmentGroup>SWRE</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>19000</ns1:DatEquipmentId>
                           <ns1:Description>Scheinwerfer-Reinigungsanlage (SRA)</ns1:Description>
                           <ns1:EquipmentGroup>SWRA</ns1:EquipmentGroup>
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
                           <ns1:DatEquipmentId>25151</ns1:DatEquipmentId>
                           <ns1:Description>Service-System: Intelligenter Notruf inkl. TeleServices</ns1:Description>
                           <ns1:EquipmentGroup>FA10</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>69811</ns1:DatEquipmentId>
                           <ns1:Description>Servolenkung Servotronic</ns1:Description>
                           <ns1:EquipmentGroup>SL</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>32811</ns1:DatEquipmentId>
                           <ns1:Description>Sitze vorn teilelektr. verstellbar</ns1:Description>
                           <ns1:EquipmentGroup>SITE</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35408</ns1:DatEquipmentId>
                           <ns1:Description>Soft-Close-Automatik für Kofferraum / Heckklappe</ns1:Description>
                           <ns1:EquipmentGroup>HKEL</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35513</ns1:DatEquipmentId>
                           <ns1:Description>Start-Stop-Knopf</ns1:Description>
                           <ns1:EquipmentGroup>MSSA</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>77601</ns1:DatEquipmentId>
                           <ns1:Description>Start/Stop-Anlage (Funktion)</ns1:Description>
                           <ns1:EquipmentGroup>MSSA</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39016</ns1:DatEquipmentId>
                           <ns1:Description>Steckdose (12V-Anschluß) 3-fach</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>73017</ns1:DatEquipmentId>
                           <ns1:Description>Vlies-Batterie 80 Ah (AGM)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>38105</ns1:DatEquipmentId>
                           <ns1:Description>Wegfahrsperre</ns1:Description>
                           <ns1:EquipmentGroup>WFS</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>22218</ns1:DatEquipmentId>
                           <ns1:Description>Wärme-/Sonnenschutzverglasung kombiniert (hinten abgedunkelt)</ns1:Description>
                           <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
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
                           <ns1:DatEquipmentId>96508</ns1:DatEquipmentId>
                           <ns1:Description>Motor 2,0 Ltr. - 135 kW Turbodiesel</ns1:Description>
                           <ns1:EquipmentType>engine</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18913</ns1:DatEquipmentId>
                           <ns1:Description>Tagfahrlicht LED</ns1:Description>
                           <ns1:EquipmentGroup>TFAL</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18940</ns1:DatEquipmentId>
                           <ns1:Description>Blinkleuchten LED</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                     </ns1:SeriesEquipment>
                     <ns1:SpecialEquipment>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>37603</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Ambiente-Beleuchtung</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25804</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Audio-Navigationssystem Professional</ns1:Description>
                           <ns1:EquipmentGroup>GPS</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>24709</ns1:DatEquipmentId>
                                 <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                 <ns1:Description>Sprachbediensystem</ns1:Description>
                                 <ns1:EquipmentGroup>TEL4</ns1:EquipmentGroup>
                                 <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>8702</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Außenausstattung: Shadow-Line Hochglanz</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25930</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Control-Display mit Farbmonitor (9,2 Zoll)</ns1:Description>
                           <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27810</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Dachhimmel Anthrazit (BMW Individual)</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>16198</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Dachreling Hochglanz Shadow-Line</ns1:Description>
                           <ns1:EquipmentGroup>DARE</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25704</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Fahrassistenz-System: Speed-Limit-Anzeige</ns1:Description>
                           <ns1:EquipmentGroup>FA28</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>22505</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Frontscheibe (Ausführung: Klimakomfort)</ns1:Description>
                           <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>75914</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Getriebe Automatik - mit Steptronic (8-Stufen)</ns1:Description>
                           <ns1:EquipmentGroup>AG2</ns1:EquipmentGroup>
                           <ns1:GearBoxType>automatic</ns1:GearBoxType>
                           <ns1:NrOfGears>8</ns1:NrOfGears>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25204</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Head-up-Display</ns1:Description>
                           <ns1:EquipmentGroup>HUD</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>25930</ns1:DatEquipmentId>
                                 <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                 <ns1:Description>Control-Display mit Farbmonitor (9,2 Zoll)</ns1:Description>
                                 <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>25413</ns1:DatEquipmentId>
                                 <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                 <ns1:Description>Instrumentenkombination (erweiterter Umfang)</ns1:Description>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>24607</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>HiFi-Lautsprechersystem</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>31408</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Innenausstattung: Interieurleisten Aluminium Längsschliff fein</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>37901</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Innenspiegel mit Abblendautomatik</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25413</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Instrumentenkombination (erweiterter Umfang)</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>25930</ns1:DatEquipmentId>
                                 <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                 <ns1:Description>Control-Display mit Farbmonitor (9,2 Zoll)</ns1:Description>
                                 <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>28982</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Klimaautomatik 2-Zonen mit autom. Umluft-Control, erweiterter Umfang</ns1:Description>
                           <ns1:EquipmentGroup>KLI2</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>33403</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Lendenwirbelstütze Sitz vorn links und rechts, elektr. verstellbar</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>77240</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Modellvariante CO2-Umfang (Code 1CB)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18313</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Nebelscheinwerfer LED</ns1:Description>
                           <ns1:EquipmentGroup>BEL</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>16302</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Panoramadach (Glas)</ns1:Description>
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
                           <ns1:Description>Sitzbezug / Polsterung: Leder Dakota</ns1:Description>
                           <ns1:EquipmentGroup>LEDE</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>29500</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Sitzheizung vorn</ns1:Description>
                           <ns1:EquipmentGroup>SITB</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>22102</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Sonnenschutzverglasung (hinten abgedunkelt, BMW Individual)</ns1:Description>
                           <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>24709</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Sprachbediensystem</ns1:Description>
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
                        <ns1:Description>Motor 2,0 Ltr. - 135 kW Turbodiesel</ns1:Description>
                        <ns1:EquipmentClass>1</ns1:EquipmentClass>
                     </ns1:EquipmentPosition>
                     <ns1:EquipmentPosition>
                        <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                        <ns1:Description>Karosserie: 5-türig</ns1:Description>
                        <ns1:EquipmentClass>2</ns1:EquipmentClass>
                     </ns1:EquipmentPosition>
                     <ns1:EquipmentPosition>
                        <ns1:DatEquipmentId>75914</ns1:DatEquipmentId>
                        <ns1:Description>Getriebe Automatik - mit Steptronic (8-Stufen)</ns1:Description>
                        <ns1:EquipmentClass>11</ns1:EquipmentClass>
                     </ns1:EquipmentPosition>
                  </ns1:DATECodeEquipment>
               </ns1:Vehicle>
               <ns1:VAT>
                  <ns1:VatAtCalculationTime>19</ns1:VatAtCalculationTime>
               </ns1:VAT>
               <ns1:TradingData>
                  <ns1:Owner>
                     <ns1:Title>titleMrs</ns1:Title>
                     <ns1:TitleEntry>Frau</ns1:TitleEntry>
                     <ns1:LastName>Max</ns1:LastName>
                     <ns1:FirstName>Musterfrau</ns1:FirstName>
                     <ns1:Country>DE</ns1:Country>
                     <ns1:UsageFlag>2</ns1:UsageFlag>
                  </ns1:Owner>
                  <ns1:ClientContactAddresses>
                     <ns1:ClientContactAddress>
                        <ns1:Title>titleCompany</ns1:Title>
                        <ns1:CompanyName>DAT - Intern</ns1:CompanyName>
                        <ns1:NameLong>Schulung SST-Partner</ns1:NameLong>
                        <ns1:Country>DE</ns1:Country>
                        <ns1:CustomerNumber>111111111</ns1:CustomerNumber>
                        <ns1:CustomerType>111111111</ns1:CustomerType>
                        <ns1:Street>Hellmuth-Hirth-Str.</ns1:Street>
                        <ns1:StreetNumber>1</ns1:StreetNumber>
                        <ns1:StreetZipCode>73760</ns1:StreetZipCode>
                        <ns1:StreetCity>Ostfildern</ns1:StreetCity>
                        <ns1:EMail>kundendienst@dat.de</ns1:EMail>
                        <ns1:PhoneBusiness>+49 711/450000</ns1:PhoneBusiness>
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
                     <ns1:InitialRegistration>2013-11-23+01:00</ns1:InitialRegistration>
                     <ns1:MileageEstimated>654321</ns1:MileageEstimated>
                     <ns1:MileageOdometer>654321</ns1:MileageOdometer>
                     <ns1:VehicleTypeName origin="dat">Pkw, SUV, Kleintransporter</ns1:VehicleTypeName>
                     <ns1:VehicleTypeNameN origin="dat">Pkw, SUV, Kleintransporter</ns1:VehicleTypeNameN>
                     <ns1:ManufacturerName origin="dat">BMW</ns1:ManufacturerName>
                     <ns1:BaseModelName origin="dat">Baureihe 5 Touring (F11)(2010->)</ns1:BaseModelName>
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
                     <ns1:RegistrationData>
                        <ns1:LicenseNumber>ES SM1122</ns1:LicenseNumber>
                     </ns1:RegistrationData>
                     <ns1:Engine/>
                     <ns1:TechInfo>
                        <ns1:FillingQuantities>
                           <ns1:Fluid code="N47D20" desc="Motor" type="1">
                              <ns1:Capacity condition="Servicebefüllung" desc="Füllmenge (gesamt)" min="5.20" unit="Liter"/>
                              <ns1:Recommendation>
                                 <ns1:Usage type="0">Normal</ns1:Usage>
                                 <ns1:Interval type="1">Wechseln 30000 km/ 24 Monate</ns1:Interval>
                                 <ns1:Product>TITAN GT1 PRO FLEX SAE 5W-30 (XTL-Technology)</ns1:Product>
                                 <ns1:Product>TITAN GT1 PRO C-3 SAE 5W-30 (XTL-Technology)</ns1:Product>
                                 <ns1:Product>TITAN GT1 SAE 5W-40 (XTL-Technology)</ns1:Product>
                              </ns1:Recommendation>
                           </ns1:Fluid>
                           <ns1:Fluid desc="Kühlsystem" type="8">
                              <ns1:Capacity desc="Füllmenge (gesamt)" max="7.50" min="7.20" unit="Liter"/>
                              <ns1:Recommendation>
                                 <ns1:Usage type="0">Normal</ns1:Usage>
                                 <ns1:Product>MAINTAIN FRICOFIN</ns1:Product>
                              </ns1:Recommendation>
                           </ns1:Fluid>
                           <ns1:Fluid code="205AL" desc="Hinterachsgetriebe" type="3">
                              <ns1:Capacity desc="Füllmenge (gesamt)" min="0.80" unit="Liter"/>
                              <ns1:Recommendation>
                                 <ns1:Usage type="0">Normal</ns1:Usage>
                                 <ns1:Product>TITAN SINTOPOID LS SAE 75W-90</ns1:Product>
                              </ns1:Recommendation>
                           </ns1:Fluid>
                           <ns1:Fluid code="ZF GA8HP 8/1" desc="Automatikgetriebe" type="3">
                              <ns1:Capacity desc="Füllmenge (gesamt)" min="8.50" unit="Liter"/>
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
                              <ns1:Description>Airbag Beifahrerseite abschaltbar</ns1:Description>
                              <ns1:EquipmentGroup>AIR2</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>26803</ns1:DatEquipmentId>
                              <ns1:Description>Airbag Fahrer-/Beifahrerseite</ns1:Description>
                              <ns1:EquipmentGroup>AIR1</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>34704</ns1:DatEquipmentId>
                              <ns1:Description>Aktive Kopfstützen</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>10715</ns1:DatEquipmentId>
                              <ns1:Description>Aktive Motorhaube</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>40000</ns1:DatEquipmentId>
                              <ns1:Description>Anti-Blockier-System (ABS)</ns1:Description>
                              <ns1:EquipmentGroup>ABS</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>18604</ns1:DatEquipmentId>
                              <ns1:Description>Automatische Fahrlichtschaltung</ns1:Description>
                              <ns1:EquipmentGroup>AUFL</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>24999</ns1:DatEquipmentId>
                              <ns1:Description>AUX-IN-Anschluss (AUX-IN)</ns1:Description>
                              <ns1:EquipmentGroup>MP3A</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>15200</ns1:DatEquipmentId>
                              <ns1:Description>Außenspiegel elektr. verstell- und heizbar</ns1:Description>
                              <ns1:EquipmentGroup>AUSP</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25702</ns1:DatEquipmentId>
                              <ns1:Description>Außentemperaturanzeige</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>18505</ns1:DatEquipmentId>
                              <ns1:Description>Bi-Xenon-Scheinwerfer</ns1:Description>
                              <ns1:EquipmentGroup>XELI</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>19000</ns1:DatEquipmentId>
                                    <ns1:Description>Scheinwerfer-Reinigungsanlage (SRA)</ns1:Description>
                                    <ns1:EquipmentGroup>SWRA</ns1:EquipmentGroup>
                                    <ns1:EquipmentType>glass</ns1:EquipmentType>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>18913</ns1:DatEquipmentId>
                                    <ns1:Description>Tagfahrlicht LED</ns1:Description>
                                    <ns1:EquipmentGroup>TFAL</ns1:EquipmentGroup>
                                    <ns1:EquipmentType>glass</ns1:EquipmentType>
                                    <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>18940</ns1:DatEquipmentId>
                                    <ns1:Description>Blinkleuchten LED</ns1:Description>
                                    <ns1:EquipmentType>glass</ns1:EquipmentType>
                                    <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25508</ns1:DatEquipmentId>
                              <ns1:Description>Bordcomputer</ns1:Description>
                              <ns1:EquipmentGroup>COMP</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>40801</ns1:DatEquipmentId>
                              <ns1:Description>Bremsassistent</ns1:Description>
                              <ns1:EquipmentGroup>FA01</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>40050</ns1:DatEquipmentId>
                              <ns1:Description>Bremsenergierückgewinnung (Rekuperationssystem)</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25606</ns1:DatEquipmentId>
                              <ns1:Description>Check-Control-System</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25300</ns1:DatEquipmentId>
                              <ns1:Description>Drehzahlmesser</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>18898</ns1:DatEquipmentId>
                              <ns1:Description>Dynamische Bremsleuchte</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>70100</ns1:DatEquipmentId>
                              <ns1:Description>Dynamische Stabilitäts-Control (DSC)</ns1:Description>
                              <ns1:EquipmentGroup>ESP</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>11406</ns1:DatEquipmentId>
                              <ns1:Description>Exterieurumfänge Wagenfarbe</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>70518</ns1:DatEquipmentId>
                              <ns1:Description>Fahrassistenz-System: Fahrerlebnisschalter</ns1:Description>
                              <ns1:EquipmentGroup>FA22</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>35003</ns1:DatEquipmentId>
                              <ns1:Description>Fensterheber elektrisch vorn + hinten</ns1:Description>
                              <ns1:EquipmentGroup>FH4</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>24833</ns1:DatEquipmentId>
                              <ns1:Description>Freisprecheinrichtung mit USB-Schnittstelle</ns1:Description>
                              <ns1:EquipmentGroup>TEL3</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>28402</ns1:DatEquipmentId>
                              <ns1:Description>Fußmatten Velours</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27605</ns1:DatEquipmentId>
                              <ns1:Description>Gepäckraum-Abtrennung (Netz)</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27400</ns1:DatEquipmentId>
                              <ns1:Description>Gepäckraumabdeckung / Rollo</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>26710</ns1:DatEquipmentId>
                              <ns1:Description>Geschwindigkeits-Regelanlage mit Bremsfunktion</ns1:Description>
                              <ns1:EquipmentGroup>TEMP</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>39402</ns1:DatEquipmentId>
                              <ns1:Description>Getränkehalter vorn und hinten</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>35506</ns1:DatEquipmentId>
                              <ns1:Description>Heckklappenbetätigung automatisch</ns1:Description>
                              <ns1:EquipmentGroup>HKEL</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>19300</ns1:DatEquipmentId>
                              <ns1:Description>Heckscheibenwischer</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>39308</ns1:DatEquipmentId>
                              <ns1:Description>Isofix-Aufnahmen für Kindersitz an Rücksitz</ns1:Description>
                              <ns1:EquipmentGroup>KISI</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                              <ns1:Description>Karosserie: 5-türig</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>26805</ns1:DatEquipmentId>
                              <ns1:Description>Kopf-Airbag-System hinten</ns1:Description>
                              <ns1:EquipmentGroup>AIR4</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>26804</ns1:DatEquipmentId>
                              <ns1:Description>Kopf-Airbag-System vorn</ns1:Description>
                              <ns1:EquipmentGroup>AIR4</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>69007</ns1:DatEquipmentId>
                              <ns1:Description>Lenkrad (Leder) mit Multifunktion</ns1:Description>
                              <ns1:EquipmentGroup>LEN2</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>69505</ns1:DatEquipmentId>
                                    <ns1:Description>Lenksäule (Lenkrad) mechan. verstellbar</ns1:Description>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>69505</ns1:DatEquipmentId>
                              <ns1:Description>Lenksäule (Lenkrad) mechan. verstellbar</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>48535</ns1:DatEquipmentId>
                              <ns1:Description>LM-Felgen 8x17 (V-Speiche 236)</ns1:Description>
                              <ns1:EquipmentGroup>ALU</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>42905</ns1:DatEquipmentId>
                              <ns1:Description>Luftfederung Hinterachse</ns1:Description>
                              <ns1:EquipmentGroup>LUFT</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>42805</ns1:DatEquipmentId>
                                    <ns1:Description>Niveauregulierung</ns1:Description>
                                    <ns1:EquipmentGroup>NIV</ns1:EquipmentGroup>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27300</ns1:DatEquipmentId>
                              <ns1:Description>Mittelarmlehne hinten</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27202</ns1:DatEquipmentId>
                              <ns1:Description>Mittelarmlehne vorn</ns1:Description>
                              <ns1:EquipmentGroup>MALV</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>87410</ns1:DatEquipmentId>
                              <ns1:Description>Motor 2,0 Ltr. - 135 kW Turbodiesel KAT (N 47 T)</ns1:Description>
                              <ns1:EquipmentType>engine</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>96508</ns1:DatEquipmentId>
                                    <ns1:Description>Motor 2,0 Ltr. - 135 kW Turbodiesel</ns1:Description>
                                    <ns1:EquipmentType>engine</ns1:EquipmentType>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27309</ns1:DatEquipmentId>
                              <ns1:Description>Multifunktionsarmlehne im Fond</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>42805</ns1:DatEquipmentId>
                              <ns1:Description>Niveauregulierung</ns1:Description>
                              <ns1:EquipmentGroup>NIV</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>77015</ns1:DatEquipmentId>
                              <ns1:Description>NOx-Speicherkatalysator (BMW Blue Performance)</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>40803</ns1:DatEquipmentId>
                              <ns1:Description>Parkbremse elektrisch</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>62004</ns1:DatEquipmentId>
                              <ns1:Description>Reifen 225/55 R17 ..Z</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>68802</ns1:DatEquipmentId>
                              <ns1:Description>Reifen-Reparaturset (Mobility-Pack)</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25906</ns1:DatEquipmentId>
                              <ns1:Description>Reifenpannen-Anzeige</ns1:Description>
                              <ns1:EquipmentGroup>RDK</ns1:EquipmentGroup>
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
                              <ns1:DatEquipmentId>33508</ns1:DatEquipmentId>
                              <ns1:Description>Rücksitzlehne geteilt/klappbar</ns1:Description>
                              <ns1:EquipmentGroup>SITH</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>77227</ns1:DatEquipmentId>
                              <ns1:Description>Schadstoffarm nach Abgasnorm Euro 6</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>19102</ns1:DatEquipmentId>
                              <ns1:Description>Scheibenwaschdüsen heizbar</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>19101</ns1:DatEquipmentId>
                              <ns1:Description>Scheibenwischer mit Regensensor</ns1:Description>
                              <ns1:EquipmentGroup>SWRE</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>19000</ns1:DatEquipmentId>
                              <ns1:Description>Scheinwerfer-Reinigungsanlage (SRA)</ns1:Description>
                              <ns1:EquipmentGroup>SWRA</ns1:EquipmentGroup>
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
                              <ns1:DatEquipmentId>25151</ns1:DatEquipmentId>
                              <ns1:Description>Service-System: Intelligenter Notruf inkl. TeleServices</ns1:Description>
                              <ns1:EquipmentGroup>FA10</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>69811</ns1:DatEquipmentId>
                              <ns1:Description>Servolenkung Servotronic</ns1:Description>
                              <ns1:EquipmentGroup>SL</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>32811</ns1:DatEquipmentId>
                              <ns1:Description>Sitze vorn teilelektr. verstellbar</ns1:Description>
                              <ns1:EquipmentGroup>SITE</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>35408</ns1:DatEquipmentId>
                              <ns1:Description>Soft-Close-Automatik für Kofferraum / Heckklappe</ns1:Description>
                              <ns1:EquipmentGroup>HKEL</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>35513</ns1:DatEquipmentId>
                              <ns1:Description>Start-Stop-Knopf</ns1:Description>
                              <ns1:EquipmentGroup>MSSA</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>77601</ns1:DatEquipmentId>
                              <ns1:Description>Start/Stop-Anlage (Funktion)</ns1:Description>
                              <ns1:EquipmentGroup>MSSA</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>39016</ns1:DatEquipmentId>
                              <ns1:Description>Steckdose (12V-Anschluß) 3-fach</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>73017</ns1:DatEquipmentId>
                              <ns1:Description>Vlies-Batterie 80 Ah (AGM)</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>38105</ns1:DatEquipmentId>
                              <ns1:Description>Wegfahrsperre</ns1:Description>
                              <ns1:EquipmentGroup>WFS</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>22218</ns1:DatEquipmentId>
                              <ns1:Description>Wärme-/Sonnenschutzverglasung kombiniert (hinten abgedunkelt)</ns1:Description>
                              <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
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
                              <ns1:DatEquipmentId>96508</ns1:DatEquipmentId>
                              <ns1:Description>Motor 2,0 Ltr. - 135 kW Turbodiesel</ns1:Description>
                              <ns1:EquipmentType>engine</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>18913</ns1:DatEquipmentId>
                              <ns1:Description>Tagfahrlicht LED</ns1:Description>
                              <ns1:EquipmentGroup>TFAL</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>18940</ns1:DatEquipmentId>
                              <ns1:Description>Blinkleuchten LED</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                        </ns1:SeriesEquipment>
                        <ns1:SpecialEquipment>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>37603</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Ambiente-Beleuchtung</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25804</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Audio-Navigationssystem Professional</ns1:Description>
                              <ns1:EquipmentGroup>GPS</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>24709</ns1:DatEquipmentId>
                                    <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                    <ns1:Description>Sprachbediensystem</ns1:Description>
                                    <ns1:EquipmentGroup>TEL4</ns1:EquipmentGroup>
                                    <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>8702</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Außenausstattung: Shadow-Line Hochglanz</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25930</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Control-Display mit Farbmonitor (9,2 Zoll)</ns1:Description>
                              <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27810</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Dachhimmel Anthrazit (BMW Individual)</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>16198</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Dachreling Hochglanz Shadow-Line</ns1:Description>
                              <ns1:EquipmentGroup>DARE</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25704</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Fahrassistenz-System: Speed-Limit-Anzeige</ns1:Description>
                              <ns1:EquipmentGroup>FA28</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>22505</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Frontscheibe (Ausführung: Klimakomfort)</ns1:Description>
                              <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>75914</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Getriebe Automatik - mit Steptronic (8-Stufen)</ns1:Description>
                              <ns1:EquipmentGroup>AG2</ns1:EquipmentGroup>
                              <ns1:GearBoxType>automatic</ns1:GearBoxType>
                              <ns1:NrOfGears>8</ns1:NrOfGears>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25204</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Head-up-Display</ns1:Description>
                              <ns1:EquipmentGroup>HUD</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>25930</ns1:DatEquipmentId>
                                    <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                    <ns1:Description>Control-Display mit Farbmonitor (9,2 Zoll)</ns1:Description>
                                    <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                                    <ns1:EquipmentType>glass</ns1:EquipmentType>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>25413</ns1:DatEquipmentId>
                                    <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                    <ns1:Description>Instrumentenkombination (erweiterter Umfang)</ns1:Description>
                                    <ns1:EquipmentType>glass</ns1:EquipmentType>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>24607</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>HiFi-Lautsprechersystem</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>31408</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Innenausstattung: Interieurleisten Aluminium Längsschliff fein</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>37901</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Innenspiegel mit Abblendautomatik</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25413</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Instrumentenkombination (erweiterter Umfang)</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>25930</ns1:DatEquipmentId>
                                    <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                    <ns1:Description>Control-Display mit Farbmonitor (9,2 Zoll)</ns1:Description>
                                    <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                                    <ns1:EquipmentType>glass</ns1:EquipmentType>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>28982</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Klimaautomatik 2-Zonen mit autom. Umluft-Control, erweiterter Umfang</ns1:Description>
                              <ns1:EquipmentGroup>KLI2</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>33403</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Lendenwirbelstütze Sitz vorn links und rechts, elektr. verstellbar</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>77240</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Modellvariante CO2-Umfang (Code 1CB)</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>18313</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Nebelscheinwerfer LED</ns1:Description>
                              <ns1:EquipmentGroup>BEL</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>16302</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Panoramadach (Glas)</ns1:Description>
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
                              <ns1:Description>Sitzbezug / Polsterung: Leder Dakota</ns1:Description>
                              <ns1:EquipmentGroup>LEDE</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>29500</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Sitzheizung vorn</ns1:Description>
                              <ns1:EquipmentGroup>SITB</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>22102</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Sonnenschutzverglasung (hinten abgedunkelt, BMW Individual)</ns1:Description>
                              <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>24709</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Sprachbediensystem</ns1:Description>
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
                           <ns1:Description>Motor 2,0 Ltr. - 135 kW Turbodiesel</ns1:Description>
                           <ns1:EquipmentClass>1</ns1:EquipmentClass>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                           <ns1:Description>Karosserie: 5-türig</ns1:Description>
                           <ns1:EquipmentClass>2</ns1:EquipmentClass>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>75914</ns1:DatEquipmentId>
                           <ns1:Description>Getriebe Automatik - mit Steptronic (8-Stufen)</ns1:Description>
                           <ns1:EquipmentClass>11</ns1:EquipmentClass>
                        </ns1:EquipmentPosition>
                     </ns1:DATECodeEquipment>
                  </ns1:Vehicle>
                  <ns1:RepairParameters>
                     <ns1:PhantomCalculation>false</ns1:PhantomCalculation>
                     <ns1:LacquerType>Metallic (2-Schicht)</ns1:LacquerType>
                     <ns1:LacquerTypeLayers>2</ns1:LacquerTypeLayers>
                     <ns1:TimeUnitsOfManufacturer>false</ns1:TimeUnitsOfManufacturer>
                     <ns1:DMSCalculation>false</ns1:DMSCalculation>
                  </ns1:RepairParameters>
                  <ns1:ProcedureRelatedParameters>
                     <ns1:ProcedureRelatedParameter attribute="referenceSetName" factor="CalculationFactor" type="String">Standard D</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="biwOptimizationMode" factor="CalculationFactor" type="BiwOptimizationMode">AUTOMATIC</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="selectedLacquerMethod" factor="CalculationFactor" type="LacquerMethod">MANUFACTURER_SPECIFIC</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="crossSeries" factor="CalculationFactor" type="CrossSeriesState">NO</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="withoutValuesOfAdditionallyRequiredPositions" factor="CalculationFactor" type="Boolean">false</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnit" factor="CalculationFactor" type="TimeUnitSystem">HOUR</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="CalculationFactor" type="Integer">1</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="dataCurrency" factor="CalculationFactor" type="String">EUR</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="increaseDecrease" factor="SparePartFactor" type="Double">10.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="surchargeInProtocolOly" factor="SparePartFactor" type="Boolean">true</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="smallSparePartCalculationModel" factor="SparePartFactor" type="SmallPartsCalculationModel">PERCENT_OF_PARTS</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="priceSource" factor="SparePartFactor" type="PriceSource">DAT</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="smallSparePartPercentOfPart" factor="SparePartFactor" type="Double">2.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="dentWage" factor="LabourCostFactor" mode="PER_HOUR" type="Price">78.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="mechanicWage1" factor="LabourCostFactor" mode="PER_HOUR" type="Price">105.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="electricWage1" factor="LabourCostFactor" mode="PER_HOUR" type="Price">105.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnit" factor="LabourCostFactor" type="TimeUnitSystem">HOUR</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="LabourCostFactor" type="Integer">1</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="bodyWage1" factor="LabourCostFactor" mode="PER_HOUR" type="Price">105.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="materialMode" factor="EuroLacquerFactor" type="LacquerMaterialMode">LACQUER_METHOD</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="type" description="Metallic (2-Schicht)" factor="EuroLacquerFactor" type="String">12</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wage" factor="EuroLacquerFactor" mode="PER_HOUR" type="Price">100.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="materialIndex" factor="EuroLacquerFactor" type="Double">100.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="typeSaved" factor="EuroLacquerFactor" type="Boolean">false</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wageMode" factor="EuroLacquerFactor" type="LacquerWageMode">PER_TIME</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wageInclMaterialMode" factor="EuroLacquerFactor" type="LacquerWageMode">PER_TIME</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="calculationType" factor="EuroLacquerFactor" type="LacquerCalculationMode">WAGE_MATERIAL_SEPARATELY</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="disposalCostPercent" factor="EuroLacquerFactor" type="Double">0.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnit" factor="EuroLacquerFactor" type="TimeUnitSystem">HOUR</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="EuroLacquerFactor" type="Integer">1</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="materialMode" factor="ManufacturerLacquerFactor" type="LacquerMaterialMode">PERCENT</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="type" description="Metallic (2-Schicht)" factor="ManufacturerLacquerFactor" type="String">12</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="materialFlatRatePercent" factor="ManufacturerLacquerFactor" type="Double">25.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wage" factor="ManufacturerLacquerFactor" mode="PER_HOUR" type="Price">120.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="typeSaved" factor="ManufacturerLacquerFactor" type="Boolean">false</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wageMode" factor="ManufacturerLacquerFactor" type="LacquerWageMode">PER_TIME</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wageInclMaterialMode" factor="ManufacturerLacquerFactor" type="LacquerWageMode">PER_TIME</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="calculationType" factor="ManufacturerLacquerFactor" type="LacquerCalculationMode">WAGE_MATERIAL_SEPARATELY</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnit" factor="ManufacturerLacquerFactor" type="TimeUnitSystem">HOUR</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="ManufacturerLacquerFactor" type="Integer">1</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="fourLayerLacquerMode" factor="AztLacquerFactor" type="AztLacquerMode">WET_IN_WET</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="materialMode" factor="AztLacquerFactor" type="LacquerMaterialMode">LACQUER_METHOD</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="materialIndex" factor="AztLacquerFactor" type="Double">100.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="aztDataset" factor="AztLacquerFactor" type="Integer">1</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="typeSaved" factor="AztLacquerFactor" type="Boolean">false</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wageMode" factor="AztLacquerFactor" type="LacquerWageMode">PER_TIME</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wageInclMaterialMode" factor="AztLacquerFactor" type="LacquerWageMode">PER_TIME</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="calculationType" factor="AztLacquerFactor" type="LacquerCalculationMode">WAGE_MATERIAL_SEPARATELY</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="disposalCostPercent" factor="AztLacquerFactor" type="Double">0.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnit" factor="AztLacquerFactor" type="TimeUnitSystem">HOUR</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="isSurchargeForWaterBased" factor="AztLacquerFactor" type="Boolean">false</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="threeLayerLacquerMode" factor="AztLacquerFactor" type="AztLacquerMode">WET_IN_WET</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="AztLacquerFactor" type="Integer">1</ns1:ProcedureRelatedParameter>
                  </ns1:ProcedureRelatedParameters>
                  <ns1:RepairPositions>
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>43712</ns1:DATProcessId>
                        <ns1:RepairType>replace</ns1:RepairType>
                        <ns1:Description>Seitenwand grundiert</ns1:Description>
                        <ns1:DescriptionId>36419456</ns1:DescriptionId>
                        <ns1:IsManualDescription>false</ns1:IsManualDescription>
                        <ns1:ConstructionGroupId>1</ns1:ConstructionGroupId>
                        <ns1:ConstructionGroup>VORDERWAGEN AUSSEN</ns1:ConstructionGroup>
                        <ns1:ConstructionGroupPolygon>63</ns1:ConstructionGroupPolygon>
                        <ns1:PositionEntryType>graphical</ns1:PositionEntryType>
                        <ns1:IsRepairExtension>false</ns1:IsRepairExtension>
                        <ns1:PreDamage>false</ns1:PreDamage>
                     </ns1:RepairPosition>
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>44910</ns1:DATProcessId>
                        <ns1:RepairType>replace</ns1:RepairType>
                        <ns1:Description>Frontscheibe</ns1:Description>
                        <ns1:DescriptionId>128880</ns1:DescriptionId>
                        <ns1:IsManualDescription>false</ns1:IsManualDescription>
                        <ns1:ConstructionGroupId>1</ns1:ConstructionGroupId>
                        <ns1:ConstructionGroup>VORDERWAGEN AUSSEN</ns1:ConstructionGroup>
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
                           <ns1:DATProcessId>43712</ns1:DATProcessId>
                           <ns1:PartNumber>41355A03262</ns1:PartNumber>
                           <ns1:DATPartNumber>41355A03262</ns1:DATPartNumber>
                           <ns1:Description>SEITENWAND V.R.</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>408.34</ns1:ValuePerUnit>
                           <ns1:ValueTotal>408.34</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>408.34</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:SparePartHistoryPositions>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>41357248660</ns1:PartNumber>
                                 <ns1:LastUPE>349.55</ns1:LastUPE>
                                 <ns1:LastUPEDate>2022-05-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                           </ns1:SparePartHistoryPositions>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>44910</ns1:DATProcessId>
                           <ns1:PartNumber>51317333835</ns1:PartNumber>
                           <ns1:DATPartNumber>51317333835</ns1:DATPartNumber>
                           <ns1:Description>FRONTSCHEIBE</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>877.6</ns1:ValuePerUnit>
                           <ns1:ValueTotal>877.6</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>877.6</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:SparePartHistoryPositions>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51314899567</ns1:PartNumber>
                                 <ns1:LastUPE>593.19</ns1:LastUPE>
                                 <ns1:LastUPEDate>2014-02-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51317280748</ns1:PartNumber>
                                 <ns1:LastUPE>593.19</ns1:LastUPE>
                                 <ns1:LastUPEDate>2014-02-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51317280748</ns1:PartNumber>
                                 <ns1:LastUPE>593.19</ns1:LastUPE>
                                 <ns1:LastUPEDate>2012-11-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                           </ns1:SparePartHistoryPositions>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>40270</ns1:DATProcessId>
                           <ns1:PartNumber>51489162739</ns1:PartNumber>
                           <ns1:DATPartNumber>51489162739</ns1:DATPartNumber>
                           <ns1:Description>SCHALLISOLIERUNG FRONTSCHEIBE WINDLAUF</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>54.27</ns1:ValuePerUnit>
                           <ns1:ValueTotal>54.27</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>54.27</ns1:ValueTotalCorrected>
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
                           <ns1:Description>ABDECKUNG FRONTSCHEIBE O.</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>26.06</ns1:ValuePerUnit>
                           <ns1:ValueTotal>26.06</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>26.06</ns1:ValueTotalCorrected>
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
                           <ns1:Description>REP.-SATZ EINGLASUNG FRONTSCHEIBE</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>66.18</ns1:ValuePerUnit>
                           <ns1:ValueTotal>66.18</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>66.18</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:SparePartHistoryPositions>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51311958028</ns1:PartNumber>
                                 <ns1:LastUPE>32.69</ns1:LastUPE>
                                 <ns1:LastUPEDate>2016-04-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83199407850</ns1:PartNumber>
                                 <ns1:LastUPE>51.26</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>81220142749</ns1:PartNumber>
                                 <ns1:LastUPE>51.26</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>81229407497</ns1:PartNumber>
                                 <ns1:LastUPE>51.26</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147369</ns1:PartNumber>
                                 <ns1:LastUPE>42.44</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147370</ns1:PartNumber>
                                 <ns1:LastUPE>73.11</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147371</ns1:PartNumber>
                                 <ns1:LastUPE>42.44</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147372</ns1:PartNumber>
                                 <ns1:LastUPE>73.11</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190392461</ns1:PartNumber>
                                 <ns1:LastUPE>184.03</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190393939</ns1:PartNumber>
                                 <ns1:LastUPE>41.18</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190393940</ns1:PartNumber>
                                 <ns1:LastUPE>17.65</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190444141</ns1:PartNumber>
                                 <ns1:LastUPE>47.9</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-06-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51318109154</ns1:PartNumber>
                                 <ns1:LastUPE>81.59</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83199407714</ns1:PartNumber>
                                 <ns1:LastUPE>70.59</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>81220142749</ns1:PartNumber>
                                 <ns1:LastUPE>51.26</ns1:LastUPE>
                                 <ns1:LastUPEDate>2014-02-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>81229407497</ns1:PartNumber>
                                 <ns1:LastUPE>51.26</ns1:LastUPE>
                                 <ns1:LastUPEDate>2014-02-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147369</ns1:PartNumber>
                                 <ns1:LastUPE>42.44</ns1:LastUPE>
                                 <ns1:LastUPEDate>2009-05-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147370</ns1:PartNumber>
                                 <ns1:LastUPE>73.11</ns1:LastUPE>
                                 <ns1:LastUPEDate>2010-03-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147371</ns1:PartNumber>
                                 <ns1:LastUPE>42.44</ns1:LastUPE>
                                 <ns1:LastUPEDate>2014-02-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147372</ns1:PartNumber>
                                 <ns1:LastUPE>73.11</ns1:LastUPE>
                                 <ns1:LastUPEDate>2014-02-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                           </ns1:SparePartHistoryPositions>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:PartNumber>51317288462</ns1:PartNumber>
                           <ns1:DATPartNumber>51317288462</ns1:DATPartNumber>
                           <ns1:Description>PUFFER</ns1:Description>
                           <ns1:Amount>11</ns1:Amount>
                           <ns1:ValuePerUnit>1.95</ns1:ValuePerUnit>
                           <ns1:ValueTotal>21.45</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>21.45</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:SparePartHistoryPositions>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51314875651</ns1:PartNumber>
                                 <ns1:LastUPE>1.49</ns1:LastUPE>
                                 <ns1:LastUPEDate>2011-05-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                           </ns1:SparePartHistoryPositions>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:PartNumber>83192211217</ns1:PartNumber>
                           <ns1:DATPartNumber>83192211217</ns1:DATPartNumber>
                           <ns1:Description>REINIGER (100 ML.)</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>11.55</ns1:ValuePerUnit>
                           <ns1:ValueTotal>11.55</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>11.55</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:SparePartHistoryPositions>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83192157286</ns1:PartNumber>
                                 <ns1:LastUPE>9.05</ns1:LastUPE>
                                 <ns1:LastUPEDate>2011-07-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                           </ns1:SparePartHistoryPositions>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:PartNumber>51317288462</ns1:PartNumber>
                           <ns1:DATPartNumber>51317288462</ns1:DATPartNumber>
                           <ns1:Description>PUFFER</ns1:Description>
                           <ns1:Amount>6</ns1:Amount>
                           <ns1:ValuePerUnit>1.95</ns1:ValuePerUnit>
                           <ns1:ValueTotal>11.7</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>11.7</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:SparePartHistoryPositions>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51314875651</ns1:PartNumber>
                                 <ns1:LastUPE>1.49</ns1:LastUPE>
                                 <ns1:LastUPEDate>2011-05-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                           </ns1:SparePartHistoryPositions>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                     </ns1:MaterialPositions>
                     <ns1:ExtensionPositions>
                        <ns1:ExtensionPosition>
                           <ns1:DATProcessId>45335</ns1:DATProcessId>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:Description>SILIKONFOLIE REGEN-/LICHTSENSOR</ns1:Description>
                           <ns1:PartsSum>27.62</ns1:PartsSum>
                        </ns1:ExtensionPosition>
                     </ns1:ExtensionPositions>
                     <ns1:LabourPositions>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>43712</ns1:DATProcessId>
                           <ns1:LabourPositionKind>1</ns1:LabourPositionKind>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:LabourPosId>41 35 555</ns1:LabourPosId>
                           <ns1:Description>SEITENWAND V.R. ERS.</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>1.58</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>165.9</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>165.9</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>41 35 555</ns1:WorkNumber>
                           <ns1:SparePartNumber>41355A03262</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>43712</ns1:DATProcessId>
                           <ns1:LabourPositionKind>4</ns1:LabourPositionKind>
                           <ns1:RepairType>body cavity protection</ns1:RepairType>
                           <ns1:LabourPosId>97 35 511</ns1:LabourPosId>
                           <ns1:Description>HOHLRAUMKONSERVIERUNG SEITENWAND V.R.</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>0.42</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>44.1</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>44.1</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>true</ns1:hasRequiredByPosition>
                           <ns1:RequiredByPosition>
                              <ns1:DATProcessId>43712</ns1:DATProcessId>
                              <ns1:RepairType>replace</ns1:RepairType>
                           </ns1:RequiredByPosition>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>97 35 511</ns1:WorkNumber>
                           <ns1:SparePartNumber>41355A03262</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>44910</ns1:DATProcessId>
                           <ns1:LabourPositionKind>1</ns1:LabourPositionKind>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:LabourPosId>51 31 513</ns1:LabourPosId>
                           <ns1:Description>FRONTSCHEIBE A+E/ERS.</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>2.58</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>270.9</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>270.9</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>51 31 513</ns1:WorkNumber>
                           <ns1:SparePartNumber>51317333835</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>14449</ns1:DATProcessId>
                           <ns1:LabourPositionKind>4</ns1:LabourPositionKind>
                           <ns1:RepairType>adjust</ns1:RepairType>
                           <ns1:LabourPosId>66 51 525</ns1:LabourPosId>
                           <ns1:Description>KAMERA FAHRASSISTENZ-SYSTEME KALIBRIEREN</ns1:Description>
                           <ns1:WageType>electric</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>0.33</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>34.65</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>34.65</ns1:ValueTotalCorrected>
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
                        <ns1:LabourPosition>
                           <ns1:LabourPositionKind>8</ns1:LabourPositionKind>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:LabourPosId>ARBEITSAUFWAND</ns1:LabourPosId>
                           <ns1:Description>ERGAENZUNG HAUPTARBEIT</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>0.17</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>17.85</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>17.85</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>DAT#</ns1:WorkNumber>
                        </ns1:LabourPosition>
                     </ns1:LabourPositions>
                     <ns1:LacquerPositions>
                        <ns1:LacquerPosition>
                           <ns1:DATProcessId>43712</ns1:DATProcessId>
                           <ns1:LabourPosId>99 35 011</ns1:LabourPosId>
                           <ns1:Description>SEITENWAND V.R. UMFASST: VORBEREITUNGSARBEITEN</ns1:Description>
                           <ns1:Level>4</ns1:Level>
                           <ns1:LevelDescription>new</ns1:LevelDescription>
                           <ns1:LevelManufacturer>ST.2</ns1:LevelManufacturer>
                           <ns1:Duration>2.42</ns1:Duration>
                           <ns1:ManualDuration>false</ns1:ManualDuration>
                           <ns1:Material>72.6</ns1:Material>
                           <ns1:ValueTotal>363</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>363</ns1:ValueTotalCorrected>
                           <ns1:WageLevel1>290.4</ns1:WageLevel1>
                           <ns1:WorkNumber>99 35 011</ns1:WorkNumber>
                           <ns1:LacquerPositionTimeState/>
                           <ns1:LacquerPositionMaterialState/>
                           <ns1:LacquerPositionPriceState/>
                           <ns1:MaterialType>2</ns1:MaterialType>
                           <ns1:SparePartNumber>41355A03262</ns1:SparePartNumber>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                        </ns1:LacquerPosition>
                     </ns1:LacquerPositions>
                     <ns1:PriceDate>2023-12-01+01:00</ns1:PriceDate>
                     <ns1:RepairCalculationSummary>
                        <ns1:SparePartsCosts>
                           <ns1:AllSum>1477.15</ns1:AllSum>
                           <ns1:ConsumablesSurcharge>29.54</ns1:ConsumablesSurcharge>
                           <ns1:ConsumablesSurchargePercentage>2</ns1:ConsumablesSurchargePercentage>
                           <ns1:TotalSum>1506.69</ns1:TotalSum>
                        </ns1:SparePartsCosts>
                        <ns1:AuxiliaryCosts/>
                        <ns1:LabourCosts>
                           <ns1:AllSum>533.4</ns1:AllSum>
                           <ns1:Bodywork>
                              <ns1:Type>CAR BODY</ns1:Type>
                              <ns1:Units>4.75</ns1:Units>
                              <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                              <ns1:Price>498.75</ns1:Price>
                           </ns1:Bodywork>
                           <ns1:Electric>
                              <ns1:Type>ELECTRICS</ns1:Type>
                              <ns1:Units>0.33</ns1:Units>
                              <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                              <ns1:Price>34.65</ns1:Price>
                           </ns1:Electric>
                           <ns1:Mechanic>
                              <ns1:Type>MECHANICS</ns1:Type>
                              <ns1:Units>0</ns1:Units>
                              <ns1:Price>0</ns1:Price>
                           </ns1:Mechanic>
                           <ns1:TotalSum>533.4</ns1:TotalSum>
                           <ns1:Wages/>
                           <ns1:Works>
                              <ns1:Work>
                                 <ns1:Type>CAR BODY</ns1:Type>
                                 <ns1:WageLevel>1</ns1:WageLevel>
                                 <ns1:Units>4.75</ns1:Units>
                                 <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                                 <ns1:Price>498.75</ns1:Price>
                              </ns1:Work>
                              <ns1:Work>
                                 <ns1:Type>ELECTRICS</ns1:Type>
                                 <ns1:WageLevel>1</ns1:WageLevel>
                                 <ns1:Units>0.33</ns1:Units>
                                 <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                                 <ns1:Price>34.65</ns1:Price>
                              </ns1:Work>
                           </ns1:Works>
                        </ns1:LabourCosts>
                        <ns1:LacquerCosts>
                           <ns1:Wage>
                              <ns1:Type>LACQUER WORK</ns1:Type>
                              <ns1:Units>2.42</ns1:Units>
                              <ns1:PricePerUnit>120.00</ns1:PricePerUnit>
                              <ns1:Price>290.40</ns1:Price>
                           </ns1:Wage>
                           <ns1:TotalWages>290.40</ns1:TotalWages>
                           <ns1:Material>
                              <ns1:FlatPercentage>25</ns1:FlatPercentage>
                              <ns1:FlatAmount>72.6</ns1:FlatAmount>
                              <ns1:MaterialGroups/>
                              <ns1:TotalSum>72.6</ns1:TotalSum>
                              <ns1:SumMaterialCorrected>72.6</ns1:SumMaterialCorrected>
                           </ns1:Material>
                           <ns1:TotalSum>363</ns1:TotalSum>
                        </ns1:LacquerCosts>
                        <ns1:TotalNetCosts>2403.09</ns1:TotalNetCosts>
                        <ns1:TotalVAT>456.59</ns1:TotalVAT>
                        <ns1:TotalGrossCosts>2859.68</ns1:TotalGrossCosts>
                        <ns1:TotalNetCorrected>2403.09</ns1:TotalNetCorrected>
                        <ns1:TotalVATCorrected>456.59</ns1:TotalVATCorrected>
                        <ns1:TotalGrossCorrected>2859.68</ns1:TotalGrossCorrected>
                        <ns1:SumNet>2403.09</ns1:SumNet>
                        <ns1:SumGross>2859.68</ns1:SumGross>
                        <ns1:SumSparePartCosts>1477.15</ns1:SumSparePartCosts>
                        <ns1:SumSmallSparePartCosts>29.54</ns1:SumSmallSparePartCosts>
                        <ns1:SumLabourCosts>533.4</ns1:SumLabourCosts>
                        <ns1:MetaPositions>
                           <ns1:MetaPosition key="TOTAL_NET_RISK" value="27.08"/>
                           <ns1:MetaPosition key="VAT_RISK" value="5.15"/>
                           <ns1:MetaPosition key="TOTAL_GROSS_RISK" value="32.23"/>
                           <ns1:MetaPosition key="TIME_UNIT_SYSTEM" value="STD"/>
                           <ns1:MetaPosition key="LACQUER_TIME_UNIT_SYSTEM" value="STD"/>
                           <ns1:MetaPosition key="DAT_EUROLACQUER_IN_HOURS" value="false"/>
                           <ns1:MetaPosition key="TOTAL_PRICE_SPARE_PARTS_RISK" value="27.08"/>
                           <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EQUIPMENT" value="false"/>
                           <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EXTENSION" value="false"/>
                           <ns1:MetaPosition key="FLAT_PERCENTAGE_BASE" value="290.4"/>
                        </ns1:MetaPositions>
                     </ns1:RepairCalculationSummary>
                     <ns1:CalcProtocol>
                        <ns1:ProtocolHints>
                           <ns1:ProtocolHint>
                              <ns1:Identifier>H001</ns1:Identifier>
                              <ns1:Description>Serientreue Kalkulation</ns1:Description>
                           </ns1:ProtocolHint>
                        </ns1:ProtocolHints>
                        <ns1:ProtocolData>JVBERi0xLjQKJeLjz9MKNSAwIG9iago8PC9GaWx0ZXIvRmxhdGVEZWNvZGUvTGVuZ3RoIDQ0NzE+PnN0cmVhbQp4nLVc3W5bNxI+gO4cYCvHkuxILqAFkrhNUuX8/6ToTSFHsi1YlmxJThrf7aZAsQa2vdkHWGDfozd9jDzbzgyH55AUKR+f7sJQJFHkzPCb4fzxIL/u/bq3gFc4PN/zhxP4/OPNXjD04S8YJv4oT4ZZEQ5v7vfevg+G2fDm8943XuStvKW3gdclvObw1/LuvFvvCt4LGFl5597YW3jn3978snd6o5KM03QUW0ieeM+9zGvD69M3XgpvP3odr+t97R14h/DvoXfsfQXf+94R09whdpgXoywaRpHgEQ5zwaODS78BGZ96LfGxy8SQFBCI02GW+cObvwHN77Iww0/8qz8q4sIPh+b7bz/vxTmhFISjPBsGaTJKh4E//O3ve59rrPKbrEqLRqvyRquyRqvieOTDKniLHrEqsq7KeLb+TquGqR+NQFGJnwyDrCabJI9xzSOFS7JGq9JGq5JGq+JGq6JGq8JGq4JGq3zrqjzxi3xovguziLNiFLNZBHUWhH42SvUFqn8BB0CffgEyyfBf8G/KRPT35UQe7JCOzf1eCFuOy+//2LsuRwKeofkPdYJJopph8NiisHiMwCa7JAlHgSowDwROcbQV9/r8eht6lMDadm3U5Iiv4+M7VaAvUBAOXBQaIRy4AOIB3ymOoQJtfr0NNUHYLQ+PcCC61+OSTQX6AgVh30WhEcK+CyAxUMq7LY6hAm1+vQ01QHiHPHIk1/HJnSrQF1QImzrK/xTCJbUtgHggd4pjqECbX29DTRB2yyNHMh2fzKkCfYGCcO6i0Ajh3AUQD2ROcQwVaPPrbagJwgklbfd7QRGNgvI7UpMjMc/QckN1gkmimmHw2KLwKIFNdgxQJTAPxE5xtBX3+vx6G2qCsFseORLp+EROFegLFIRjF4VGCMcugHggcopjqECbX29DNoGT3I8KEDSJgwAFjsIiDgTCwzT0Mb1EXpH8IiSJZHlxr5Qa5U/asuo3laK+qoHqkyIWlHib/F0BgosZqTj+qk4wSVQzDB5bFJqovqQmNKcIzAO5Uxxtxb0+v96GmiDslkeOZDo+mVMF+gIF4dxFoRHCuQsgHsic4hgq0ObX21AThN3yyJFUxyd1qkBfoCCcuSg0QjhzAcQDqVMcQwXa/HobaoKwWx45kuj4JE4V6AsUhFMXhUYIpy6AeCBximOoQJtfb0NNEHbLI0diHZ/YqQJ9gYJw4qLQCOHEBRAPxE5xDBVo8+ttqAnCbnnkSKTjEzlVoC9QEI5dFBohHLsA4oHIKY6hAm1+vQ01QdgtjxwJdXxCpwr0BQrCkYtCI4QjF0A8EDrFMVSgza+3oSYIu+WRI4GOT+BUgb5AQTh0UWiEcOgCiAcCpziGCrT59TbUBGG3PHLE1/HxnSrQFygIBy4KjRAOXADxgO8Ux1CBNr/ehmwC229TRCkEH7FtLmoa/iLrHW6p3yvt9fInbVn1m0pRX/VYwcIgx/a84MBfJHdu3d8rbfzyJ21Z9ZtKUV+10K8S8UYwyrA7wteVYfynr0AhbGbYqk1GEZON5C2ottJbw79joDgVl5Vfb5MKodCMdFrNb1S3RfQtIj4n0aaw4Sm8b2C7E9j2ynvvXbjl8y3yIaGPQGQBBKZA4AAEanlPSKzW1q+fPrukTAuHlHMADyWdwPsGVeOUTyVRyteFv32CbB9eB/DqOUXILSL8p5T9lrVZQ5D8TwqSWQQZkQATAnMGrzMysisSZgafF25xMos4Ha8HQhx4R/BnEQROTJoU2IuhZfEwCGmdU+Q4HSWmyOJ0ncO/aP9X3gfCce0SNyiAoU5KEXffewZWvg8iD5xCRBYhTrwXcHyKeqwjC+sTsGNU21O32hAt0Sx6EK0A3GTqp6OsZBMEONenCb/9DAw/fQt4XYC4dyD0LeAnLG4qBPeHPyssfvouyJNoVIR3N+dWTJK84lVi8prR2JAHQB+wcjonhkalU0LzwvO9dy5tJJmV8xi2dA2cN96nT971g2wzK9sxOaspqPMC/m2BDbfANS5pdEbnFH0QANmBv0+f4TPqrgOvtvfXHV4oSS0y50BwQ4jVlDm1yHxEEkycjBML48J74wUPckss3N4BRs/BciFmfF+FDnzl8Aue+45TktgiiYhCrSf/JoSXoMAxIPkSPqFD+ueDMsYWGVEfLfZDLVIUfj/g7wf013VKGVmk9DmWP2zMkUWecjVw70L0QinewsgKnE4LditkRUu7BHzR3hCLU8JgBiis8TA55Q0t8o4ARURzTWvRct05gpQ8tEhuoQOpAZ6KNsj/hUacGUwSWCR7BRQ2TOm0hlSBRSqDBmUDt4SwDFqXjOsVfMYUJKVjdk2rlhTm3tM5HsCslGLuGYW/HefXt2xGuIs7chebB7fiOw7vsde3On5OjWs5/jj3R0VJnJ9nS0udLUjQNTnmMbnIW8fjd1TSxGlSclbSjGcgqsjCngNVtNAx+cMXBMAZxxYRAAgS0s0Y5q0x/YNPcxjDVXSODJ5JzjwFqwEdWJNVGcGQSxsi5w7eNh5ByaMHGW6fcl3kcUlm84EEHpEbOiOwvsDrTgZIg1gcl8TQ//fh36MtYtXZvyAdnFrlghJCkjpkB3XASS6SasM250DkPZCe8dZTjBgi0F6RLT+HSSlbsEneVyQdALhy2/qpEVqaqjDP6ahcwM+qCkvjMfiEkaJCLCCO2VpyCBZtjDnwL25KEJuzTQrpqznWPYAjqPYgYt4B7+F3svA1KG1GRceUqi1RglyWflbmiDI1Qf8gEt8W7XoGinbZpl8oGzsiu+lqzIUaromFSOJXVKQJ33BuVbofalo5opwZTxMq/Hsii74KVf2eJRQ1z4q8lUXOqEg0ksdkTS2yHlx8SZDcskaRAQYiiOEnFlp5ru0ZxRsQLTTmCdBY0o5vRQZjIxBoRj3guPyCzukVaGJM2p+xThbChRpEstg4GUe8I0kEF06pKBYn4wudEjSCj7TnBZdXaGQJGcStoifK2kkM5TTZ7C9KMw0OPEPPgOhL0gyyFFnLgmPM3DiiNoq+RrHHFn1CW7sA0xnTGbmiDGDtADmJNI2jzgdEBFiL7oB6rivYNEOw0I2r49bnBPfATTeluHIKY3PyvX+QwzARQRWcwNyXdoSjQtlKh9SNCIN5/sRZ8oyEXlEb5QyYiE5DC5ImUckvKBCs7E42ikJtS0cEmOLrTHO8M73s12YAmlMCsqA1qn+0qypMlOBzRID2BEXhvsQeLzipWRkuTMKNjgxPIJ7dv5DrmrH/scSoKMg1jzwAjsxTFDnoNFdkwNLBrEqPL8+NTKJyQONF6Y4WNLpRaz0b/0DhPyCddgV/9JxXnIwIT1QQHVFqrS20/Fih1acTiP7yFWV2f9AZXFGMvaIoc0qwTQ0XEFDueGe1wLDINA6HbPQ2DmjtEz75kvpTeCXc7VvayPtahtOnUyXIC90KjzWhiHHJaQweo6QMa2Olb1VppjrWZyTMpdq5MYTII8UKj0uNyJz6D1o+VU1ZM7kqYu4wuzBLNVM/4qP8mgG7pD1ckx9ekLULl4H7lmCObcmJhVWqeo3j0otKVuvStE+J2UfFb1kOaZiGGjw9jnpvYNES0J2BL2pT3D8jN3hB7hmBOaNyCLPHWdnYW5N+7mg3CzKOLywUjVvYJ4mWUx6wjdeuwwxy8XZOfaRkuG0tu97KKXfrOA62aB/Wp80WZWktwiEMHCWIKEAw1ca8ZUqmigdyQkcbR2QzWDkcPihrTia043BIrkoRgsxkTiaZrcFMb8kpS4aVCMx0ynFgYU06txLMkrGaLA0oHRCMfcCOQsScQ1wLfv4JrKNPMhQE7TVZuIzGXVj8zPBwkk+s5lNdwlPwQYveUGKpNqXxIEkjwG0ii7Xu6SXlSHee8iD6HCeE98K+8pzcy4JEdZhYSdPXaHbZWe2mqZiWSU8pUAbk4Dss4/+gQUO2T80sCjMtqi9xrl0RSj0j4TreZa2UL5tbndFZAvPACRMbG6VyOaQQLPQdcIEq253nxHZWad5KS02gRFYoaIXkFXUzXIHoY0oL5+Lkj0uIn4j2Lhcmt7STiOsaefWwADJTO3RqlSMLix6RGBPXU6U2sOZQNpq5evBFcXlIHlu0F8TB61Ki/pQiGv4mDuE+/P1gpRkoNAckZ9egKWL7NUku68Y1xUOECe2ySqoBxTZtEkOIHZks1kqKY467KsdrAnfB3J+7alRJUSl7+px0iT1g/ibkFg03xPmMZN3Kf0tavhJbe2VFaURFzcDPCYsp032qZA4uT6pWRH3yGV3SUsp+eULeGGP5GR+oFkVykVtj2nhOlcCCTZEKENGbbnnPbAzjVMtAOgxRupV5jDnzmMCG12xSzs6DpB4VW9Q7VupKXqNEP5k6LpjjWnaxt/iEGh/ZgnL0HthwZ1QGyKRtbaSnT2B1ApDabVUph2RrsUcMZesQtaL2/tx+XS9zjsgvdZjWCtbNyJlYqrk3HHzmdMQETjLnDSgorCgwtsr2yT65dOFUdPJrq2CBlk8M+C5CrlwSnYVSQ1S/KL1qG2WlGuqRY5eUZ9yyVLN2eYQe6om5rFCtjPDgHvLRTekgbajSn1N+OuX02OzGV+mxOHrIV9ZSonKyFAdWSXyjtOiw2WzYGYmOPiahbeC2EOmojVIebbm2jkbpqULpuWHZVMGq4dlq5HohdEwcnnnyPgJ3O2HUkCbeBRdbHdLfRWbZgx/OhJ+yMdLKoAE5ih6ZKoos2+NVN9fW9ytJqWG+RzL3qTyfc7LTpouPjdKUaVFwQ/d54Ylu7isIXnZIErUNMiCHhtH0HTkqKemae3QruxFodQ3+iVbOO0jPV5SDt0l5yzLSCThv6WgIoz8nda7Lg3dJBnvKLk3cyeJWdmeoahU0ptgxpeddFhwRNw4Qoliz4h7b3g/sgVaUNn1gCKquttmSocJgxTX0hK96XFc7qXymqdaNUgiZY7B9o7Qsi9tH3Sjho2dpSY3LuR6fOnHNI8CXHrhNNztql9Jx6RDkKVMWvl/WoeiEJnQ22+DKx+Smz9093xY/U3LmTbkNuKQANLdwzIqS4wHVEeZtgBUaCjgp5yBLCKZtOIMzznNe0+3OBVvlwtYbCLJQ2+gx32ebXecTbushIdigZiyiOXrFcaXKx8WjXmh/ontl647R//CgVCwDLp5OOHm6oGrkikshcXUl2qp3LECV97/hNhcqBY/L2MUzyUue6Dk7ZXtb8FwRN/lcxhaILsBtjAINXHkz+LjmsKiA8CQKVgL5HVk2M4eiPFXcmew6UJdWKFdvYwkXe0v9vi8kXmVhIwIEQ6/waKKkMv0QM46yknGfTKpDu/5/X7CbUvga9l3G/jXVp4jlLYVg3bAtdMJIoXNIrqXPHQyAckZKEW1Fve290lyBhXBQuZge30wM2IoXDxx4mWFWlxdzb6rYEUI7pyxIBB6RD73ly411mQfMKGtqEYyzHX0zp6M95hBTCW1emEpdYg10yonpZKsPe2kJZ6YPPuTs4w3fa4gbG+naF1qsrTwy2gsC9bGsAFZlMp6TJYvHXq0RVXXKXb4G62rHYWsjVNC3yectWBcSgmruPjOfc4PMvNP6yipL5alrbMhGQfG1PXpUQUTJt5584lVUfHTVBVKojypUNYBaAcgLYLxtlz18eQLwPHxltEr2bVIp3rhu5aA6VlGOH5Yttwmv/UBxaUZoiGdGXnoh6UZVO5qHfC4MG3IvIZrYTUFxpx268hLWGLA3myveVC9qd2TFqqvESNTjoB+RdEtPPIk6pgPznrPgV5xi2qU0vN5AIbii6+QTdhOyGWa7To1glnmdKhko7rDHT7+pFSJCcUdPgYr6KyKi8hqy8mBVW13E3UuqTcc2joHqBo75jrPiKHsdMot1F/SBX2gRseqpPCal15J3r+VI0NHyy8dNt+SoTvLDOQsvKhItDPW5s5tSzBHWoabrZuzZytrBs+UPJ+34pHBa57FqmJiEzieK/wurxPPWCmVuZHN0cmVhbQplbmRvYmoKNyAwIG9iago8PC9Db250ZW50cyA1IDAgUi9UeXBlL1BhZ2UvUmVzb3VyY2VzPDwvUHJvY1NldCBbL1BERiAvVGV4dCAvSW1hZ2VCIC9JbWFnZUMgL0ltYWdlSV0vRm9udDw8L0YxIDEgMCBSL0YyIDIgMCBSL0YzIDMgMCBSL0Y0IDQgMCBSPj4+Pi9QYXJlbnQgNiAwIFIvTWVkaWFCb3hbMCAwIDU5NSA4NDFdPj4KZW5kb2JqCjggMCBvYmoKPDwvRmlsdGVyL0ZsYXRlRGVjb2RlL0xlbmd0aCAxNDEyPj5zdHJlYW0KeJylWF1v2zYUJeA37aFBk6BFtwF6CNAUwxRSEinptXCaNTXqOLOTDHBfhi0Fivmhfdm/62/b4SVFkTIVWx4MfdDkOffce/kh8mvyNVngytPrhKdXeH+7TETK8ROp5Fkt06rJ0+UmuXgn0ipdPibnrGArdsvucX3ENcdvwj6xB3aDZ4N/VuyaTdmCXb9Zfkkulz5lqVRWRihfszNWsSNc63Om8HjLTtgp+5kdsxe4v2A/sWcov2IvLecTsvO6yaoiLQpjI09rY+NUQ8+h8TmbmNdTS6apQFCqtKp4uvwLnL9WeaXfbC3PqrLhedp/fvuclHValTzLES6ZCpV++zt5THTkeFOn/adtn8u2vWjbN5Y3fFJ7ygKvARFNkTVA8X2sqLpArEdZUZSecVZKkanAikj1r+OEsyoVptD0moimyirbpIKctsHTNqUqs3qcZ7KsALEqOs92oYo6K5z2TO4Ly+vO2AiYaA6yxptDrJVNsx0Rf1Ch19PbF3DJ9F99r3nRgEmWQuicFHlTivT2ivq0VOigm0TKwr7/k/xuSjQ6Nt1AcRU+xNV4XAFiEREUH5RWUOGxF4EgGn6bbiS6Ch/iajyuABETpGxvDZ8kiEaxqIknL3PE3pQ0lS3z2lrpRrxXG2Jdbcjcx44SGRqSMs+EJ9KWeVyG33oTtN3twtjUqqbENGXyZN7bDJo5b9NNf67Ch7gajytAHJBaVSniMb6ZUue5mVg3wTTr1YZYVxsy97EHpLalMunpRNqyisvwW2+CtrtdGJ1asKs2T/TuMkgLzaZbc1yFD3E1HleAGCtIVhIOGXbz3to1q9CmW5BchQ9xNR5XgDigr0lZEY9ZPU1JU9lyWVkr3cLn1YZYVxsy97GjRIaGTH/pRNpyGZfht94EbXe7EBFJn4SdJFrOnXdU0sDdvoRqHdAP0zbtE3qsY1ZPn/YJPWH0fJrtDtCnPSSJ9CXjXKOSZyjU72r9QGxjR8mwHloZfUNhGP22u0Xu7i30Oeb0U2m/3hKqdUA/ENu0u3uL1dOn3Tt6Po0XnwG1h/QW+hJ1rlHJMxTqd7V+ILaxh/QWK6NvKAyj33a3yENm6QEZpmw+v1t/TcmTEWC72pC5j/0fKetHw5RbkX0ZYZz9trtdWIS7db3pps992qxj85nTbn376EAKeFSVBcjs2QE2f2hqRgm2Neds/YZN2Uc6mVix39hCk/D0c5QoVx2RPSDIgJ4D/4D7FCwz8Cxanh5HmVX6o5t3JPYkwx4tKOBWYACafWeXVLomVTP2nv69wn0St7ltL0eqq6g9QZQRCAJrvm33CqyqS+y+w3iszyH4jmR9wqXtzCF+K8Sx0ChVd3xhaM7g7Ht2xJ7j7RL879gHcj5yXGTcjnGdsGP2DNdx3HH68tvPcfQo0XP8DL5dkr/30DeHrx+QsH08z/V5R9XaLlq1IeEUpfuIs1ioRIB33irgHqjfTNjJoGHsrvpADoiOrz6Om0H9hP2g01ozifAbVtMT148xQRiXuc9b+OF/OZQAKwfjvy8nI99vEYM7Nz4OktRxj5PEtyTB9BzGdGJXh4eoIx6jRzZiS89rWJqTpAWkXEHUd2Twoy2PkYYtD298G07aK/bjE4PH7FL2GjwS+7yiN3gukGMteM+JQkreUYQTRcs0o75yg/s9uvKt9jjiLi/0OWSEraU5Yr8Q0R3NZSbGK/yr2Hpt/7wZVFnyNiZDKodGtdEVwXNyaEpKZqDQ2T0lPXrEzuh+j9RShT4Nj2XZyitE63YxIM/OYoMMuRhy8AgCLobQ1r0IWiu2czQIYt12UIvId3lzQ6uSmUIQwUEmng91Lu1VAeyDXYGm1B8m7A94etN5bMbcn/ERZnyP2DgdHvkYYGU9sDb9B8fKwaUKZW5kc3RyZWFtCmVuZG9iago5IDAgb2JqCjw8L0NvbnRlbnRzIDggMCBSL1R5cGUvUGFnZS9SZXNvdXJjZXM8PC9Qcm9jU2V0IFsvUERGIC9UZXh0IC9JbWFnZUIgL0ltYWdlQyAvSW1hZ2VJXS9Gb250PDwvRjEgMSAwIFIvRjIgMiAwIFIvRjMgMyAwIFIvRjQgNCAwIFI+Pj4+L1BhcmVudCA2IDAgUi9NZWRpYUJveFswIDAgNTk1IDg0MV0+PgplbmRvYmoKMTAgMCBvYmoKPDwvTGVuZ3RoMSA2NDk1Ni9GaWx0ZXIvRmxhdGVEZWNvZGUvTGVuZ3RoIDIwNzUzPj5zdHJlYW0KeJzsvAl8VEXWNn7q7r0k6c5K9oQkhLBGwiJ7i+wiRAUEFAgQI+ICiEAANSyyCQxrQBEhKiAGxIiICaKCRNlHHUBlwBcXEB0jMg6KA0n391Td20knwKj/ed/v/f/mM8mTU/ty6tSpU3XrXmJEZKPpJJNr1KRHkui++LYIWUPEvHnj7n1wfMtJY4gk+GnzvQ9MybvQctUlIrkn0Q1Fo+8ZkWsMLXqRqOU3iG89GgFB6xLfIWqVBH/q6AcfyX+v9fE28HclGpH3wNhRI5StMf2JVm6Bf96DI/LHxf1ZG0/0S0ukTxr38D3j2ut/h/MXpFFHs1ZUSofwu4eKaQ3bCF8eIscjpEjaRrNpIkL2skNsvtQUYRvpAh1Fyrl0SC5WiPWmLIQSnVAlusj603aU0ZaFs7a6ppDSV9mu3K6UKueUI9RGmaAcUXKUCSxLfl4dqG4E2srvSaF0gBKplJ2mCbRT/lbOkncpXZVgOi0fkYvpLGpRUP4hWkzraRraEs7GUoE0TbodIfvUI7Qav2MRf4StZUfRup1sFh2np2RF6klr2XH06xD9TLPk/lIBeJol5aH9+1DWEeRfTRMUUo8zO3mlxgjbzseERor/8XJT9bj4vUAFqLk/rddKtXA9BbVwjm1ke1mFtpyK6Kh8tzxePslmKynKJqUnLTY5IOfQYpS9mufR8tgU9J3/TuOlS5OVHFZM3yo5+kiU/R7vEercLt2OHuXRLmCy5kKf2rPZ8ny0lMfG0xG9t9Ic+VGC/hh6TTRWbkVj4JpGW2kbNZVX0mKUJPqrtVF/Rs41yhfo82K2SPqZjshdKYPylPPgNYVDRIje0DVVkSVGTZJcJVJar9wSz22DkvYPTm7apI43yaUnlVB2SdCUpFKfL3uQEqsOLlHjSuQ0o0RJS/niepFfNG1yS/agpJKqbl2tUrvldEXYHYPg5D4EI7xbVxHHKy1R0/DXK6ckadTopCddT6a0e9J1T7umYBvleVcqeep6zCSdYjxO5QppV5ihFkgKNS8/VnEDuY5VHKvIDHMnu9OS3cl5ClVOkGMrz3pX6sG//PiwlkEqjfd9pWdgVB0URSmUDgme72mdGpLWIK1BSHpqehda5kxY1mxRvWWp2jLnogahCxumLm2ZnhybZpODIoJtQSHJQY2DY4NCbnC0dFXeUmLrf0uJo/9dt5Q4+b9w/i+Y/wvqf9egMrrBt/vGweUVFytc538+727rDm2LNp5pcbHDGRHiOp8JRugu9XuOwfVZfS0iPDKrRetWLRukt4iMCNdS6jdo1bJ1YHhaFksJC4hTP7pz1Kg7B4waNWDtzjefLdr5ZuWqgaNG3nnnqFz5hqLKIUWJa3e9uW5d2U5p6YonZhYWzpxVWHDqzTdPnnxz10lpROHMJ1aseGLGyoJ//kMLOvnmW389uWvnKQgWMSrx/ihN00IpiNp4QrSnaFVwkE5yqEZh9mDXqVtKwvqjf3bev1tKQoSbPDcOPtOiwt2Wd7KyIpNpUkR4aFRKA6lVy9A20rQ5M2fNLlpZuGKVFvq1t9O5c972Z79j739+mpVXoL71qG+sqC/RE6Lz+nRGjlAlzCDU1+FiTblhWZGhEeGSntI6tFVLaT2KLFxZNHvWLC20wtvh9Ofedt+dZe+dO8feFf04AT13UlUw3ikeN9nYGl1WpQiFouxahOF0narsUNkBktP8GGh5JnMnRyS7U9zJrZLd8lapadXRTVVHpaaqUnW0mDuKoQcZrfWFsr3khTRFe5zyWpqlyQqLpnoamnfssNnKNlkRckrYhaPrZ9zu3eLdzTzIl8tOSwXSLMivewetkRRGiuvUYSG2mWGoOFeKrTorzVrP230S/7aiDqR9g2ZJvHgF5aKlouyUk0ePer1IR74u0jb1ONI19YRTDJOYFCOT3EVaRzMUiZjcvFww7mJFHVmDHElGcdUvxerxfz7Ix1yiub6vlMX+ueEJ04pCqci5NHRhPVtcSIIcFxFbDy24yOfZGS7Smay+5HaFZrUIdbuk9BbkdlFKff5fWrDm2Wfx9+yzV5jNe+nKFe8lZlOzvUe8h4EjqDqLtWRZRd4J3jneud4JbBGbwqayRbzfXxApQ9AfiJMnootcpEhF6gydimxGohYnUyJzuI5ZEse4xFWUm0xpcZFPfXQRXdseIoco0tA2yW61VVoWH1Iv6+19mt1zkPWuXF+sTOhZ2vPy8WIhH9CCSm/0OY7WetKjY2LlenFuiItbVZUurufcK4KKwpcqWA3JZZeYPS7KJWvxfOJHYOJHWnMebZHFTD9WsXu3mOSiPQEsV79nJXEud1RbtM7TYoAyUB2oT1WmqpNi50brWCujlRgozbhHaJI2MWZC7CNxM2lO9MyYmbEz4zbRplj3UBqahm60ak1tOjFogZT6mt6qE8tqoUAR6Bphgd5T2QeMzBpx64tzhh/Nn3ps0DcsvNtd0d6LxcXFk9nSdg+u6jV5ZZebD9/Q4pt3794wLt77nej/Goz5BPS/IY3zNKOIMPscW+KcpLCiiKAi23ItrihpecpSbWHECxmRcWEkh0fHNUhyxcnhiTYtg7Mhsr+fAzbBAbAAUzVKiFzFmYvQc19DzfFf8CWTeWy5CSMSRyTlJis0lCWwiHAluX6D9FYJzNRujVkr01Grg3LnpS94P/R+M2zfmP77H3x7X9mGrTsK177w1B1vPzzhwOCvmfNPclpi+ZLPfkxL23tDi5WLnyjcOHnchGmpDbYnJX207dHNXLZzMc7rIVcSNMwMTzwLkoNIloO6kOzQi1Qmz7Axp53iNENxCv3m6O9X4k7esWMdyitauPnInjnWoaIF+iKGVjmA4T3AB7WRgxpRTxpM99FkepL0SNaYGrDGcmvWl/Vz9gsayPLYRDZVns2CMJg2lixnuTGNha6RNa/EvK28x48fqBqmplV+JR+pzNrkLWI5e8UYrcUY5aLt8TTMk6LE6O45rviYIj28yDU/SCqiGUEL9fUJUXHMLseR3aUluCpZ4Mi4ArS0i88ZDJKr/DyfxnweY4C85eb4cCXk5lyniHCqNTB8PD6To6uKmgxqcpmleo95fxi2d/SQ3fe/fPDgy7c91189XuxdFhLiPf+3v3t/Sko6dEPmjjVrdqQ2EHplMdq/UuiVVBrkSQ3TKGiOk4oitaK4yA2uIuf8+kvjFqY569viohPC4uTkxNg0KBoI0hmhas5UnqkRIU847FV2RDoiH1EOqYc09HxbgjSUDQ1cJFlEM5ZSX5L9XUlJ4mopuUWktH7eunXzAGbr80yf/UdD2m+7/wumei986a3ynmfZLLbPM3L7nc8/9+abzz2/U5pSmtrA+6P3hzuHen/47mvv34SiGsk2JJhr5CbI1GiMi0ajPPVUtyRLsluB3lAxJrIqMyh4TXdVHi4Xa1fzq1QwH6RBb8GY4YuDTjrGyd3mxsGe0EES0+QYta3aU71XLqESTYfMYHBYCkveJO+u+vIo81ZlqccHXp6hNuZtkWkBeLxA8DiFmtPNnrR64HC6VpTQtCh0acLC9Bcy6zlTG8VFpMaF2KDJoc5DkmMzXZWwTsorBHP9c1b42mKyBlodzaB1UrOE3aGLaZtSPxXWR5g/AeRDWrBkw4YlSzZu8G6YuZR8/3Xau3TGshe8ly5d8l5a33PprJnLl8+ctVR6b/XcuaufmTN39cCkbdNf+/DD16ZvS6r//uIT33xzYvH7bMQjM2c+Agi5mYE+zUWf6gm5SdETo9kcii6yb1CKaH5kYpFraeTCND0uLjksgerXjwsSYoMO+Feor70/+aUmsjz63Zjdsbvjdse/m1CeqBeH7gr9NlSG3LQRMh4aFgyJoVYtKcuUlfoNmL9j4MIXfdbcAmlpt+2Bz71XmOtLJjO391Xv2T5rWCdLohIhKyyIhQ68m4V89zWLFIvbOu9dCdIqvzzxPl2A4OxVUoQNG+cJ1mYpG7G8QwEpVM9wwRZpwVePi+YizzXEhaNH+VKvpHgte2aYehJ5NOrnaaytIZgesrpGUWTsvSA1a1RNklgXTZUlUpVN7EVdk1IVStF50aYdEGXpLgNiqFgwII5hrVgEa8WwmbvsVTT5wg5v843e5jvYg2IsXHy/KPSnnd713ERuGC+qIvF1krntsp3cEvSpXcfiqfFAm1u2GzwCGlYv5PpVtRnYF/Ldhk21YxUvj+KTosOZYxV+bSoWympifO+fKmb7tiU5GRvq6RLCQqQQPcQIoUE0icbRQrLpzJA02aZEsmhpIBskZTvvZaOlfDZJelR+WJms5xtz2TxpuvMp6Wl5pRJlKmBuAcnJcoq0y3teSvNOOyu1/cu8quHzjqvBVdHy1suNWYF3hphbBzDPK9B3g9yUhLmVEk2Fdlth6AxWaH850e0wpLDoRJWC4yLV6LhmNooLVZIhiS1gDYq1UBgEYhfQNnNbSH30AnamKV3VjrTkwMmVzJazri88++wL3l2s8YqlS1d4HZJy7vL0Rws3eC9cqfpGOlD12dwFC2dLed5OYx8eP27j7lfnPx+edOip/X+FjEzwfaWmY95EU2tPTNBzwVvthW72HG1VCqOWuhfG6NFBlBnuiuFNtKaKuUPJ3B4SmxgroXlcf1o6s3WbiOBqT6Sanndupo+8F5iL0cxzeWO+f8L7sncqm8PumPO9OvL48GHefd5PvSe8+4YNP9qzJ1vHMBJsXQ8hQ+CjWmLxsZknggpt4KDLkFx2UqODWlCcTQkVFiZ0kck0zINtOWGCYda8TEsWNIOx5RchrYneL7yHvF1Qzza20jvam+0doTa/MpnVY81YExa10bvKO937uHelmDt8HBegfgevXStUpEKaYRQqL9tVZtOxdipOzpJj5eXV45W5LTEItYt10cIBuaQqRtpX1Vb6pbITX/a6F1d9VVxdfgrKt1GGJ9QqX3nZUJko3G4WbnaLFx3iCCw65YA8pGqclF1VcpCX2rO4qg1ZY8n1ejy19SSRGssK5dhCI/Q599aIwuClxsIEieLcLZWsetEOFxb+isozleXVY+o9xtV6ZprYz2iKfxSVqMDxVfZ6d0ihE71fF3mf905kC9iwZUwfO65ygfe893sWxkLv33ScLd1YVXDHAPY0e5A9xJ7u2f2T4TneP3s/8v7F++c0f9/V9oK3TTzhRqH0skIz7Bo6rt5oY37WVgrt1uEMHJnbsgVnYZ67s7gVBAYclP7r4MGq+uh/1Rop93JjzmWrbLZc7HGavUGvSLw4hRufLm7RkNgFiH0R8wRlqh41W81RF6vrVI2XjlJR3uXG/jaOEXuLHzwNDbeqqbpbg6p0+zVZF0OVZJlesWkqUzSDV+QwR02YflDOfuWpBCgnhSsnQ+bKaVm4xBTJZkRKDdWGRhuptdrS6CF1V282Bkj3SpOkyeosaZ662FghPWOckyKgs1SbFitH6yo0pV5Pbqg21hrprZXWamutlZ7pvEn2KN1Uj+bRPc6Rcg6sjXv1yeo45wJ5gfonbbG+2LlaflZ7Vt8hv66/J7+nfyJ/rH8jf6t8o/5NuyT/ov5TazJ0PA0dD0awZK7zBJfXMqUqVo7x/lyVxXk9X5pc1bPyK+mDqhuoWo45n1RK8ziFELM4uR0pfH/LOX2mItNjy9Sz9enydEUxBxET46D0SeVw8Bo7K1GGlogynPSOp6Xs1g1dcjPJ4ESWbHYbFg27rYtdl2QDDDccWB2wNKh2LU7pZAffg7gsc+3J+c5t76iaRUIsDYZlRW0bF8w5P1DmS4JNskdI4XqYvYHUQE/SG9iT7C31Vvb7pEelafoU+3Rppj7TvkSKVJhDDmOxcgprIqcbDW0tWQd5oDHYdo8xxjbJmAK9tEguZM/I4cLuAuMgoTC+wD3WlD3GCljT97wFh7wF5erxSkP+5XJjNbGSFLr8RfVcyBJ6YIonQXfzPbkbu7Qu6Cy6qmpMl+KU1rqlEyrNow0uXW0DpEtIVSJXEZ7M1tKNek+ph36flKdPl3SN2bQIFqN1Z720O9kg7R52nzZFm82e1ArZam2dwyVaDZXpFgPOXNLKcu+FqjFo7ZVE5YvLjZUvriRCH3PdciJgv18YSoXmfj86JEuOjnDVE80L2O9zlZEldvrppvoQ/+X0U94qJp86xZjXd4q1Y/need73ve9557Ipah9vqfes92tvKevJYlgs67nee5d3LbeM2HrY0rCm/WuDskisDWHUzlMP6wJfHkJddkNS+OrQ2c2Xh3BTi5hiIXb8HkdIRGJE54jhEa9EqGKdqF5PsXVUGoMBbLl30erVi7w3sv1XeAuveA+qzas+WDZ3zrKNX5387MuqTdbahF0Mao+jVz2tYKvIds3NjSs3jKsumkIRshJRaAsvDJrhUFRNdmOdjwxW7dHRirtzuD3OqcSLxpXz1rnN9asDb2JoW/4baPqLc4BtngRhzkwNYyqpTIUBoysRFMHCpUg5SkmjNJYmNZDTtQZ6A6OBLSmhNWstdWfdpdHqRGWiOjlsnjZPf0p7Sk8cKrbSUWEpcjPG++tOTuKmRDUr5EU3Tet05MQ7vRfknzrI9jOqnFU137ussHCZtCtyyePe0axg5ciq+erxjz9dtFPqV3V+7qxZs7kc8/Og5yEf6fS4p0OQUwp2SAmJCYZN0u1SYmJCF7sjIVGJYBTxXPiKeoVupZBWpMHAaJhgdyTG6lQ/Njq4qR4dXr+h61Q55OgMLHHBF5c4GOAHoO9XT+tgzhWLgDkhWOCH7kjMaJ7RL0M27RFhiCde49CgOfPvTpSeEw4P3/Da5I1Tv/zE+5n33Jgfpk+rePjlXXNXT/vyIIv66b6/quvfa9N6+qRR9yRGNz6x48Tnmc0/7NZ93uMPPZpYr+nuze+fwYaV+S5DFr+FLOjUGxa6qQA9WMI9quE6ht2okL0Wmdi/2fn+zRD7N4MM//4tjGyJ5MK0S9RdNo9tnG2dzTZUtk4WNeWHqvOHqs5jkb98XBXr0jbMwwzU5yaPJ9KQ3A5SC4MX2mhGqBFnvxGr0E2hNcsd38xbk7KFZSllsh2JYYvD1oXJXBWbWzJMfnN6bju0de+7Ww95T2MOnvWehsKaiC3FBXlB5d3eU96PWSOWytvgt+81esOTrvC1UcaG1lwdZcRDezPqIivsFeJGPKmwavw2PBTXdXRztsFlfCTJjeQeSg91iPyYPEvWNdIlQ+E6LFyKUWLURtSANZAylAw1TUsybqQsliV1UDqobbSe1I11k3opvdQe2mAaqOVJ9yn3qVNpEkz7KcoUdaI23XiKVmkZmAMw6G2w6aXeVe8fZSfYX/9StQ/6Lkr5Fos/o65E+ka+HrFpnl5qjKZiDVJi7DY5xu6wSzFMcjgw37FMYb6r1jLlRGo3kbOLHWaBBt3tMJwOu80wH5o4dApyHTscZenuFtdeoKpp9TaGxHr1oyZpqmSHLWIPtTdUU7FSdZI6qS3tmfY+0q1qF7vHPlgaI92v3mvPsU+TCqRH1QJ1un2lVKjG62STsGoqGhQHYTVRIHu6jWyK3e6k4Bg5Qokwop2u4CQlWU3SkvQkI8WWak9zJAUnBXeQ2smtlCw102hta+vo7MwM7k7dWW9J2BlqFyxSXQyP4bF1td/q9AR7ggdJWBed2cF50r3yCGWkmqPl6DlGri3XnuuYjHGYJuXLk5VH1CnaFH2yMc7IdxY4C4LnSHPlecp8dbbtScfi4FXKuuBXgu/iqxIfIj5KKTaW0vUwloq2X/F/R7zzvVgv3vVixEKV8xxYU12XL4j1tGO1bZnn0YIUjexOiN4p2Onbp1OBXRqKmSmsNj4OmbeUdMke5AkXpp3NjdEV9h0GEtNKd1VU/3nCEaWTYVN0Um2KxiS7rLEQ/Ay2mskbyWacYBPYxBPeJIlOeO/2Dv6rFAGb6bjUuCqr8hdpWtVsOZ638W60MVGs+Us8scLeMfiBUBcD2kMuVDFcrItCmp2fLfKHRnZxNKeZx8Zn3NXbndonRB4PZESvp2fAnDFNgJ6GTZUdBjki5RjD5WjuaCW3NTo7esi9jX6OAfJgI0++zxjrmCznGwWOdY5I6+CIHx6z5AlKYWW2vO9KR7mk8l71+OorY4tXK0s5j30V3ngl3LsFNnbI6/QS5rvi4vsgrLAMWZXwK596tyxebD4nmIZ1oakyDbKbRrs86dGJjihbML0UpZUFu5PmJO6MK0spdS+MclKUXC/IZjgSZSO8WwOsjoePYZ6YfS0/c7ESRsX74uTJzRdIz0OZ8ZkJmYmZSZnJmfU7p3viPQmeRE+SJ9lTPzs+OyE7MTspOzm7fnb6uPTZ8XMT5ibOTZqbPLv+kvSi9AvpCf6s/kz+DDkJOYk5STnJ4xLGJY5LGpc8PWF64vSk6cn1As8MO7I27pRW/AiIP1PLSg48gY6U3j69ZcbYp8tKSzvvmrflUNUVJr24KmdH/3veHvKPC1JW3rSRE05sz+hTNaM4b8Se59/aHVqwoFmz4vT0Ss6rneDVei0cwhdHN3qi5TJniK2sXsTCkNLYVdEUGtqjnlMzYroL26HFRbGPOcNP5N4/n7kjJ2F6QlGCjHb6z6HQVCYONd0uCW1N50dE8tkXly17kaPqT+1enXaYfL7D015tV1YmNT907twhQLo9d4R3l/cX/O4akbsJrWH8Oah8DmMYTZ09sTSHzVOC5wTNs5e5lbKoUn5IEBpEPcO7xbgqz/gPCVzei+ddP53nJlesK3Z67JLYoliVBSzOWdZhQX3rsEA+1/fZ7Nfef/+17Gf73rphaBVWm6ZMG/C80mpL48ZfHTnyVePGxamp6FAwC2XtUoRsoV3KELTQZfIrpoyCw8tUY2FwKVsFs4gMqYc71NEtXpwTtGhRza/yWvziW0oxnJIwWCNZwDml/HxpabtXHz3kI9+hR1+t2gfObdoE7sk7pGH/rNiUO4J1ZQZ+u47wRlgMtNpVAH6FUyyN86TCTrPNMeapES8xtczJ3qxXFlrqXBgXGyEZEQbdIoWGdIsTTSy3HvperDAPsS+a55EZnePHxRfFfxh/IV7tTJ1ZZ6lzROdYtYne3Ghua2IfS2PZWGlsxNhY29DxnMXJwtipOYqBCOiC7bpSULnNeeSNMftGjvrwfu9F7z6WUfkl00ulDfNWlwVLw4a8va9ly62NmrAbmR27+Zu9n5Wv2r51LddZzcHwX8DrMBrsiVNdzGm8pLG5tCpY22WXwnTSbaoRFOLoE86tDzu3Phx8s80fcXM3110dyis7lJeHiinNt/Wu8y1ChUHiiciOKIrgphsaGc9M4yelVRafXtIvJaNuZc29H5WVlGx9Swt/Onv0qMWVzeWPFvd9czPntXegMgS8dlBDWGAp0c54W+icsMiyELmsQUpp+i5bWchbMfENoslw9tBCQ5O6ZYhzbFMcys+YAuE9zjndFlLRaHqjokZ1ZlGUS6qxITsyS1RCISpRrbLk5zcUrtiwYUXhhlKv9/KILbfdtvb217e33fbonysr//zotralUsf9p07t33fq1HfeL73fxie81qTRW+/cNWokljJ+6t9u5Khizt+dsCNzBX9bYubbSA5m2txgd6lzlR1bYerLdWN3saURE78DP4p3h8KO2JYTIc68Utxmk+HIEs9lIpXc0kcfLdxSVtbltYl73pfWV90trV239u31VXO18Kq19+T+wOfQHlQ+BfXyM+bGsGDfVl6lXZLKDIW6V58xn6nkmydun2bbcmCjqmIfL46c95TiR8m5UqSFf+vvxxqUZ4e2z7j+uckuWuU/ODGoe+2DkzPXPThxiVPd4YpkNyKldClDbWwMlGBtGBOkyepMab76J2O5tFJdZbwghfLTEskh2/WGcrrCz0oa6x7naDnHOV+eDWtjkbZYXy2v0ovlF9Ud+nv6x/ol+YJ8SbmgxPBTEH4Iwld18HVnmZT2XdVW6f4LVfvKtPDK+9hXVRertkgpVZ+hvzX8q/8GrZJ4b6qfvXuCXNYR0zj1ArbygmlgmBb+zwqLV3o8ZLc+DfE00EJt9UJIi9cjnHPjk+TS2F3RLp3cIYahZbuNkOy4elD9KWLbWIldrXhy3KHDmYviwIMLgicsMzU7dVzqktQi/L6TejrVl2qDZAhZiAiUjxpBiTAFJaPb7pmvvF328MTFG8senrxoY1lZ55IpUzfL8x+d9NOXXGyeW8PFRlr7/DPvvFA1V8nZeu/IR83zHyG36EMYta4tt7uuLbdn/HK7PSfigwipruRG/IrkomouuKaOnSjmfRTmfZhWFkplzlJ+HhEacpscGtGtzv0DT0rn6Gk0TSvQC4wCW4G9wDHNWRBUEFwQUuAqcE8LLYq+EO2u/WSw1jWFCSu2bC5cvmXL8gss1Hv+wt+9PzC3fPrcgQPnvtm/79s13v3eCu/3UKhtoTfD2Y1ifdoJ3bQebeTrUydPrH99Kg1eyN6Sd8VjbeohVqmAFd115ox/ifLYzDXq8wSFDU2rZo61nNda5ieUldWs5tKN/jV+U9VWzV4csJ6z7/yLlH/s5N5on5syPeEa9ihuhzw3uNS2S7dr2CZ0D+WqUsx/rE3HDvPFaHs2to581Mx1vGbIouTeib2arHkRLdk5O6xZnLw91H3o7aptGLC8Uaoq6hsLO2If6kunc9YZwR3WEcEdNUcEsC/mK+FzIubX4/ZFWmnNGcHtsUawboTX79aQt+tYrTMC6PCfuMERWvuMwH9EQOlccTwYZ49zxDmbYdFs4mjibG9rb2/vaO90JFESS5Ua2hs6GoU1D28e0SiyYULDxIykjOTU9Dn2OY45zjlBobwHkqTZNYfslIPkYDlEdsnRcowcK8cp8bb05hmdM4ZnFGRMz1iSUZRxIaMerOnxdQ8j+EWsuocRrcE9eUHfTUPmzx+5onP5hkufDtn7QN77I2YuvGezZ/NTn/85b7vSeWvDhv37e3olBzd6ev6aHSkpb7dqNfi2W7LTQlILZ67dYj1jbgOh+1Fdi7kIayhYNULkl8jNdhlz7Q5wGZLmCg3mc1EsxC2sbYR5WQHryCvmOsJX3/DI9nwtbtCKr8JuNplN886+ZcJbbx1/fu5cda333cVVRfP7rl73FylnMetk2vlbMR8HCT0QTu09cTWaYKGd7QovdUIPhDv6QiN0j+ATs60pV2daVKuDsRG7uToIcwecSlhmNtvK1cHLpaU3vzpxz372AdspbawasW7d2+ulaVeKtuSNuiBvsvZ+sLtySKMrnnRrxWGSyoksadj9YoOudZFkeocfWUhMVUjnN4Ts1c8G+DUIfl/nLv/pya8cWjDPn3pi58333HOk6dJSab1k8Ipssk2cz8XIMUoDasAy5AwlyWhFrVg7uZ2SafB9dC+5l9Jd7al5jIE0kA2WByvZRh7lsfvk+5R71dFajjGRHmHT5GnKRHWqNptms/nyfKxcc7SVtJKtklbLTylPqau0TeqLWomx2zht+IxO/n0zS+m4lw1jw/Z6776s5FT2l7dcKRIyMhAsaAUeOdl3nl7qAPNsY4DdJg/gZxsDftPZxjvXONvgXLylxM1vOYXyf2H8n8NkJOcs49cexTUZfjhVzd/ffSTCPD5VipQi1fr2VvZeUi+1u91jv0u6Sx1gz7Y/JD2k5tmnYDSmqAXqXOlp6Sl1hX2XtEv9s7RP/kCNVyWbrCkO1W44bCDOCClajlRi1Fgj1hbuiHDyk9QUKV1OVtLU+lp9Pc1It6Xakx0pzrZya6W10ZafgUg95e6KR+liPmsxutq62rs6+PkHH8eBUrZym3q7druebdxh628f4BhFueweaYx8jzJGHaON0R+yjXDc6xwbPJEmsinSY3K+8hjGt0Cbqhfo+cYUW4Ftmn2S4zHnXP70J3gVrWIrpOXyGuUZlZ/gPm14mq90rgveSBvZemm9vFnZrL6kvaRvNtY7Xwl+XXpVfkt5Uy21vRNcLu2VDysH1SlCJmIZ/2MpDpYysPTrsye+PlvqPXni7z+egHSslMdwXCmSV1aOgYy0xzyaAhlxsJs93VX+OEJxy4rOiaowicluCcPuRkq722ZnnDjsEBmbGwLTxa4rTDEwxyTLhSnh9AtIiDX+QlT4oYZ/1tUccJS7o+o8QKsrElfPwqfsimKPUSLsDewdlRvsA5Q79UH2PPskNlWZpD9iX6TMtD+trFNW6cvsS+wb2UvKK8oG/QV7kT3OLisq5oAjRo5QI2wxjgy5gZpma+RICmrH2spt1JY6P/vKDOold1e72Xo7PEGD+WyVBst3qgO1wfpAY6BtsCM7aGxQPisIeoat0Dez9XpJ0AdBp4N8Qc359QEpRRwPYVoqud77WfEJ707vzhPsNe/DJ1gGy1Byqk5X7WGl3p5SbynSO54tFroMtgPXZSFsgedm3ZBsbgrhbCYKCXaHUEiQ2xlEnAQHYeI63Zi2XYIcNhc51LnyW8GOXa7gIKfdhtlqhCghDpd/AAzBdkcA2x3mZTzBdeuc2F3rIUSd2ah+H9WC8/yCRqqh2eSgSHtUkCsoJahVUC97P3vfoCG2IfYx9rlB04OWB4XaCY3ATHMEO0KiWITkUlxqlD3cEe6MCY4JSadUrLxJSpKaYTS0pdlTHanO9KBGwY1CktxtoC1bSZlKpnqjvbWjtfPGoLbBbUMy3TeRh3kkj+xRPNYM7GLrZu8R1Cu4V4jH3Z9uY7dJA+RsJRvjMwDjc6ftTszCAc7BwYNDst15LE8abb8v+L6QHPc0Iz84P2Q+PWmb7ZjtnB80P3h+yNO2Qkehc3Xw6pD1jvXOzcGbQ0rcH7hPu33uezCWajAzrx12ZuJsUlred8Wjyx/o0z8r2dveVLij909d3XNOf6Vv5Qr5AXNdHgQ76yTG0kbPemIM8+4XpksX4yXaJb+kGjIjhZnHffwqobPmuM+6Oy1mSXmL8use/XXhOrGB1EPqpasOI8RRT441GhtJjtZyWyPTwfnVTfDrZuNOebAx3JHDcqQ8OUfJUUcaBY7pjlccsbUO/8bLY6r6SNsrH5O2V92j5GyqPLl8k5zG1/lP1O5yhuYS+8Vl/InHnxU6YrBcUnMVw3WqUlyt59vGTDIFjl+MvPq5R+ByIC7BR5nJfLvNZOiwlSwEyaKvWYbHzbuRo+Zo49g4aZw6TjOGMmxJ0wBp2KFD3imHDmmugwcPClsX9skW7NOa02pPZtP0ZKeiBSWR0ihyTlRMWVijMnlV2MJmTltQfFJyus1ITTe0eCPVFdnUcFF3fvWt8rDr/fPHzLtv/Bkdt1685/nJAawXvvvyhKghWogekh7S8Ennk0Ewoe06n5n2IHtiUJI92VlfaRAdFJ0YndQuqV3yrYm3JvVK7lV/TOKYpA3aBn1jEj9jDBPGYFQw+9cGYxu/8b3zh79+eFJetandTW035nxx1DOvV/bCmx7Jb3/P3Tl3vrjKmDV+5rw3lfH7T37zuTEhp/ltjdLG/Cl3yxvR9dYnxA+/q3P/Tm3az72rYEv8veMWzLqyHKLq85nntZortAF/CuLWaMztREnbw5s2dOiNPREFDcc2zG46vKGnab+GmU07N6SmIQ3tQ29APmH/iXyDzHzTiOptl2Lr2ZEvyBPbr15mbOd6FBtSTxt6A7+LTtLgp7/K9/11eEiHnyjR4DOFPnqs6qKfXvq4sk/wYBt/xcAQs8icS6Q/6I0nCvZe+vjybcGDrfDqn3q3K0fEe0kkFQMLMPOgReSt9J62ndaqUVSsr6bxWkeaIWXRe3IilQDrFaKOiD+B9GulrygX9KS0jQjp5wJfACuBNUAuwMtZDGwCFgAzkPYCsJaX4YfSmZaj4XPVKeRSH6MD6kqaoGWABtMBZTUd0LLgV+iAdDeHb6XaGeETEX4OaSpB+9AE5ahJ1cUIC6e5yle+y+pJ2sbL1L+lruo06oiwStC7eV94m0H3ifrJV4F+FSvnaBry7lTyaDzoeKWCxksfUXPuVkNpp9SW9khtfSeV5023foh28nDlrEi/k6eTe8PfmMbKKdQGcVuVXeDXAhoI2p67lSwapEYxkrYxhVOLl4L34M8WziNgGHA7T4N23Q18YhCLld9DP8+avOO852GIOw7s5WFyKxoGjFSITUD+rZz/fHzgT0H4fOTPQf49+h6ab2EkeL9Y8P0aQP8MPhZ8HAKBcWgPPI+x8IJqGB+7fxyuwnYWDZonxiIAfCyUT1CeHfwC368F/SRonjkOgcAY7AP/l4D+F3BR8N8ah7oQ43uWevKxCAQfCzHWnKKvYuzrUvRdyMJ1qJBRjLnoP5cRLq8Vv065PFv5rk0h62qo76zeH3Qx5YPPZ9DPo+C1DPoj/D+BnoG/BHxYKeYF5FEpRfkPQ0YxR7icinkCWRWYaKUx6TxOZbL8u0ALUG53kvg4cl7WpdpMOlLt7iPkcHxdaiymCUZz9BNzkM8Di86s9vN5iblxPcrnLJ83damQGT5uv5Hy+S7mHJexXTXzXsy9OtSa30nqF75VQvfwefwY9Fk4UITx8I81xlhbVJ1GyBbGcxb6PlH5G/TiavD8I1+BGMPHydBPQ0ccE3PFrl4S41AGvtt5ezCvtqmV0GMWL/W+dC/Km6SvwnwJQ7ltUE84lVm67GHwJlfMuxLvjyZfqJ6fP9pn9DLKKdHiqa9ajvT/QF8/hUz7+9mfioC7lXU0Gv7xQj/3p6HCH4F49JfLj3wB2ELh0lA64MihA/ZcOmDrgH6/gnl9C+JehN6YQAd0hGsjwCNrjggd0Nb3uV8GfusYiflQZ75xfcPnfN35YMqx79u68sb7hn4M4rJeq81WPoOvDxPNNULIct16oJeEbqg77+vMV/TxRdSxF3xSQb+6qh2LaV8tOa/b5zryrSq0RmlCPax5fkH9EjzdLvTKeOVLUP/Y1WnP9eadn/rlXT5MT2pv0075I2rDeaNX0ngOdYqvCnU4Ic82zHs70m8T7UJdWD+z5eOUDfm2o91OsQbU9F/oE81jjcdisqOfwcj/M+pzwI7YKsLNNXCncg8V+NdQdVmN3tb+RI8qd9Bs5SaarbWk2Wq20OUn1aVWWhvSlWONAiw9vdNad4Ol12mj9E96RG5Et8hfUx+pHe1RN5prsB9qY5SVIvK8JvjyGco8SivUHjROzsYay9GPn+SCN73Qzk70BPCIcgzuY+a6LZX4TnDIr4J31nyz1nJS/o72HYCurFnToVsgQ5x/HOsEHuTzKhBifF5Au9BftRhojz4N9P6oDkSdwQj/COVaaY14yO0kIAbtX485/gW10doBB6CnNqDPHVB/IrXmUHtDR/H+dKCJ8g00keX5vpVCaSLmcE9pGPWUDUri6aQr1AD8KoJtVwR7YCuwDSiXJiItx08mYCc4TKCOAMD++9i0M9gEbifV+Im/rz4BttRYAas8hCVyyAmwD5+kXKTbB/9q0POgfUB3ABekOT4f6A/yaLS9P02VKtGPRWZb5B/p47qw2nNcSYP+EGXRDqLKTURV40H3ANuBE0RXKkDfQfjzoJ+AtgHlYbCZK9+DfxfoBWComY7Dm4jwJSZ8U2rKrUoFyhE/AECequmAw0KqRacCk636joM2BMYAKUCfgPpGmfX76xQIaLPAQqTPJ7r8PdyjQSF5VVuQ5u+gyWYZVY3RFs3qp7//2822V54Dfd9qB+9ThEkrdwSAl5Fl7gN4XYJXjU23rxn8vJxxtVHVyHJPhgweUBbQHu0s9FczrEuQLQ6hZ7Mg08R2+HUAp9zet2TnE/VJcnGbVP3Fd077xfcPuavve22670ftad8X2jO+k5jnqn8fwG0Tvx7iOpHrSz6X+HrF1wQe598D8DTC3kQavhcQugv6lutEsS+A/S/isU5ym1XYBN3RPugjoWOgX5TnqJCHqbG0G3M7SehUrq+G0P1++1Kke4PeEXYjbGwln3ork+h+kfYj6i303zZhj3J/rigT+gd6oT2n2ms0l/eRh4s8oDxMrHF/Q9kXkXcV3am95fuCUyvPTZjn46rXm0xawOvgeyN5s8+DNK8B72gV9LCq0mQ9H/1EmZob/UZ/tAEo+ztqCrukn3KScrVUhBP0x1P+dYOaKL2h41CHf/8j9D2vz9Td5cJW5/qd7804z1tRAfwD/DaSoNb+QOsNvn9h7uP42mfu20jj64ixm/obd5tp1K3m2CmfU4pYC/37Pz72yI/15h5enrGWGqrJ4FGlNdbIh/T9eTv8MlE97txe4+POy/yKpohxb43wR+kV408oazfSv0Qd9BCzHqQfa7xAR7GmzRP7jh8wVm+ABy3R13kYV/Rfb0Xd+ZrFZVvI93HQeOqj2UDbW/u/9tbax2Ue5Ys14hOUhX2f+jDCd9JK/XasU/OR7kXqpN2GMF5PLsaH298fYh2y1kmMTXNeP48Ta5K577wo1vIbqY+eiTLaIM1xqz1cFlF/9bg3ogQ1hxL0J9EvL9ZIG+ZJV8qy9UD/ZcxbU47uN9qAF09hTYmC/w66S/sr9nwytai2KzwYj9vht6h+AbYq7CsdYw3ZGm8bR5OMtvSUv16/rayo/Fz8yl+hM3TgNRP/PCgPuvSxPOiXQRp0hjoG9T5GyeBBAzFunHcYc8H3POqhlNGNihf+jrSTjz8fAy4DYhww/qLvNTQZtCPa30J7kRoJWepFe7CWHtAV0I2gd4APGuRxQc3+TcgJH6uAfYLgJT8rwLjpU2BfPwJ9BNnh4xdIuT7Q51I47IsQP+VyXt3WzqJt72itMM+GUjN/m4QsYo/mL0uPwRi04OOLsOvYwwH238RAehVfLHvYr4f99Hr2Ipd9IWOYK6L/dai/jf5x4XOGy61/fPx8qqaP0VKM53jDSUv1ppCTw0h/kTarDyH/67TZWE6t9U3UjNvl+lvgBbfTe6A9zaELSqAT+T4K+pbPbT6/bEOov/4PyHs6yvkb5OAmmqd/RY8IfQ570b/P88uBsQHpO1EfMd590O9B6P8k0GTzzEHTaSgwRLibIiyRdgn352acOpd2KV1pl55Du7RvmCHs9510k5ZEmxCfq6XQcOjSbepfaJmK1VULwZrH02ynfO1eGqKl0QYRb9aVq66HrCyC/x8Yl1tR5qNIF2zOL+12ekjYS7DF2OdE0hlS2TmfT+5EEFkagrE37d+bMU59hU0rbGwlwbSJ1W+sOL52NcHYfIL5c0X4RT7lM7pXDUMagxbyMKmJ7xj2GifkKtiMiIfNaOd1KNPoITXTKp/vnQ9a9bpprDwV5R4U50gZkImx2njqrj2OsvgZ3lf83X+pK/++Ej8ONcH9bJ+FUSb8P4zfi+vL05h52SjMl4/QmmhEvsfd8jx+HslGqYPR/iIaJPeBTTwM8twOfWwGvGe60d4ydhD6mse3BxYivB/Cx2IviHRyS/hvwP5ZAgW/FB9wG9K9A//LcD8BuhnoQuFyOdKPpHnSBpon34EyGgLRZqswVrP1D2m2VMi/G0KV4iytMy2X99IL0MWvY84+IH/m28ypdjPNFGeC82imcgMt4JRDbUTP+iEvoccEkIfDVk4zBbaY0PNoCYfyPuY3IA3yVRi30AzokPuhp5eoH9Ji2AcL1c9pOa+Dl8Hr5UD7Tl0H+wHYifQUeNvPBJ2CjP1D6cNKgUjw8XagD/AKMBcYAHSwkAvMlp4WZ8TblLvpTt4v3iaUdUAaSFP9fb0eAnlQF9U8+Vew+CVX+jYrHYEvTVodHsjLOvzkfOQ8vBYEXwE9g2YaDyE9KOezH9x/LfBxqAWMx1VYifHi/fusdjv948XBx/AaY8DpGODDwDEIOF+/Fj628Kw448OeW84VOlnYBcJG2W3aKNpziJtBe4COsF257bJHOkId9S0I2481tKuVh0BPo6yOWJcOYf+MOB7Gy+FhAs0A7gf498qALpCJ9aDYT9Bdpp9Tthr0uDST9nNA5/B7cLnSV74KtLkE6+NMNZ8WqDNovnwKtrYG25L7p8OevQttqU8z1AyfT+0Ee7gbDUc7egr8TIO1+oh/nEYLPEsekYfnbUH91BBhl/bVFtHjqgtuhGu30kGEPwj7ZLiSDXsvuxJtu+KpjUov8CJPA8RB/86QiaZCX0yVt/qOKiPobvk81o5cWg7bBvuzK48DnZCnL08PulqMVxKNEhhKkWjvKIEiGiz6m4u1YQzdZ7Sjxzk0L+Wr/wVd/BA9pL1MD2F953Z6NtaRDno25ctFkIOfsH68LWzXfOi0mdrHSOOhFqqNsvVbkOcSZOpnK/x7yMxBrHV2hF1CuYQ8PyFuAcqogrsC4ZVIQ2jLYeqg7UH5mDvqTJRTDvdu5PmGshUXxioV2Ij1bQEo98cAjBpqo624CBpiPAHaTGCm1ttKhzhtmBmGPeMQULu22swv0qQKdODxkNkhIn8q3BlmHvl5CrfKyRfU35axyL8OdAzy8LBlZjvlQqypq9CnOs8xNG4/1MZkAb6PeBnxdai+C3YcbC4/5Xks92Q/5fklJ+yOQZDZUTRMIB5ujjSL7qSecgTN5+mq4wCjFHV0A4pQ1g80+apnL8cRdg3w9on+XLu9k69HeV7FTfPZfJpf9zmM+gnia2MKhz4MfY6jbVfRB0Bbomw/XSHolAB6QZ5C83UVaQHI4WQ9EWXqsFN1tL8G3QMgwjS+52sEG2M26FzAT/3h14ufjTpvAm9vohs1hvgshFn0f7zeqagXgI08mZ9XVIP7/bDCsBc7oDUAj38BjYPfT/3h14v/BfVEog6MIafah5CFD9EeEw7LPzkwXOx1e9BkYwrK4H6LcihHUM46lHfkqrK6/1pZRkezLEH94X5abIVblJcvZO8o3EfN/bmF7gEQYZDjA5qB+gaCNgb81B9+vfiB4M1g9GcoAKpuw7ha0OvXAfa/2uWrqS0R7T18fQodPl9VMC58D1eDyQEQYdChB7TO4BuXjYWWjCwMCL9e/FyrD1w/fI65c4fYr062cMCP6/HQzxvR/+NCn6yshQ/oVguTOfgzHK4XuDxdpQ9q9MIdFkx9YM1vnkfbgDo3oB8mugf6lZmIBy94P4yc6wPrQGA5gtrDaL4fhmLC71efhr9QyGtdOa2WaTUN/UujZAuTA/3gjV3M9QwghSbI74DXHItgH6I9dszhoBATDjLh98sf+Srkv8NW2ear0Cf4KmwtfRX2n+qEZVlhlQh7B2EzEdbNV+EwAtKNQ1iLmnSaCvRD2AtmfnWyr0IJgT0VDMptt7fIIZ6Bl1AncV7B93ifUKr8Pegd5n5Dbkgknu8WkyTOo7Ks5+B5sKGmiGdsHFn8uWz1c/EWtEr5kFoI8POPp5DvLPZ+hdjrxVDz6ucb/JlGK6y9xfSaOBeYhXw8bxnsCuzP5YfJrnxDqjyRCuQvgOYCd8jnsO4dpAL2KIfvLbkvFUh/pgJlMOLfs3AJaZ6gHrId7ulAuK9SLqFx2MM2luvTrQKdqIfaHPRBmsjd8kAT0pfUX/qcbudh7CHYZKOxX+LPDroB/RD/M9L1s4C82FumyB3pIfld2DY83UBqILehKdIV7P8ikOYO5PmW0nhZ/PmJSBuY5haa4k/Dz6l43/izKHUgtcAYLOXt4HX66xXtG04J7DPft6LdKE+Kol7Mh/IjqZdwf+4byP3sC7pLljEmlVYfeiHPx6Iv4/19QHndpVt83/J+wM4ZBlnuIZ1BGg/6jnZK56mN/Di1EZQ/r0Ie2KB31UEXjuozJvM5dmnAM+/q891adxt+hf7WOw/8rJo/a699x4FKLbrTehb6vcY/EhkKWbbC0Wey7j7o/AzUf6ehLhX3GG4V66ws3eqrMu85+C5a9L/4WTF/RliXXu++w6/ddah+5uo/u7RonbsPdWn/X7sD8Wt3IX73nQg+3v47LvzugXVm9mu07tlewNnoNe9RiDOlFFKqn4vyuwEYb0AS496Atokzx+vdtfnvor9RHq9HIWdDMKe7Wndq3vm18b8erb7T8Su07nhV3+f4FVr3zLou5XsW+SNKEs+z/hX8d71UUgEN+XTtPlLUYtLVv5Minn9dA2oJ4gF9J/IdJk3PhPsB5LOe2V8P2jaU/wrpRgmpxg7SjDZwjyZFz0f+5aRIr9MzwFLpdd+rwJv8WRnoUeAQ8D7WC13you5wUgFNWUK6cpgU+W+ky7y917gDJsZlLOo9gLreRb28vTNR316k58/h/gW0bkh3Be2MRhubQb7585V/hftRzzuo5w3Usxf1LEX+fcg7HHQt+GPxXfBxlPnsEXvjnejbIvFs0d9mf/1Wuf/uOP674/Lf1e9/1Xb1TV8lfz4s5jKxOeI5sqDivsCO6vZ2CGj3OOT5xXdOf9hXyZ8ni+eAsN2A7TwP+Pod8BXwqSVLZ4CvxR26u0mWj8Du6Or7HmkfBwpFXXVkoPpeiz+MzzH+XHkv8LTvC+hA3bwLQZ9wei3+6HORdrrvR30E6DO+k/w5tPlMXPRPXNz1U+kFfn2ciA0U92rF3Vz2NAIO0zV/xD3cr8QZIb9rkWuYQHn8/qivIuDOh6Di/kQgiNoKlLIsDullqlDvpAqUwfOeunat1qk+2mXfReODvqTx7CNqKFVRQyWDGga6pR3kkLNoLbBH20575S9pOT9H523THvK9yCGRr9jg54tEn7GB3vnWfeMSPYd6q5/Rcg75sugjv6v7qYWO0jYWz/Nzt/w0LeV9F2VuZzfCbr6s9qWGcOdx8PN7bQTit9M4cW8Z4E8qfs+P3IoGCpuzFXUG8oC7gAeAwcAdSlvIngV2icYC98qZsNWQT9zBte7o/q783BYeaNmzi4T92kPc+bHuzQi7kdfBbd1K096FQA7kz3WBHGA2v1cs7J0oqm9vhv3fKtg/31J7rTsNRxi/F8hlrSEQjvgPQZsBXYGhgEu7gSaCrufxwBjADtwMmzIM6BgA+K9kc7fRgG7m4DalUUl71RTfx/B3MOZjz/E3lLWSxurP0l79G+qFvYukHRY2F7+rOwS2ent1BerZS13lvr4zsCuStNH0vnE7teb3nhH3kLqG9otnaSOpizaL7tAG0n69Cb2k8vOJhkw2nvJVIm260C0/iTuQg/i8E3PvPNWDPuhafY+kN92tFomz08ewft6pfErPI6w/t1uNP1FbeRuNVn+me9Vc3xV5J8WqDTGeduquj6YhtkW0Sl1LqepfwMMOaNNB7DEfpWjYui/A/jQAXeiLRXQn9PEQ2Bl3SR9QP+kDX6TWEbZVa7rNfyfb/nP13exhAXQk0Nny5/nvblvuB5QFNN9/h1N9AuM60uyTPoJcxk/kss+H+05xh6ajPpk62oIwzybW3LPntrDYS75Ee9RozNHHrTtujyH990g/FO5FIqy9toLaY1/eXjxnsO74cbmy/UxTeFmcgo8T+L0fXj7aNxDzDXOOvQA60aKWnyXVhpibSENNgEgr3QYr34aA+Drh1XGT6lCerhEwBNgSQD+z4psC/YD/4joBOAo8W5NXVmvazVHt5/GTa9JRvlVnfkBY7vXbK/zrrT7vMlGr/7k1vArkVzX/7rfStYF/GGhPk1bDU9sv0k41Ue2fXLuuuu3lZZt1iPkThX1JCnSF/47PL/SMOsR3mQPuVzjUt+lEoFuNYk20YFrDoeZiPgS88yHeGanHnkR7VFViXYFBkL2O1XiDTmnFwHYWizn9CgfyYZ1mJdD1eaAuTtWT/Dl9DbB3mqhl00SD30Os4/YDfZnCIUXQc5wGtOvTwDYCz4v3Kog+rBP+W1C3rBPaDhNYoz4Ajvx/KLMu/hoII4dWcMg7sE+4Vv01efzuD+vg1+o7XAdvW+GB9O3A8biqjE4WttObvxuWbPmhNDJRN/wqXKc/GIMpHHCPBKagrPPYh+33g8uewBLIuAAt5FAlminuMEr0T6ucq8DD1VM0iiOAP38xwR4NbIdjBK3g+Ddl4Ys6/uMGySu5DReAQdeap3533XiLnuD3GoGHoeuX1egkE/I3rL1lq+3zUy1fuqjlQ4f4KX8HJxZ7CqJLYj7tRrrdNMdPlcbsFczLRrYbaQ2HI9uiCykfbqZV0kq+N+I2uH8vpIVQDE+DuBTogZLakBZdHVYTrsHC1og2mTTQTZt4W9DGNvpi1IV6sY/SoCMGq+G+Wbz/0ENP/RYoH/kqTEj1lI/YfvCvg4nr+Tn1uzn8+QPL+T3xdVE3/f/fUJcfPIzlW/58E3X7+3vCfwt43lruFwPg5/HomnRi3EYHtLeaaunY2/xbkMOuDlPHXz+udjiX398C9QETfr9yrwku94HARlLgev7fm07gCo2TL5oUeNii/xJKG4GdWn+0d28N5GjSAlGdp277sL+9Fh8C0xgXadxV8XXbEljuesQD0PUCPAw6YDP03WjQXKAYmAXM5lAK4W8swor1WHqMQx1Ojxkx9JjtEi20M1qKuFLgDQ6lC622yuG6ZYuFdbyOAP825TQtB33Voo9Z4byeXHUI8AsVqy2oWOtGxcrdVv3Ix6n6inBvtsJ+C+Yad1KxH2aY9BmnyrdYO06ZgP95vQm7A9gN9y+gClAB91Crfzz8HMISQB+02tCN7+OsuBLE3QR6APgS7gHADuA2IPMa4X3McHYzwstAB4GeAe0CuqPGT5/K79MWNZbziOXDvwv+16VTtEU+TS+rlbRFS6InLB6u+RX4+WyB3aBdxNpxDfx2/vJ2iraOAd6HO0jpL8Z0ijm2LAP0XVDIGlNN0PcWcrEfLTZsWNPfoOdteRiHttwOYkFY2z4AnQ5qAy2wcBng63R/wK7tFjbKq+YYssGgJRzYn+fD/yegK9INDARPq5l7toEW7RUQz/dFT6DM10AbAzuAVhYdBPB9QBbo96AyKC/r70ClZu7LAsBuB5xAJyvsTavdvJ47LPedFppb4ZmWOzMALcw20VNWOR4rr788P3jcixaes/CQBX+9z1l9WQPMtPwjLIhyMCZ5wNQ6KDb3lBLsdUmTVtBWIF/pS1uBfLOPbC3Q16yPcV49DhTBvdSEFG+ClQEngRSgLTAAwB5PKgcesM7Anvut9ospH/+tmGiNZyC9Hs4EwApjFXXSNDbBIkxQgQnWwRoDa79dPXZ+9wRgpWbu7TgmwmZ9EOjH1yL5Z9ikP9Mr8L8hvncwAfp3AmGvTncBgzXzvKCfrQtNdMC2Bfz0em5OJ2J+EOZNk+tDfuI/O/7/dfxv8/9/O/7/bWg1Z3rEoU6mfgKn4T5tfgfkWucIfgg7uebcop0f9tW1z7b+NXxvXyP8fvGNjn//LOrfPcP6nyj7detc1U/baNVnpuIc9BrxCC/BOJnoyfGv9grC1udhFylVgJ8ZmKjP9xEIu5WDv28vvv8w0feJcpTs/D6Iwu9Jpfi+8d91qb7TYt2p4O/bi3ct+fMJ/u7959TRplFX/VVxx2K0/z1c//vt/Lmx/D2N5O+B87tZ/C6JKGsn3aa8S3HKE5St8Ltyr9F9ei/KVmUi/VnqqeylPyknKVt/DvE/AXvhvg/0XcrWJlC+PgHul4G3qKU+CnHrsAby+9flZhqlFNgl0EK5hPihcL+BvfyraNNG6q5nw1+O9O+KMrLV+kjTCrQJjddjaAKHOpE8aj7drEaQR3lc3Ft0Vb/7G0yz1EngqY9Oiu/3fI94UH9e6V74FcoQfOxMnZQbzXi1ISi/16HSWLR5rNaOxor3TS/RYf68hPsFVWid6qJR/vLEt4aWiHu5K6vbx5+VpMKunkYdxR2py9a4KNZ5eF+Ezbcofz+/My3mMlj3bIw/9/wde6z/SIj3e607rPyZkfWe9mVxN4w/j+vsO67Ug73kf6+Yy/Bq61tQ1vve4vkVl+/F4hs57avv+ivie1EvIP+BWt99eoyW1pUpMfb8XUL/N4kmksHvhkrYLwHLlPfoFQ7u5mHKdhP+b7KI77u8Thv978Ea7amD7qFOxguQlV00Tv+Qjmpv0x6jgO7Rb6H7jXnYB7SiPrYH6YDhCrhb9ina8BqNt39GE4wGmBMGtdO6+C6rU8W7qeIdVf87p9f6LsJvhXSR8gRU2uuHeD/hBM3H3ncCh18X6Rrqf5na+N/JFHdOG9NYm49c+hc0zVYE+h1oCugJmqa/B94vCKBbTFr9LLAzdF8xBavj6YCcQnuUF+kOeQz2OI9ATz1Pdn/fhW4M911RT2N/1sJ8V1K89/iJGV5NJ5JDvDP7pXVPcBtdkCUq4t/R4t8r4/zi3wkR7xoPAK+zSEE5CtqhQMcqkCF+J0aB7ChybzMO/VO00b5VyrNobzr14O9rQ+bE/XXxjBTyYnuKurLX6V12jhZJwfSQFEc5UgoN4f6rwkF/Uzjy1w3n39iA/KwMhLKeHhKooof0eNCtpl9tCz/yKuNNv20w6A6gFPugi1aeN5CmnxmmngAtBm8vW+EZVnqOMsTfYLnfoJnKQTOPkgzd/gLcW7A/9bdjA+qORX64+RqhTbbe0fktSK2BdsvVUIZD9q8FfodwFjVX7Sb0XSYwv5trX0E+n6XNwFbbUuAx2ursQFv5u6L8No20gXqrkdRXO0FbtRtokN4ZctEE6+w7wCdwT0QYoxyut8X7oZupr0UH8XdS/bjq3dRPabDcmQbz91Kl9TRYCXwvdSzStrDeR/W/i3qN91D5e6u8XJHPJ97bHSTenzxJM6R2vgppjK/iv9sv3oPsSTPko74KxXm13/+OpvIjd/9+P393E3bMY9eln/k2K2PM9yI59b9fKX+A+u9He3+nn793qUWZ719y6u+neBczmJYoN6JNJb4K8X7n27TEn0/UX99qxzWoeF9zM830l+endcN/302ia/3w76vwH/6tFSJpEBn8HWBB69F9pj8grBb1XbT89Titfkd5nPmesjTOfFeZ98fvv6pf/DsT48x3mAPlRLyn2puW/po8/dvyUUce+Lu89ix+loO6UnwVV/n5e75H4D+EsbhwtV+8T83Hehj8S672i/esu/B3rdGWUwH+5qa/7nwQ7wtvofur/XXkiL8LrIXQYvC8QtqIMP6u9h20UOkFd1GNfNblq18u68pb3fFRlviaoa3NQM+CnlWWUBTaHAXaH7T/tSTKaEkJWjD06Snar0wH/TNorgn5CdjHRPv1drRS6kr71WiED6f9jjEICwJyzTjo1v3aj4grwRr0V+Sbh7BlsIXrIc9jcOfDNp+KsmF3K5OQbpIoO5fXy8vllKfj74/+b9ue/8lQv4dtewI27SL6Rv0Yds8o89upcirlyfV9KzUVYR1he2ZROewq/jx/nloMu3s9varuJ5fxGXXVHqYH1E2wl2+B7VZMK8QdL04raKxchnWWf7/sLNa8D+hr6QPfJ2or022rL94hMr+FU2xCPm19C7WM2qh/o1chgx31njRQHU19sMZ1hF0x6Ne++SovpFX/Hd98/b/3bVfwNIruB2Za38EdAqyw7ljeJL6DGy7uT/627+Va35So/laC9R0B7uf6TOiIOt+G4HrS/90DrhO53vJ/IyHwmwy8vMDvJIhw5Pd/G0FuCZ01EHrnzyblfuUAKNdFp02/Xo/rTbihE/XmFq1nxvnz83CuU1UP+jKS9mibTGocgf2OMK0zUGa6bamIaw3/zXC3t2iqGefPz8N5Xp5O5Eca+7e0/z8B2uz/DBjN/y/CQyf+r9ZXF4PoaVs+3WLcSR1tnppn4tiHDQ98Rm5h8TXC/tdwjTam+N3O41elb4f0OZzyvl4LRL4y65uLE8xvDVY5QT+wsM9E1WrQr8X3MlZiZ7akBn5/rX1KoA0WYH/549mO2unr2qSB9uevueXhRFhfjkPvhkjnvT+q+WxZAJZb8PsnAQuuQf1ujlkBWMC/DcKaEPHzLfEdGyDQZqxl740RtvoebiP6vw0rvvds3R0X70W2pXfE2QfWSW07e5nM7/1cC+J7QPy7qaJ8gH8nRlnGKfqdSx3lXE7Nd4+VXZyCJ+L7MZzWdpvffeG0djj/voz2HKcoS3xnhlPh7uh3i+/O5HMKnEX/znKKNh2hjtIRTjGGW6Dft3CKPPuRdz+nKLcr/0YNp3Xaxr9XQ5wCp7EunOYU5Ypv1XAK/yEapx7itHaZgXkD+xWYt5abf/emGad10ge4+fdGf81e015jq6q/hcftiSxzH1QLY8y9UCAC90DXc9faFwXuiQL3PwF7n1rnANdx19r7BLj5t5M0zB+OwP144N4o0F13D38td605cT13wF7qem5+HsjP4jm4PWIsoc849HWUop6hDcb3tMHxE22o6/bD1sP3iwl6n8ORTbf7Eew101z963uh2r2qeivW9V+DPRAAzFWppYV5wG4AMiWHAznAGWgP7PdUQOsA/AINWIrdHjSnLQ64QGQvJ+Kf8q2FR2vgzCcKagig7GAPUARcJApZA6A8l8eEezSwhSh0E1FYNoC2hd9tImIcUSTiIz8lioK/HtoSjbwxa0zE3n0NzDMRt50ovg+AviSgPYkoO/EboqQSomS0KznfRH2UX389UQpoyudEqU8QpaVaWEHUAG1ORzvSQTOgVRujDU3Qp2YLiZoP+v3IdP3n4oYbr4Fx/8Mo+gN/4A/8gT/wB/7AH/gDf+AP/IE/8Af+wB/4A3/gD/yB/9MufT9HVYVhHN/ku0chW3J32SxEIIp6aTEJrFKk6CaoCAiKAQGdOKJXRXTsHRcjSC8JAhepItgodkmCay/MKNhoYy8Uu2Iv15k3nr/AXx2d98x85s57znPmnPfMVUoppZRSSimllFJKKaWUUkoppZRSSimllFJKKaWUUkoppZRSSimllFJKKaWUUv8zBaFQh4mMCZWHJoWiocKQE1oeahMKhUsK0/Ybbimsz7b+JQQp/nT5I8PvPr/F+VX4RfjZ5ac4P/r84HJobrU5JHzv853PtwHfBHwtfDWAL2v4Qvg8w8EDteagzwEbPFDL/n1VZn/Avio+Ez4VPsnwcYqPfD4UPkjyfo738rwr7LXxvTn27B5q9uTYPZRdOzuaXcLOjrwjvC28JbwpvOGzY3uZ2SFsL+P1DK8J22YkzLZOvJrmFeFl4SXhReEF4XnhOeFZ4RkhLzydYOtM12wVWprzpkVobqozzXma68NNW1zTVJdtpSkb3uLylPCkzxPC48JjwqPCIx4Px9m8yTWbPTZtTJpNLhuTbLCX3hDwkPCg8IBwf5L7hPXr4mZ9hnVx7vVYayNrfe4R1qyOmjXC6iirVpaaVR4rVzhmZSkrHJYXcbewzI+ZZYIfY6ndtNRnyeK4WdKdxXHuCljUmDeLhMaGOtOYp7E+3LDQNQ11NGTDC10WCPPnVZr5wrxK5to251YzZ3bEzEkxO8IsOzHLY6Z9qZkuMxLcKUyfljDThWkJ7hDqhduFbOvUXM5MFXI5bvOYMqbETHG5VbhFuDnOTVFuLOIG4fqA6wKuDbgm4GrhKuFK4YouXC5MTtSYybVcJkzKcaktLhEuFjzhIuFCYeIALgg4P0qdcJ5wrjBhfJGZEDC+iHHpUjMuwznCWHvy2BrGlFBb4JjaDpydYvTwdma0cFaEM4VRIx0zShjpcIYwwq6MEIYPc8zwdgzrHDPDHE6PMVQ4zedUn1OEIYUVZkhATZ7qEWSFk4WTBifNSSkGDyo2g5MMGhgzg7KtxQyMMUA4UejfL2X6B/Tr65h+Kfr2iZi+Dn0inFDG8TEyvSMmI/SO0KsqYnrFqIpQWdHWVDpUtOW4DOU9XVPu0bNH0vR06ZGkezfXdK+mm0tXN2K6FuNGOFY4Rji6mC62zy5JjvI4MqDMtlDm0TlGJ/uCnYSOAUfUUGqLUqGDR3v7Uu2FtN2ULqVESAnthKQNJIWE7TVRg5Oj2CMuxKJpExOiNh1NExGKHNoKbWysjXB4isM8wnYxbP+AEuwsQqGtCysocAgJBS0F3owFBeX/hRH6ty/wj6Pz3yZgwL4KZW5kc3RyZWFtCmVuZG9iagoxMSAwIG9iago8PC9EZXNjZW50IC0yNDAvQ2FwSGVpZ2h0IDY5OS9TdGVtViA4MC9UeXBlL0ZvbnREZXNjcmlwdG9yL0ZvbnRGaWxlMiAxMCAwIFIvRmxhZ3MgMzIvRm9udEJCb3hbLTEwMjAgLTQ2MiAxNzkzIDEyMzJdL0ZvbnROYW1lL0xZT1NYRStEZWphVnVTYW5zL0l0YWxpY0FuZ2xlIDAvQXNjZW50IDc1OT4+CmVuZG9iagoxMiAwIG9iago8PC9EVyAxMDAwL1N1YnR5cGUvQ0lERm9udFR5cGUyL0NJRFN5c3RlbUluZm88PC9TdXBwbGVtZW50IDAvUmVnaXN0cnkoQWRvYmUpL09yZGVyaW5nKElkZW50aXR5KT4+L1R5cGUvRm9udC9CYXNlRm9udC9MWU9TWEUrRGVqYVZ1U2Fucy9Gb250RGVzY3JpcHRvciAxMSAwIFIvVyBbM1szMTddOFs5NTBdMTFbMzkwIDM5MF0xNFs4MzcgMzE3IDM2MCAzMTcgMzM2IDYzNiA2MzYgNjM2IDYzNiA2MzYgNjM2IDYzNiA2MzYgNjM2IDYzNiAzMzZdMzNbODM3XTM2WzY4NCA2ODYgNjk4IDc3MCA2MzEgNTc1IDc3NCA3NTEgMjk0XTQ2WzY1NSA1NTcgODYyIDc0OCA3ODcgNjAzXTUzWzY5NCA2MzQgNjEwIDczMSA2ODQgOTg4IDY4NV02MVs2ODVdNjZbNTAwXTY4WzYxMiA2MzQgNTQ5IDYzNCA2MTUgMzUyIDYzNCA2MzMgMjc3XTc4WzU3OSAyNzcgOTc0IDYzMyA2MTEgNjM0XTg1WzQxMSA1MjAgMzkyIDYzMyA1OTEgODE3IDU5MSA1OTEgNTI0XTE2MVs2MjldMTY2WzYxMl0xOTBbNjMzXV0vQ0lEVG9HSURNYXAvSWRlbnRpdHk+PgplbmRvYmoKMTMgMCBvYmoKPDwvRmlsdGVyL0ZsYXRlRGVjb2RlL0xlbmd0aCA1OTc+PnN0cmVhbQp4nF2VS4vbQBCE7/oVOibkYKkfMzaYviQE9pAH2U3IVY/RYohlIXsP++8jdyUdiMAfqOQRXVXQ2r1/+PAwn2717ut6GR7LrZ5O87iW6+VlHUrdl+fTXLVUj6fh9ufOOZy7pdpthx9fr7dyfpinS3U81rtv28PrbX2t3zw9/XzXvK12X9axrKf5eVOEvv/YlMeXZflVzmW+1U1lVo9l2l71qVs+d+dS7/zgP/HpdSk1+X2LCYbLWK5LN5S1m59LdWy2y44ft8uqMo//Pc6EU/307+9sQWrMpb0FSSH1FqQ9pMGCdIBULEg9pMmCNLjUNhakEVJrQSqQyII0QfIhQcaorViQW0hqQSZIyYLMkLIFWSC5YZBhuz1YkBOkzoKcIXksICOc1mMBGeG0owW5c4lg2MmwTW4FFBgitaDAELkVUGCI3AooMER7CwoM0cGCAkPkVkCBIeotKDBEgwUFhqhYUNA2TRYUtM2NBQVtc2tBgW0mCwraZragom1WCyqS4GRBRRKcLahIgvcWVCTBBwsqkuDOgookGKU6FUkwGnQqehSyoGJ6EQsm9ChqwYTpJVkwYXrJFkyYXvYWTJheDhZMmF7QoDNheuktmDC9DBZM6FGKBRN6lMmCCT1qY8GEHtUbBBN6VLJgQhLKFszoUdWCGUlosmBGEpotmJGE7i2YkYSiQWdGEtpZMCMJRYPOjCTUMwAzklCU6syotnN34AhDnQ8JFszVe3jgNPjm/bti70v4/n2InT68rOu27v0j4kv9vs5Pc4nvzHJZ7qfq7Vf9Bm+GikgKZW5kc3RyZWFtCmVuZG9iagoxIDAgb2JqCjw8L1N1YnR5cGUvVHlwZTAvVHlwZS9Gb250L0Jhc2VGb250L0xZT1NYRStEZWphVnVTYW5zL0VuY29kaW5nL0lkZW50aXR5LUgvRGVzY2VuZGFudEZvbnRzWzEyIDAgUl0vVG9Vbmljb2RlIDEzIDAgUj4+CmVuZG9iagoxNCAwIG9iago8PC9MZW5ndGgxIDE3NzUyL0ZpbHRlci9GbGF0ZURlY29kZS9MZW5ndGggNzI4NT4+c3RyZWFtCnic7Xt5fFRF1vapuvd2dzbSCUnIRrqbJi3QhEBYQiCSzgoa2bckA5JAkEBgAMOmsjSyBxCGUQaQYRMHBJGbELBZHKKoKAo4Ijgug4gw4sKA/hRHkdzvqdvdMYl+o9/7ve8/7y9989SpOnVO1alTp5abpIkRUQC5SSLzuFkzrOunvT0LnM1Ehs4PTJswZfZdz3yL/JtEijph8kMPPLjg1nSi4LlEcmzZ+JLSU2m31hKZN0CnRxkY4VPC9qD8Fspty6bMmHNqR4UL5W+IIrZNnjquhCLee4Ao8XGUd04pmTMt4EzwH4l69YS8ddqD46d9sW/6ZZQLiALvKEcoBohVdlGM7KBoIu1T4JqgdRO1a6JeUP45tD0+EO2mfWwi7aPj9BK7Ca39dJhq6DVqRTkY11x6nJaRgYrAWUFD8CjgP85itBpKpu3ww3Y6DdmRNJ+OUBSL1j6jBbREOgetJRRCbSiTBtFUWs3u02bSKPpIXkSpdB/9nqYxt1agPaat03bS03RYek27Q0EUS+PwnNb+pfxd+5CSoPEEbaSP2LqAg+RCL25I/pkepE3SaJlpE7QfYIGNZsMGmfrTaVbLnWh9PH3KotlcKRutPKWp2suQiqfRVEab6AjrzvpymzJK66+dpij0MQetbqRqOoTHQy/Q+yxYuant1G5SDHWkezCeGjrDaqW6OwvrMuAxBV5qT2momUp/pZP0FrOzF/lUJVhJUVzKw9o7FEFdaDis3QXNf7Lv+Hw8C6RX5Twti1rAL38Q3qZX6GMWy5LZQDaCt+dT+RbpQTKhxy54Smki/L0BrV9kTnaIB/Oz0lPyXvm2oXXdJa0FZsRBT9Kf6UUWgpFaWQV7lF1gn/BsPoY/yS9Lj8vPyG8bSzDq+2kKraa99B0LZz3ZYPY7VsbmsmXsD2wjO83eYtd4Jh/Gy/kNqUyaLr0gZ+EZKlfIi5SlykrDtbqCupfr/lb3nZaiLaXBiIeFsP4J2oKRHaaz9B6ej+gyU1gQa4HHymxsOHsEz3y2mu1gu9kzrAa9vMUus8/Y1+xbdpsTHgOP4zbeBo+dP8hn88f5Zn4Wz1v8S/691EpqIzml7lK6VChNhVXLpLV4Dkofy7HyWVmDn1OU9cpWZbeyV3lJuWkINj5qItObPz51p8Odi3VUt7xufV11XY32MUViDmPhBQulw/oSPJMw3+sRcfvpHAuG72JZB9aH3QfPjGGT2HQ2B55czDaxp3Xbn2PH4KV32Q3YHMLjdZs78e48iw/Ecz8fz6fztXwdr+EX+A+SUQqSQqVIqYPUVxotjZdmSA9J6yVVelP6h3RZuiX9iEeTA2WL3EZ2yE65rzxGnilvkT+VP1VGKW8oVw2BhimGpQaP4StjD2Mf4yDjYONo4xrjIeM7pmJE5wk6SM9Tgw+7JC2UcqWD9BjvKsfwM/wM4nkMlUr9OSKV72bL+TxWw9sqcwy9eW82gG7KDvj6Vb6V3+K9pf4snw2lSbyLtzVDhIzdiNLlE3RdPoaxnUHLcwzBbD6/YQimakY8DX2+InWWndIb9L70ETPK2+kDOZC1Ytf5LmkQouAFuY9SQDZpMz0nTWfz6CDPxe5027QKcTyA7cG+MIylsH9LGkl8AKIoVfqEFlE5/ztdxzpeTn9ipfIEeoy6srn0Kf0Fq6K98ntDB0Mke51PlCt5S1ZDXH4Go0tjbZmkRNBiNlraZLjB36OZdFYOpIvSs7D+LH9O6i/fVIawMqyAebSUpmsL6SGlQH6bTSCJjaBE+RJ2t7lSimwDXYBdZRT2tENY3UewD2RK/cGJRuTch7gYjh1iE54N2CdkRNBErPGR2MXOUI1hGPfQBKUFw66Dff6NuiFUpP2FNmoT6PfaOkrCfrBMm4sWd9NVWkO72ZK6R2gaJWDlXGT3KXn8rJKnJfFK/h4fytc3nl94O5FF0+d4nqM86qMcpUr5XRpKGdoq7Tyiux122I00lu6lKxjlv9BDP6mWutYN4FVanjQN4/2IBmu7NAsLpDJtMg2kY/S0UaESo9OVmenK6HN3eu9eaT1Tu3frmtKlc3KnpI7ODu3b3eVIbGtvY7NaElrHx8XGRLeKioxoGR5mDm0REhwUGGAyGhRZ4ow65trziq2qo1iVHfZ+/ZJE2V4CRkkDRrFqBSuvsYxqLdbFrI0lXZB8oImkyyvpqpdkZms6pSd1tObarerpHLvVw4oGFyC/OsdeaFWv6/n+en6tng9B3maDgjU3uizHqrJia66aN6usMrc4B81VBQVm27PHByZ1pKrAIGSDkFNb2adVsVZ9mJ7hrXJ7VXEyhcAoNdaek6vG2HOEBaqUmFtSqg4aXJCbE2ezFSZ1VFn2OPtYlexZaqhTF6FsvRvVkK0a9W6sE8VoaKW1qmNt5SqPmcYWO4NL7aUlowpUqaRQ9BHmRL85aquHr0T/VETj4dkFyxrWxkmVudETraJYWbnMqm4bXNCw1ibSwkK0AV2emFdcmYeuV8GJ+UOt6I0vKSxQ2RJ0aRUjEaPyjm+8PVdwiidZ1QB7lr2sclIxpia2UqUhD9mqY2Ndh7VLFJtrrRxWYLepGXH2wpKc+KoIqhzy0IEYlzWmcU1SxypzmNexVS1CfZngkIaZ8fV1ek4XF7n8IfWeZcIi+z0ICNU6zgpLCuwYU0+RjO9JleN6QgyfQgYttRQzMlENyC6uNPcSfKGvKolmu7XyW0IE2K9/2ZhT4uMYEs3fksiKOKkPNdT786rTqXboIELEmI05hY199HL3pI6zPNxun2a2gsB9NAi+LSnslQz322xigld6XDQWBdU9uMBbttLYuGpyJTsLVV4samr9NZHDRY3bX1OvXmxHJNeQuIhGqiZH/U+oOaplblkvlUX9h+rx3vr8ofb8wUUF1tzKYp9v84c1Knnre9bX+XJqy+wCKY77cjxO0msRlKPqhUWhIFiVE/Fj0IO61GM0ISp1DrPmqebift60MNBm+41KHu2m0NLJT2o+M9Vezsbl3o3KjcwLrpRgMA7B/GFFlZWBjeoQat4O7/ERRDwNK7BZs1UajpWZiB+PVttToDBOdcFl2UIA8edl+YqNBON8+UJ8RHQmdczDRldZmWe35lUWV5Z4NPdYu9VsrzzMX+IvVU7LLfYHjkc7sjJOzVtVCF+VsV5JxJl++VQIt1kjZdVwdsVg9PCNrpakyFckCjTKVxjFmAzKFS4dw6EegCteJ4p2mm+l30kfYP4mvf+ddMpA3vwjki6dbWG2sEQkDEfaj1ap9keXQrfJKteSiB/tU56mnENfQw+TpF2sjkjjHu2iyxqR9ieJcWmrtF/i0ixiEZCGaehfukb8GvOwZw7iHDzwMDpON39z3XwdfWakL1M6OUfPM7/cpTMb7XRGsq6MPbO2riBG+fIH0QJukcRvK7UUSBUuq+QKCetWLi/ga/hGk/yszALIoHApQGHBnJ0KJHjUFW6zd+tMzArd2GDFFRLaTRHsFoKtMCuu4lyJCTrC0tkS+GCA+cro6U64AqnXDxmt0lhYmjCHRjtt9jCDwdi9R4/Urvx2Tea5YX+6nDxDfqTPXMtzfU+NEfalY0xG2JdAn7p69FZ6G44qxw1HjSdNr8cb7wkuDB7Wojy4tMXD4Q+3XBF+LPxq7NW4m7HBx4Oeb8njzPHm1uYEs+GveKUwYt80gQZoN12xCYFmk8FwKj42Ij4+1hQfC7+aYuOlkASzh+88MDCMhXlY9MGQhAiFEjz8qCuU8eDAilbnYI8Lw2RH+UKykpn1dAWHHczA1X8qX8BlfoS3JQtbU7VSTP1ozMAtp5gIfeozrt8ZfSUsXIwdybIWnZwtMCkowBPUEx8mEhrNRj+YGGlzpMIjPXp07+awtzEY7+rRo2sKrgLwFH5k44+pvFXiU5tu7N74yKOb2eGW//7buVv9dr20Y1TCvn2Z6eNq57989YHyP26ubHn2vc/3Few5tnN5SRd4coT2TzkKnnTSOVc7JSQqJDdkaYicGzYybFacNCRqsnlSRGnUzJCHIpaGVEasiHs6JFCxSh7tkisoKDikhWxk9pBgJhzkQmNHmXgZC2Hda4KDI+XoI3wnxfAyV9vIhHhFTmgfEl4xxjrVyq1uY4VD+Kyzg5HD7OCOtUnRHtazOuYcO8LwPo3ICUK1FW+ZnNZ29LB1Pvc5rwsHImqufzMaLrwOB8J/acnXzbojvX5EFMFzCCQ2vWVqVFTXFK/LjKn1Wb/3hPuMIiV7G8eIGssT5Qv275jX9b6I8KAKz9JJE1dF1Ng+f27OqfIHSh9dW3ftwosaWxS9cZn66NztEVv4nHnjHl282Hrw5ITq0jGbOyW88Fht3bf/JH29Ev/bl48svbJxTGj6t6Y4k3573PHJXR0EPXh39Ws/7L8zwdzLdJ/+Gwyma+h6xj51AyjbTD/sr+tq7uXj13+UdgYfS9z9fVD5u3S/XEGRwD3G1jRbGUEFbBkV8T00V0BqTS75WXoQsntQzgQ9InQhPxz4CEgHRgCxPl5/oAQYKsqQPSx00cY00Y5OK6jIZKGpygjtDvpbr5ykB4AtyO+QP6HdhjSagvJO6B2XiVKFDHTWG/bQBvA3o34ceFtAC1Dejvwo6HX25QOMqylGUMAAfnu0s9I33rukF6mHXKF9jLEUos17gaXoYxBoHpAPmZagWcAydpKWs5PaDtSD0iL0v0zwgRwf7Yd2lqA+A3ptUV6EfCzsMICGAjagHX+W0ngEHQNNxvhHescNnKQyMeb6McF+n00/h9fG/IZAny8Adp6mXQUNaGBbUyxqgnukruQGLQfigMH8NE2R7yMGf21UrpIkgMgTfroI3C2X0gCUGewcqtTQJlEG+uuo0O7Im2mb9A31RN3DhvUYRyn8jbdRfouS+ZeUZEikBYivHLS/ENiCNq/p8VBKw9B/J9Cu8lU9hpYCq9DXDb+fhG9QXoh5HYK+fhQrAvpDgb6YFzcwWdiD/pOFz8W8sxF1aZC9AplRAuC30oGxi5gUOkIfbSX64nDHT5R2QGY1/HoJVAYihQ1+6HHmA+peRTsxgAFoDXQCrgI7gHKgF/A80A59E/qV9HhFzIjY1OMDsaGchA9hmx6z3jFs0efTu2a2+9oS/dgMz1K5DzbRplgvImZhS5W/bbGmRMz4qR7f5SLu2VdinCKm6inWnvwF9RU26GsQseWnYt3BZrEe1vPhtBx0E+J4kYhZYZ+fCr+IWNN9gjXho+kNxtpZXyOgEpHdF+uL/NTvi3paRjvRZrFhLPaUbdRPnoH34T/QWPkm5UjtqZPSGTyMB7Iq/4KGmPCujLkciPLGJnSDgPE8m4STaou8F/48T3+GT6fL53kb+TxTlL3aZwqx15W9fL6e/xltClbrrRNUoGHd/yv/vwJ+QdmLPXOv9rlyXtMwnnViTRi/YJ0Bq5+CXw24gQ4mJ9tgKmce43AyG4i+AabKLuqluCgV18QMORL7PNYC+MOVj+m4tJpWyOe195ib3Pw8LTVGUglfjz0NffELtEhAtA86rUEcNYq5prHkp/54bUrFnu+LKQuoAevvjA9XfLgFfIs4eop5+0gV+7N+PmCPBpZ641X7oT4+X6enQVf647NJnJY3ic/gpnHZlOpnC/Z3/zqFHSv84xf7o9jjxB4p9jmxz/jlm9IG+pV8D+JY7MOnqci3rtv4cC9svOxb+9iHMd8jNc2Qp+0y1Gi7pXBttyEF+b8DirYL455Tf6YWaHW+87S9/yz18inIf44qXWmKbz/bqe83X9Pj+jk6QrcvwLCfFii3Me/YA3V7t/nWIPwJu8vlYvh8E63COGKkZViP4AOjhE/0uSCKFueCOBOlJ+BncRatpkXSB7gvCN2uFKafFxk0Era/rvNwpgoqeMpI2mH4glLk4dhra6lUzJUYh7BHzL1pJoWYIrFPnKcu8jOQiaRAyG3TfeCiXXpcCN1y3H7gC+M4MiJmB0BGtLdd13FRuM8fO3Vf6Pq4i4j4Er5Am4ZIGqLfJ76grcpwGok1tN3opu2G4VhzkbQbbTwNveHCFujF6uf1E/Q7rK/l2JuWY88hPf6LtNvSXoxnDvZ1QHLDR3spWnHDh+X62HNk7x67TKwfaQ85RIwYnsA+LO4TT1Cl7KRcQzmtBm813h/bod+V4C3G+u2MtbsC+hbfvk3oewX4QjdD3GXEHUGsF6OLWhrc+j2AdBvEPQX9S5/RduleWo44zjQ9AT8soSScFwyxlwB08UIvz/dhlRc6z+ylzCaZaZ7O70pv8z1SEOJWnKGH5YU0UR5BKVIXipHDKEn+G9bq9/SkFEpj5FP0pOyhVaIst6R2Et6dpRrcLQX/LA0SfP42yhuoSE6H/nL6vTyGKqQqxN47FCg/gLmGnvIY4qQt9L9Guz6wT6hIGoG1tRT577VnhZzeR402UkDuR0m6XgPotvrRxGaeD7/dizmFvSLfyF7YWm+n38ZfsE8fp2gXekJGflK8l2ofAoleWjeYr6a9wDb+PmVL/ekhthsbzGbKY1eBzT7so346rQIG44zvzuYCneTu9DywEPmOoH8F9nvLuLt1pw+AJWj7RdAD4r1AgGdRD0HB2wJsAN7w1zWE6OuX+A2hxFHj8kFyC7BvtDsCTeXh5x7or4d8N/wJIBbXChgWUJFxFubvLvAT0GaTMvpJkQ/SpF+z59fAzlJn3YdeuBqO0T8foFG/AR82oFZBfWfD/5d9/xVgfhcAo3X//osifTHUgl2gNqAjQEdIM2mOAMpJKBf6/cm+QawJ7KY/6vz6+fPyESuEe9zdTflNy03n9dfK/AA93RD+OKiPh3W0WEDOgDzQtGx6nRYLGF5B3Ss/L8u7fgVF1EHapNtEeow1KRsG4swEeFvYGqvrrBKoL5/FWgaErK4fQqsF9LUL8BqaKFBf3x37N9DArz2EX9GnXu+fH/+8NJ0f2OeSzwBFOCvOUGfQoaCZflof3779olHMD/bGe31Z7CVXm8j8tCZ+WhtnxVnzy23+bwLWzingJPDq/3RfYpcRe4RZ7BMf4h6SgXvkedxPfkeLiO5gL/kxGfgL9qFhoO+Ch9O7rj0QgnwYeBNA/0x0+1vkHwT/vBcal+Nom+9eGQPeIZ+uydfeUK/+7deIfkBE/bDfq397DzAJ+a+Aecj/A/RF0A2Q/xx6i0Ff8tbfGYPyLOAYyl+gPBkoQH4taCRoR6AlEA799QLiPvKz99D/dvrL7x+/leLOMg52WsTvvEDnNn2H+M3UP5+/Qpu+a/jn/9dog98ZNKFeP+Cd6TLufWrDd5//9I7jp5jPuoaQh2t3cKcMFvdocZcV92f9/uij+vubfo9Fv0QRfiruzuL+Ku7O4v4Kuh10uUHR7Rku3vOFXb5fVE7+b8KHXrC52FVfFf+31YxmNKMZzWhGM5rRjGY0oxnNaEYzmtGMZjSjGf8RTPwnJZIMGkcKcTJTMmWhJjjwDknEM+0UKrWiG4AGSGRBmgwMBMYAa4CtgEGXE5ypwALgOHBTr3FJrarXdXV5QFbq5MCkySl6scRbHDVaLx4YWeil/Qd7ac49XrFeXrEu3bzsTlleeldHLw1PTHELGhiSUpsZJUXRWwCnaUgZf5lCGSMLbZMiSQW4ZPBxXFL4gbaOlK3HJZmYxCVGpWTRaiVWHRKWkhnINX6DwsnC/8Wve2v49QMtwlK2Zt7LL9N+4Dgg8ct4PuYf0wJ+Cd4MRZoBbAWOA2eBG4CBX8LzEZ6L/CKk/kHJQAYwBtgKHAduAEb+D6Rm/qGYGz0V+QyA8w+RmvkHGNYHSEP5+8i9z9+HaeeqU9NSDusZZ7IvY0n0ZVrF+TLhUSke/nb19+0tHv7JAavTsi2zM3+HVICjs3fQ+DtkBQYBxcA0wIDcBeQukBtYC2wDVMAAnQvQuQCdU8CbwAXqDLiAQYCJv1WNbjz8bLUjy5IZxc/wk9QKTj3NX9Ppm/xVnb7BX9Hp66AJoKf4q9UJFsoMEr/rho4Z1AyajHqFv3igbbhFywzjx+EeC9JkIAMYCIwB1gAGfpy3qS61hKORo3TKRJCsps90+hfaYSLXJIvLkY0Ys4rE0etu5JBstW51cJdj/UYUReJ4bB1yInEsXoWcSBwPL0ROJI7Js5ATiaN0EnIicRSNQU4kjoHDkEPi4Vueb3uXJXVgObNmhvLZ8NJseGk2vDSbZD5bPPS9LGx7srpDB3hsk8vZvoPFfYS5jzH3EObewdzjmXs+cy9k7nTmvp+5ncwdz9wJzO1i7qOsJ1zhZq6aRsU0VzRzn2LufcxdwdwO5k5k7rbMbWWpLg+3Vd/TVSe5OjmQKdYV6N19UkJhow0etSGsbVj2x5GeBTS95IKQtY1XOCZB0DYHOmR4y516pUzN7MdPQPEEpuEEfQTImKATCKMTaOQEGghFmgGMAWqBG4AGGCDdBoav0dNQpMlABjAGWADcAAy6OTcATlN9Ju7XDUv2GT1QlPgJPOKbvDZuc7U2x5ud5n7SmngWmsAGJmgJPJWioogoPMwU5mEhh74L+fd3IRSQGcAf42uoNSZirY+uqf6+tcXDNlQ7jloyI9mfKEFG1LE0crBE0J5UoZe7U7xJ0G4Uz/eCplTHj4BaaLWjo+UIayG0Dlm+j79i+Szew5G9Fn/U8q7VI7Nqy3lw9h6yvBO/wvJ6sscEzjGHh4Ecseqih+N7Wvad0kUXomJTtWW+IIcs8+L7Wsrj9Yrx3or7K1ByhVqGOIos/dBeTvxYi6sCbR6yZMTfb0n3SnUXOocsnWGC05vtAGPbx+ud2hP0BoeneliZq6NxvbHAONDYw5hi7Gi0GS3G1sY4Y4Qp3GQ2tTAFmwJNJpPBJJu4iUwR4ssQTvHP+xEGsyDi73aMZD1v5iLl3v/t58zE6V5SW0r5PH9oFstXa8dR/liremuo3cMCBxepij2LqeH5lD8sS+3pzPcYtSFqqjNfNQ76XUEVY48Vgqvy5R5Gwwo8TBOsJXHia4iHibGwJavjBG23ZHVhIUVHzcqIzgjvE5aWl/MLSbEvdf70iW6Ub62uzx9aoO5pXaimiIzWujBf/aP4nuJh9jW7mZtzmH0lSGHBYakP+zp3iOBLfXIKC/M9bIQuR1b2FeQQMV/pcqYEsgo5spoSvHKbvHKJ0IdcW0EgFxBAibpcYkCALiczIVdV0TY3p6ptW12mlZUqdJmKVtaGMqcSIZOYqMtEuemULnMqyi1k1D66SHw8RBLidREWS/G6SDyL1UVG/CSS7BNZUS+yQu9JYj/JxHtlQi75ZUIuQcb5Wz/js5xOdqB34bhR4juexfbc8UCxunJWWbTqHmu1Vo0r9H3501E8dlyZoCXj1UL7+Bx1nD3HWtV71C9UjxLVve05VTQqd1hB1SjX+Jzq3q7eufaSnMIDfQd1S23U14r6vroN+oXGBonGuom++qb+QnWqqO4r+koVfaWKvvq6+up9kR7jgwqqTJRVmD3KSw/woEDEa3GcrTAryjytjx68vW3R8+OOyOKfa4KchWqwPUsNAURVUmZSpqjCmhJVLcQXeX1V0fN72+KOsN2+KjPYYfYscs6YWTGTonMn5nh/KvABa8ZM4XBv6qz4v31Ql6u6SnIqZhDlqx2G5qsZg4sKqoxGcIvFkNRefl5QUK5Hq/UyO4HZSzAlqV5Q8NIFLyDAJ/jz+Z/po9liFbj50QPMlcBmUEWhpCbkD+PYCob5vjF5BNclcTxUFGKAFczJKvxt6GaTN09ivH7MmOnL+fwww0e9WlCp8Luj/gMdbFX/B3m0BIoKZW5kc3RyZWFtCmVuZG9iagoxNSAwIG9iago8PC9EZXNjZW50IC0yMTAvQ2FwSGVpZ2h0IDY5OS9TdGVtViA4MC9UeXBlL0ZvbnREZXNjcmlwdG9yL0ZvbnRGaWxlMiAxNCAwIFIvRmxhZ3MgMzIvRm9udEJCb3hbLTY2NCAtMzI0IDIwMjggMTAzN10vRm9udE5hbWUvUkxZVFhPK0FyaWFsTVQvSXRhbGljQW5nbGUgMC9Bc2NlbnQgNzI4Pj4KZW5kb2JqCjE2IDAgb2JqCjw8L0RXIDEwMDAvU3VidHlwZS9DSURGb250VHlwZTIvQ0lEU3lzdGVtSW5mbzw8L1N1cHBsZW1lbnQgMC9SZWdpc3RyeShBZG9iZSkvT3JkZXJpbmcoSWRlbnRpdHkpPj4vVHlwZS9Gb250L0Jhc2VGb250L1JMWVRYTytBcmlhbE1UL0ZvbnREZXNjcmlwdG9yIDE1IDAgUi9XIFszWzI3N10xOFsyNzddMjBbNTU2IDU1NiA1NTZdXS9DSURUb0dJRE1hcC9JZGVudGl0eT4+CmVuZG9iagoxNyAwIG9iago8PC9GaWx0ZXIvRmxhdGVEZWNvZGUvTGVuZ3RoIDI0MT4+c3RyZWFtCnicXVA9b8UgDNz5FR5bdSAh73WKvLSqlKEfatKqax6YCKkhiJAh/75AWp5US5zkM2f7zB+6x86aAPzNL7KnANpY5WldNi8JLjQZy2oBysjwm2WU8+gYj+J+XwPNndULa1vg77G4Br/DzTB83VW3jL96Rd7YKTIn8fEZmX5z7ptmsgEqhgiKdGz1PLqXcSbgWXglh90RiJzXxwZyUbS6UZIf7USsrWJg+xQDGVn1r3w+RBd9/d1gQVFhomqBBYU+qBMWbOqDOmPBRhzUPRZsmjz/b1JaJV2pOJOb99F0PmW2lkwZS+XabnFJBfGxHxBpe1QKZW5kc3RyZWFtCmVuZG9iagoyIDAgb2JqCjw8L1N1YnR5cGUvVHlwZTAvVHlwZS9Gb250L0Jhc2VGb250L1JMWVRYTytBcmlhbE1UL0VuY29kaW5nL0lkZW50aXR5LUgvRGVzY2VuZGFudEZvbnRzWzE2IDAgUl0vVG9Vbmljb2RlIDE3IDAgUj4+CmVuZG9iagoxOCAwIG9iago8PC9MZW5ndGgxIDYwNTQ4L0ZpbHRlci9GbGF0ZURlY29kZS9MZW5ndGggMTc3MjQ+PnN0cmVhbQp4nO19B5wVRbb3qa6u7r530p2cmMQwDEgecpIrIlmCsggIMsAQJCNZQJKoqDxxFURACSIiIiKgEkYWBV0EFXiCLiq6KobVkXVdVBxm+n7/qu47cxnA8O1+773f+y7j/57K4dSpU6e6q1piROShecTJN2zalOyrdzeyELKaSOszYuLIcTdrY76DG6AtI8fOHKH1/3gbEUd81rxRw4cUecavfZgotxrim41CQPRzWSvg7wN/jVHjpsxISzOvgX8GUeHjYycMG6J97MkmujMF/g3jhsyYmDnOqEd0phjpsyfeNnzi7CHrv4T/QyLzKTaCNWYjqJj+RsTa0noq5Vmk4W8EQiXdwvpQCeKHIuV8fRHrAzpO30Aa4ufqb6FMjTWmoTQJrjx9AyumPfQ5cs9nS0RnMUCmJvlPlvWjOMC+Ey21ltRPH6e31bfr8/XtSDFVH6HPp234bakd11frs/Sj+izqJ1vGukvIdtBK1pXl0kptJevAUlkH7S16BW0ewdqxlay1OCKO0Ek6yXoh5RaarnnZn9n3rAHrx7Yj14/0I8uCr6nWlJ1lX6LFK+g47ye8tJIeYHHwFdNbaPfn9D1N1lEqPSBOanXESTpAn9B7CCcazTT8ZvB64iT+vqNNNBqc+YRp4qSRYOboI7TzVMIWahu18yyXafiLY1ng5i38Lb1Q/7O+GLHgDtN4Y57F2+N3oEwhTrKVaMUnxgg2E+nk3yzUU6Id0Hahj/voNPqF2rWB2ixtJZ1mW9ketJhoEduqF5pD9XRaaazU+9FZyRs6rr0FfvRS/LiP7jMa0Y+6Qd/x7qxQ3yQ5RnniFUYsx+xqxNFy1tVciJ4Qb06zKAGxbzASrzh/SGUZGbRcz+ePo+2aNifINzaT3tJa8qGQYfn3ENtFD9Eumkwogtd8yTSEzjVGdbN927S8LkXb/L37ZR/qn1OvbhVvts/M3ka9tkXNzN4VCPTqp6eL/ttEtW08z9qm5+V+cqXIT+rV7darX/YuVuu6Dm6x1xV2QOCN/eCUPgQj/LoOKk7Wuk3k4b8uhduyh43Kvtd3b26re33DW9WTkm4v10eIDZidJmUVk85qgg0Gq/kis8RiTacGB0+UNCLfiZITJQ3jY3Ni83Jic0boVDaZp5d9bi83o89/f5tRW8o4o3H2aa0lW0iCUv2R/GnaZHAdYhNv+MpKTryJUspQRk4sz40/zkb9dLKILbSP2vexqTLvBFasfaZ9jHbEvaQ9Q5t1RrrvxEFkOqcy5UzQppTfr31sn3bm09DAZ6IB5DCCkinXH+/ZEsO3JK6OWZFCSZHJRlJcQgpqK5NNP3OuxHe2IfPVzK1uxPqSGhc0Yz7KyaZY9cu33jp79ujRs2eNZvPt/fb79il7P/OzfFaT+bUSlvL55/ZX9udffcVS7CX2OPYQm8ymsIfscbLN0CNCxyzxUi1/It+qa1vFEpO2eqwUI41TimAR6EHJQdmKBiUF5xQLc2KF4mFsznesj/0Eu5mNZ30ulDAvf60zMzpfaGr/qHj5OPqHuUUZ1NZfXTczlqVtMX3LY5clbDG3R2nP0ZKoFZm8OrHkJG8W+TJ9H6Kag76zbn+/sH8467PPxLVUrEu8mjXOpsQEyqleMz82k4EFTZtIdpin+Mvl0+r2b8hiWUP7Bfv9uT/Puv2DIfevW3f/jcVjxUn78y8jo+y/n/vePtuogDXo2HHx1Gn31Kkn27eYSD+L9hl0nT9ZpGpc01M51/IEmsYxATgj0/fhm8kt0XeMIGTT9IlvJfpX325yxgb5I0yeJmryprwjF4PicxJZDstZrA8v32Mv1vLLG4mTpy7o+h5IxBzwIk6NdS41oE7+WimR+VvI2JJJ2+ptiVuduaJhSqInktdIi7kqLbGmJy09n6fF1Myp0dBXdgYyIMc/rmVsXEuHOWd8Z31nW7ZsyKobiQlJDi/y6rOmTWrkZOuJCYaZyRIT9JzsGk2bNIsPJgCztDfGTpkydsxtt9mz77mXpYFlMSztvntWrILIfGSftt9b9f2wgQOGDh0wcJi2etr48VOnjp8wdW7tzXNffv21fXM3177q5aUfffbZR0tfZn/oX1jYv//gQinH0K1aD71Qzb9q/mhtE+3QNxmCYerFW76yNiUFUnjcOSD/Pme32o9I6IX2HHujPceZD17M2nyMhwmX7fdThiHMDMMQ3gzLKwzhkW4tQ+cMsDK4zr0ZHq+u8zyvTlstfYmheT2WKXQoLo/BIbjbszgbdFCNX5szJ0ogSmoMLTWGpvOfGtGKkP7VmX9eireBt693hHcuzWVzrbmeKd57vWu8f8LfUfx97PXFWdU8WZF51lWe7MguekfRyers6cf7633FTcYofiuU0UijMHIKzWK361PFLGuKZ7F+l7jLWux5VF8ullkrPS9auz1H6DX2mnbEfNV6y3OK3mXvaqfMk9b7ngaDaBDL4TlM/XG9Y/nGwfYcrTY7otW255RvYo++yXz2d+JkaR0tT7tB8o5j9SOxGLyzKJayqZc/L452x+wzdqct8exOMcjkcZmRMZ6UdN3kSZmRSYk+MymV50C/FEi1GJssZQv/tXRG6lxJy4Z+D1X3VW9QvVd1nQ1iSoLqsNj4oIMpEavNYh2J43E333LLzSc/nTJ1ytRPtc6z77E/tN8tn6+1Z81Z8gj+UK8e1/e2D5ZPHjpsyBB7ppZa49UlfzkhThYfHfeo0hUjMD8GYn6kUmt/WqTPQ0k8ypeatJX7tnpW8xVp8fUiyaiT5is7WBBUiPZB32tOqxvubJA+OF1jg/KiWa6jFQuSkmPrs9zqWmJCHMS/uRg4+os59n12d7aTTZ3zxegxxya/XVLy9uRjY25o3oKtY8Nhh6xr0dw+0qWDff6rL+3zHboomQRfjZaKr8lU359I+z1L2P4kS0vykqjnq09JHu5o6diWLYPca7i9VyqUA4t15x0Di5KT4hITNNMAx7S295b8fP7b8h/Ychhj10+/dcSIW2fY2/A3Wt9eNunrjz/6iuUOmTLcPv/U0/ZPw6cMCfKnFPzJoG7+vNS0pCCL0nZXq2BStcz01EaRjalBfD2jTiZade5MmVx9DqrlA38uuyTHtg/OQhPzDD3IL/1ifsXmxuaI0qX24ScV04rZgmUsduacn2Z/8fN3p9uMrP2N1m9Cx46KcbeyxyXjOnW0A3//1rZjfKy6NLSYkskfwbsIutofr+239um0xGtAAIWHJRGPdKRPKoc259qAbf7EGB6jx4gYI8aMsXpFFUZNjFoT5WWDgnpD/hWz+VoLrHNzyw/Zc8XJ8j9rLTEPZpbf7azfqFNrizo51X2JXtFkPbqvrNu2mD7dtvn63NxvN1L5W/RXy1lD9qJP+EUvwVUNxbJUOavccoxJal2c74+3hMY5veKBTtMNS5YZodp+MFaplpKCZEyXvkkiyfBFtuGtze68m3kzjNNB5gQ+UuoCY5RZGDmXzzDnmhMjF+l3GZvN5HytQGtttde6WX20/qKfNdgq1EaIcdZEbQZUxlzrXrHEesaKH6S6z3I8UAZO7+uwP5U34ql2ZvlWxYGPtZzytmVnte7lOyt4oH+CtgtK9kdo+2mJzpI4cZgwB2W/zwQVsSxsw4UPxMkLPWCSqHymlPVIetvfmDczLVNrxjRLEq55vB7WzOv15HlNjZMFdkQIjwUjUXiNRrq3EUEYyxxV4vDkIFyVa6ZVoWWxdsaotXOER4uxYjxZWqKZZWV5Er11tHZaZ62n1t3s7r1J62/2947SJpgTvMu0pdZSz9PaNnObN01nOqfoJJbKfdFXsTzeijXlPZmfd7L6Wv09vaJHsZF8uDXaUxi9yLrX84iVAm0aL7mHHsOql73+GtOuL/ub/bC96Zy9yX5InCz7hGeV1tE7lH3A8y4Uh8quh2b7M8xmcjfQzDCNPNn5VyxhMFNrpJvotdfpdUu31y3dPuvfSsi+mowG+Zt4DYpINVqwTqyr0Zf1N3pFjGSjjMKIPexFIzpVSzOv1hqbXdB5v/kHbYA5QrvVjFBDz+RIqWZv1bLYOPuG8k9Ui0kntJjK3L1ZUP97KZ4a+ZMit5oRW2mJJz7KZJavnh5hQWgTnAkX1FTKmNtOiUxWI5W4npMrq3K1VrE2l2WwRjBvP7PtuWz+yYm33z4R4vb1N+Xlpfo+e/C4oqKxSt6wbovRat1u7I82HIFrwZOohbB8J7pt82LqRaupJ9TUU7bkuZKChmy731M5ub2i0I6159o+2GynL/TQtzuyDL13AGXHouzk2AgLNoXYH73CQ0virCRvSzkX4yqsZNinUuhe9MdPjF8Tz1XZjvWDChyDGTI/c/G9MzHVX7X32HvtV8HK+bvXrNnN55bNtw/Yh1kz7KJZhS1i0EJ/Ps/QYVVkYKMoCWkGdhcZSJAnhQGWiZwFOmzFEzsfIGy+XZMDwnB5+Wf+uqT5tGxtm6ZjeHgyS+EperLIsrKtTtSJdead9etEV+Mm1o8/YMUGBZjleNlCdj+7jy0sf89uimm7Xe8htZUc/36Bz/TXsO/0Uh495r/KY1BqVgT9Z/JRY030sdjsN7OOVFuTezh2RSTlJvOUKE9URNssHpXQuiaYdxCDURDrCMWZc2XS9j7749mWzkLh794gv21225x2+ddnX58zKHtQzvjs8Tl3ZN+RMzH//uz7cx7Lfizn2exnc17OfjknsSCzYda1mf6sGzN7ZQ3LLMxalDkv66HMpVnrM9dmbc/cluWDSFfYrG1ZXmxOU6zY1WtKw7Wxa8/HSktf19ZPnHRz7+H3Siux8875W0/BUq3+zl3/Mfn1P0z+agprwKLY+e5dO1z/4Ljad5fP3zhi0JH1r+2q9oee9euz2GoZf1c82QLZucVIwPpTjVr40411kcdiaF3iipjD6U+kHEvl7eP8KZGeqDRfhpwYEB6lHNXe42zDnT0zCzOlSRG0ndFojqYVyOUSTc5PhMxymjxz5uTJs2bN6rpz6lHmtX88OnVnV3slG/HlprVrNz29Zs3T2smhg+yX7HL8vTRo6HojwdHRcryaYrxSqbk/jd5kJ/ToN6NOeNfF6uuSMUxpZvsoSmh9sb1z7qzvBzRscPpcaeswtV67vGweG2L56E27PNRz+VNPLe/ziL/PszfZx+3N0HcN+j2jt7U/LGj43GOPPVfQyP4gKwu2WSL+mmc5MjQQ/IpGA30Ov5LX0bHo2HXimLUi+jB7gifoFKX509pHtJb8kjIjhfzMuTMlvjOV/FL6So2qbE3jgiQeysCNbJS9ouv2qUftH5n36JQd6yX/bps5kxdr/X4uWT9sIOvCOP66DCp7Q3JQIijfwqvLJxzpdK0/hxL/wjxvWifEmkj2XsqauMORK6qlJ2pWYhR10KJiWldTLTwYsmGS3DsrLcWMdhmymYk5ahMZwrhsEo4ECm/Z3qjV90/6ds5c6KNj9nOsG0wai7W1l04vHLXApzUecccd13awSxo2Yk1ZMotjrexXHxoxZ+p4Z2zzYZAvAR/jqbe/mk+wSGudwdbQE9HGDq8Wb5LpEVFR18VEJPg+7LYtqkI7Rkjt2KakrM3Bg44hfqagDHZbQZzc6PnFPHOepaHdaGEGc3RmbiwmTbPGfMnr3duwAvtte+X27W++ayR807xDjwCVreWFjHq89JwaW7ujiNZnYmRrwYKsWS2GU+KbSSdS18RlYFp4DkftyF0X9z4d4zUjKSran5jd3mhdO6gbZFvOOCONTbncJmC4ryq8yrW4q1PTJnKkk5sqLVu5Qech21O+EcP+ln2ORb41dXtXiMEzdvGtB4fdsvPmbRtKJsyeMXni7Nn7hg5k15ZeYNcMHLaxLNb+3v4sO4clN2u6cgM3NixfuWbDsuUbwN8tWG/iwN9kaupPidKJeT+IO5Z42PdENNOiqFNsVFSMTxrlzoxuAzNYrXkNdxamzkt1RLRpbJOa+c78UZyUEztJxNkronyJnetPnCencO8Xx7/6hra5vO8E9uhD49Ny8599tPyUkVC+aeigs45+wY9sh9z31sbKdxr73ic0wdAk30X7Xr+nl6fQM9Ezz6NXrndb2AhZi71SL7yw1kiwP1SyI/s2E2V66X5/grI7d9ATQcMzinwXG55npOFZmMpT9VSRarQ2u/Au5gA+yOhnDlam51w+TZ9mzDLv4Yv0u8V95hq+TCw3Vpm7eVqSliRaWR20TqKr1VcbZI3UCrXhYro2UZsmZlt3a/eI+6w/ao+IVVbixSYo2s1Ws7Xlp7Uedg+7m73SSCh7nq2CglvP3rHrOX1w+ZL5Ej2hyWbDBndMbrBCFIqJYp5wWaHYYCT8XOLMnc2wQXdinufRrf7a6YlxHt2kbMNMifkg+1guP5y5oxomUEJcpBVldE6IiuuclR6V4avpWPiYQxlyDpW1kQaB87SkQZs2Z861OVOC9Q1/yXImxWTlN8zvlT8xf17+0vzn8s1BTI1+ohKD4CKUE+vorFj32RO06p4Oeye+cthewVjHHiMmaPYK/w0jJ8I7qv0zI6ds5xtHjTv7WXlfrXNUtbTpYzatKX9f67xnzNOPlZ/SCzcMLpxIFeMbh/5Vld0dl5fdM78uu4m/IrurHgzKLtrhiK6rT/PRDvnssZ4/3lgXR+siD8etSPG0j+nO2ye2rvLs8cXm8e1SO0mbKvSZEw9qTvxqr0yfM2f61Nmzp0JMroNp9bH9kb2bdeKznlm37hkJRvYhuwR/h1gLloC/Fk5btth9xS1oi1x3WvszKtedw9Er2Ed8RwbWHL9afUJWat+ZM1WXnrwKdrhrdHxIU7U4yZeQZXoDlu3JWH7Wl+80vBtCFmneXK7bauVR48VL0LZYrNNJsdEewyS+P+Lh6MOeHabXiCLLFyeFL14KnxXY36L/QTXrz8itd6wyoFjVoUrmJQ0GNbh3mWzPdTvmxF1VizdISnz+yfIyvXDX+OFcSDkZDftgKOrNpw/9/qhILTqiWWZWpjBMyyN0b7OsrMw8b0Rmlp6obIeENxNPpKyJ1dfkwXaolemNyEo36cb0G6ITzF7Vr68l9fiJkjNScbdsGbQmfpDWRFxwjxb9LSaHS7BrsSLkDu0WjwfbvoiIyIgoT4zITYtMi0qLTompa9X31PfWj6gfWT+qdnZLq7Wntbd1RKvIVlHdPF29XSO6RnaOmh45PWqPtcezx7snYk/knqi8aCPajLaiPdHeqIjmUe1qD67tkc+5KoyYLKYnyS1I6OPdBkw+02wmJ1/y5HcHjxjWbUg7Fr/PPm+XTvh2zphPptw6usu4dn/ff65s2Puwbb5r2LBx0zr1Izy5a5/ZsTM3l/maNGnVsmGDKCtz/ZPbt2RKvqZjPDeIx7E2j/OnRQsrhq+LZTusdeS1IjyaB0Lmi4vukxDyyKDbtlj5E6fW6Gi1Rh+sXKMPlpxrI5WLVCwp7ahdvHxNxmN8MbG9tF68V2KhVsidjkqln5DUGg7Yu3LpjtUas0n2A1cP3GW/deL57dvF4/arAbLzejQP0PMn2AeM2NVKZ6zFXDX0QvVsLB0LN4v8IOFY8gof2xFnaBQfExXbCbrDl+ZYZY7aw16oQnOkz5P2YjzkL0EDp5Md9lbYaTXXslFadGxSJ+gOqYx7vzDu1SNsp7Zl4s32t/Xvnp6eW3PLo1rtC2vXK+3BsMUhkYr2GPRO1b0Rv2hv9PFFe6M1v21vNFu+afSp/VFDza/11UZo87Sl2lrslpy//fg7hr+/qr/v8JcqCKsM92I2xLNqPE2vSTVYHV5bb0ZNWEveUm9odaSODKujXmjNMO5m9/C7xT3GclrOHuWP6svESmMTf5Ht5jUq91pZWOaSWRIbaXeyp+uFZaXcuLDW0eGpsKXi0P8Y1sx/bUwGxQg9IjKKR2eABVXZEYNUYEdMXrRX8wnyrrHe57TDFxMd4bEkbyBxvuAmOU7KWULlQyrFKmdXKzdjl+WYBCaupVi3oZJ1fq2XNlybot0F5j2s2LczhH0nXPal6MzDhcAwmcJKYoki0Ug0a4gaRg2zKTXFJr6Z0cxsGd0y5jq6jnXlXbEtvc4YqQ037tLuEncZ90TdE/2IthwmxaNRj0Zv0jbzzfrT0U/HvMCK+S59m2eb908Ru6N2Rx/SjkQdiX4j5l3tc61lBYujWR3WFJLYjqWC1/Ug7iPs2p1eXnV04s03Jnv1wnJLO3+h2d5l37TqlqX4PpBI7wi+e2ixP83K0LjGM0zLzMPs3cHXCYuTzsjwQtSyjBgDovZmQWzFM9mL3t4wf4f+Wl/zVm2EOVObZt5pPmRamLWWj4F7HNaK8EXU5LWtBhEtrXYRXa3BEf9hPW49z1+29vOj1jH+sfUZL7FSVVcSpTHelOVM5cfLt2s9ypK0HuVH9MLS8pUBKtVGoE3QOcbn4i2stNnUhLrTUH+LelfVyU872zDlbM439EXTbyO/KKjzzTX5V9XlNRrWS0nXM1Pr1IjLyWyUOrJx5ogaw+L6tR5u9Gs8rNP1vhMlJXJdxrYg1nmUm9wy1p1RZ+2zZWfflft29WLIjGYVk725MmxgNPDcREe15sPgUe+JslguwuswaCRWUPmYOrd6jfyaWtMmcc2b1dBp5rGb5L++x2fOelu5+h3dnpvbo+f1dbZtvbWwdqeMCZ+PqdkqI/Ika7SCmePGjR07bpz984oV9s+Om5miMXIdvX3m0Zv69v0DXDNvP3pTv772qaNNmzQpuHf6zL4TY5N6tTp9ssc19mregTUfjwJKV66wL4wbNx5uJlasZAbcFAg4z2bMMXGY5USxZrIm4thUyt5pxEZzs44/cWn0mtiJ0XNj/dE9Y7OjG8T6orNivYMaSRkKnIIutcR31Ihu87dOqZZI9flVxk+1rKzYn2Ia1d/KU6ttTVzNV+TEFFxVqzrPy6mdHWsVxHgi62TVjjMis2vnJfnMFIos8J04WHCwoEwtA85/EDU5IGrOHiw4c67soHxDcbbgdJuzBe5Dd+f1RH5u88ZqXWsOR7PKVxWGmWPmOIMGhzNuwhp8dKJdaj/a7VS/oQz/9vSbfz0bzoyJRwf33jVs7o56WnpfO16TUc/2t08WPHfHsBf6yFca4ocD0VnVMrJjDvzINPl8vkfPWdMO+GrUiMqKPXD77T17Ktur7DVBgdbiR/fdHQzSfxiaBe3G4mDanChzXpy3kQ/rGifm5gFlr33zDbvvm2/Ej/jn6EOU0//ROdZVHQfHtPmBsiz1SPL4nPJzQfrTbWVbY97yjERay82hfs1xNnSjL+en234uiHnLDa/4l5Kvv0UjVDOxK9DewMq9kWXpdeiAsZPuEw/SWkun9kYpzdIm0wG+ibYBG/QGVBvxp7iXxvEbaALocQ2bC6QfCnwJrAcWAwOBx4G5rn8OMJo3ps+B+bKMIPQNtAQNv9toRF4jlYrFxzTC2AA63YHxIPzbqVgrlQgsMRojHOnMHxGHcAP9EKcdatRG3AF6SExFWXMRhjKtd6itUYfyxZFACfTEQNkX2WbQ+1D/UR08AG4RI6if2ENb9H2KDhTjqB+Hjajc22mLtk8iUCxucNxWX9osw8VcJ59Mx79H/gPo5zuUjri1ojllmUXUWdSmLLhT9U2yLEZaCdMllf0P8h782ar4lExdQVNlGrQrGnjNIpauLwQ/69Djiv/gvQpDHLBdhc3HmMynAdj2jBOfoaxkmi/HB34D4bOQfyryv2J1piIXoyTvFd8vA2srxhVjERyHIDAOSc5YEAeuQd05wXG4BDvRx7eonhqLEKix+BL0FfBN8v0ysIZSPzUW4y4GxuCkOxafg+Yq/gfHoQokX0B7qLEIBcZCjRmo7KusryqVfVf1X4EqGcWYy/4rGZH8kW38FSrlWeW7EgUvxfbAt+Zh8OoG2ggeZ6OfitegNUDrgsaoMZB8cKk4h3yzpT+wRMqpmieQVYVUN41DH5SUv+v49SmguYEN2vnAB07dtKUqNU/TrYbksQyT803ytgr19KUR1ivwYw7KeeDSB4N+OS/l3LgixZxV86YKVfKCMfutVM53NeekjMlxdue9mntVqDu/44w5gSlK90AmQHuDNlGyHxxrjLFpIU00LVVjPc8ZT+MIjVL6bXpgCZ8VuE/pqn4krIG0hc9GvzMwl9xx0D4lr14c+FrqDWN7YEmQl0Y5jQX/BltP0wizO+q6JjBFtcPRZU3BmyxZlz46sF/x5SnKDPLHeI72opyVKKe5sQDtGRIoMVqhz27/jPr0MNBHZFN3+KdK/VzhXwY9s8eRH3Edyh9AXrgPR06i4ojuVOwdSgOteOjZ9xy58myhYs9EKrYmom3uHEF6A/KkV8jCbxwjNQ+qzDepb+Scv2Q+KP4FfrhE7tA39Km/lPXQNgfzeXuCH92dNULxumo90EtSN1wy76vMV8ynZ1HHz+hrAznvLmmHI9/TK+S+al+ryvddtFj/kIa78/wrOa+Mb9DumdD916He4NhVac+V5l2QBuWd/x3lAXoKpUveWDsxjjtleYEz4uPAXn1f4HuRGigXUwN3yXapuq6h3vrX1BeyH4l2N1R1V/bf0Sef0jCjD9LWpkj+feBdp77AT2jjWjUnnDVQrZ9KTxYjbV9nHZUwNZoJXTNeH0jjjUU0XrxP41W5fVXegUIgXU1qLBIBR08rfaMPwly6izZLqs9A2P1q/d1q7FVr8HoXWItRVj/EP+WsBabk5WQaZQzG2tcDeQHRGGV9r7BZP4iwg1L3YWwAtW7fECjGPP6b/h7i3PkmYaJuyNt6MRD1BNd0pVvoTrEEbZ8BZFN/YKqcV6FQ4+NDPeivuB1tulu2394gPkAdvVAu+h9M62lHAz0vAW1poPkWdF9N1D2B0q1mlG98gbRtkWcPzOobqL4YHehq9Ap05U/SeAn2SuCEdhd46oJ3oWoqbV/yaaNpLWy7tbAH3gGkXWBrZ+mswmrINQA7IcIBbXdxtwTsvw8cO4ONk3ZSpZ9ukWHadhqk4JaHsDQgm/ehCdpamoB02+CfDvoZaF/QDcAr2tvK7jrDu1E2ewXtjaQO/HpKcNqiyq+KnZKK9tBVqizaQFSGfWv5cNBFwGrgAKnX9mV7EN4NFNZVeQToJ8BrTrryNaCfAtlOOpX2BPBXB4FuIeXCDC9HPXZTYCXcNyPsa+AM3F6Hlj0ObAypLxEYChhAX7c+2a6RbjsXVdZ7UZuBC7DTy1oT/Xw9UemroLDRy3c5acr7uWX8BPdHbh7ZzjGg6522yz6Wvwj6OmiWm9YHuiEEfRBWw9kHlE90+x/ruAOSV5OAxS4mOihPd92jxDLwfxHmXj3o1m2wJyBbEkqfrYJ8Entc6QDoLn04bGjY+/wedrMcO2MINZU2qXEwcNSKC3ygLwicNLMD75vvBd4w8wMHeCY1qNgHpDr2u9JDbzl2kZxLcr2Sa4KMC+4BRDS9odZS6T7t2qrQt1JHqXDY/8abNFmuk8jfUemuuTRM6iOpY1Dv42IkrZFhSo9Nxpo7l/orfbUH89q1L5FurXgObh+1VTY20ql4qYf7UN+g/jNaY56nUx1ZptEeOqI2NTEG0CLjnCoj362rn4pHmFrjmsKW6IL6z9NV5vuBo5JK3YX4+uKfNKFCzwftUPSR/xN2xOM0W3Sip8wBdJvQqZ61D/3dQTOMTc46aI5F2f+kq8RHdJNoQrcYPWFv3EJFhq7inwGfWuq7qLmsI9h+pZdlfbXoXpFPTypbXfIFdUueQ3cth7+DWA5IO0lSd39gmuC7u4+Ta5+7V7hGriOeNnSLx+ukMe519291qLWi7rgHx97MplmyPM8RygTP71ZpJGS+J+mW0P1fxbjLOqVdhDLNvzvjLvtvTKcnPZ/CPliFcu/E3qerW8/HtNBTBHdtWqjW2uUAdLVeH7p2Gk1W69aPlKlvpCIp2wrjgQ9pEtqxRepyNSZ3h6x9T5Al1wbzO5qk9n1nEXcH3WnNxZz5C8rlVMtsg7AYlX6x+We1BrWr2OO8SLVk/aosrEnOXody5ZiYZ2mAuRHp/0q1VDtWOXsYWb8adylLu9HWz6iWJXn5Emz378gHWWjs/Qi22/lK+93zGfxoA2zCCZDz3tajFGfNgS1caVd4xVLlV9TTkAqt/rCfVqCeL6lfxNU0xTMUYW69FXLZgppDjzWCrtgOvZHg4Of1vN9Pt/F+5y1zE9o1RdnZDfUzxNS47XH3Iui3uJFa6f0g+1KeBsDuxPjLMZAyIMdBzRX0XcqBSxuCRltZVGCsBm83ovxp4Md/gtq0xdsQ/cwFHx7D/D+NMQm2E3Kixip0nyD3g/JZAcbN+gJ7YEaWlB05fhdR6AOsyTHG7UjjUinnwbaqNnpR5ypqZkyiOko+MUYVfXfLsr6BPE5znidcyR6usP/kXiOEXsIX2MPSBgnq4Qp6JXsRsi/lT84Vt98XU7eNwXGRc0bJbXB8XD5V0FRaqp+mAZ6OtNTMowHWOXrDHEjrjLX0hriP1nn+Ts2s6lRH2uVWOtr1EtqRjvk1H/N1LMYB+yipb+XclvPL24Vuse6jSdZdqBd7VespWoh87VT7odeC+7ygHHhzkX4G8gXHO8jrBfS0OAm8Q81gg9VT7o/obvTxaeinp81WbtyN9LQ+Df7n6WnjerpDvECPQCd7xHtIu4tqiPVUH/bX00I+R8GKLDaDnoJ/DPU2vkP8Npqq4k+hPTL9/dCzKBPr5VR9NcrcjLqXYT6lwfb/Cw3QnqB3tWKaok0jppUTaQsC3/PnififqLe5gP4oqtMq1NlbPA1aHf6asNEXKfcqI9KNq0GrtNtplflX+NOU/48yTJf9qaHS3iHDtBmBA6JG4E5+BvsPmecs1k7UAZtzANq4ys33R3Omk19g/PhJlCv9DQJL9B9pAPjYDnuDP2qf0NtobxFaPJiI1QfSAOb6Yf8w2FYMthO7A/bE2w6kW7tVppHPrqQf8wVpDdhILFW6eSmtleEYiy36J1gnH4L+26me4+zR/kR7eBPHLSbQbu1mukdfg/h7gPcQ/keEH8a6JdOthX8i7RZ91HOkPeJaoCsli5Z0rThDe/TjmAOx0J/TKUH0gn8xysqne/gSyPZWoG+gTMKMo0We9rQI9sohGEo/wY45JJ+X6ck0B7r4L5izj+o/B+TcXWX+gearZ4KwrfXd0ImgEuIgPRaEnk5zFFYFnpGI8NICCe8BB1ZPWiqBdu2Q0IoDJZ5utMDMpzEof6nxD3oAuvJ+4wTdIeuQdct6JdC+D68AeWxZHv+YCd62AtrIcNhiR/RP2Z+ATP1TSnWxAlgAdAMyXbQDFkn5lPsG7N1ukv2SbUJZe7S+NDLY1yshlAdVwZfSnF9DkF9BiMkX+0N5WZWfko+Sh5eD4itgNaL53rpI30jxcmkQ0n85yHG4CBiPqjDnoW455hijUATHS0KN4aVjIHE18FzoGLjP15cAT1wGh1wslTKoF2JO9FfPm7OUXQLo+6FT5frThm7Ub4UfgK24RcyD7bsEa520N6Kgw1e7eeQet7ubZhPKi3LK01dgTuluOCD9EpAp7E9oHmRC3s7E/oaudfySsumgr7n7zneCbcJeu0S+HzB6wy4tA2y6QV9CtcV3sKP/CZ2aRL3ERoSvB0oD7xhLKFf8hbqJ49RVwiyEbfwY1uNvaYXC81j/kceoRUOwb75R7KSrET/K8kPHHaFbjetoqDkD7V9AHbG3Oggd01X/pOwquA9cjLJHgOYyDXAv9vw99Wx6xviUntFzAjtFY9gbMYFPjThainQ7kKYU2ASb54RMj7CrjLqwV+tSE6x7ftkucQJ2PWAcRnt7Q//E0UNmJ5rm/YoGSMBOKcSa1BPrWFfjWeqjl8AmroH+mFjje1ERdJpH/4F6GvuohhmDfUsA6/y71N3wU5LwwObphr3KT8CPbvi31B36sBVsEBl+nSD04QfE3UeDjHLs20sQXkZtEN5fvIlxf4Vq6AfhXkBdQOMhLx3EV9RIH09F+gKgFG18FnQisBAYhbatdeNugz29AvR+hQUG7OtgPmO5EyZWgu6lNsZx0NsRfqebdyxsXcSjfCf/OLjvdvLoN1CBKmeGCi/SJ7h0B/K/A/puZdtkHF9GRdojaFeV9xhmW9gPF2OLhJUHOyEO9lsV6mkEOy4TcKnMo9ywKYJU5se6W6y3oVl8BPkVasEdAvDJzw/QLJkuNNzzAtp0BvXswX5kiGP3XdTeZFp+OfxKe5dfRHMrqcyrr6JZ7ATmS5X3MMZdtLwKJktYk1H2UKAqRV+sCWhLKB2N9CGUn6ZZ0PvFCg2Rpjr2Ud9TH6A4BH1CoMKs1uD1m9RHPm8GLQ7SYPiV4iXVNfAbgN7tAxQH6e+p16XFVWifX4oP1is4tQCKQ9AiBCrMjAK/36UWxleg5YBLVXg5tQjSqvGS8jmoZxjkB9T8EvL3JfoXxGTkrYT09/Fgv+4phbw+CvoO/C6VcaITyvkZbe70G8s65ZTl7eCUEaRAseclahGkVeNV+ZA92M99hHyHUIk+IVBh5gXgGdRXDPo1EKTB8CvFg/J/oD9bAVBzGNK48CRVgXx/8dilNAKyHTHwylScx7xpinnaFGNRiS0hUGGWAZjQK2lo109wB2kw/ErxoPwHV2ckYO5ci7BrMS5HMQZHkcaF2idXok8QslxzC/WRZUh+Q4eMCoU5DjrAwRYJzxBHh8EOvlQfVOqF8S4cfeDObymD5nHw9zjKctAn1K9jDOS+U/YDMnhFYOxCy1E0cg/NCsI70EHQbxyCv4GS16pyWiHT7lh4XWwJ9YM3WXKuy3e2wBj+E/gtcT0lyPbIOnw5DqKgs6PGVvr1/rBTUgIl5tJAidcKlETOC5REn0eYjrDZbthMJ0xfgjCEe+YGSiJKETa1Mq+nBOkmVaaTMHoi/GMnv0A89sOTRJp6DpFlPOPs//WPsEbK5xXSZrsV7hnqne14aevxc7BtbpDvEQIfqOdRq5znUSp95wqky/ey7jvxm7FejxK5VEdCPf+IR57Paau5DPblA9jLu+831HvSq2iKfEcRtCVlXqOd8/yLf0EG7Gvi79E0vQFN45Mc6Lnk15vTNPZXicAu/iXCm9E06MBpMlyhM9LEU0/sd6fxT4CJZGBfNQ311+RP0ziFkzRObHfoRUh2ATd7BfQLpOsJ+iTwJdDTpV+66dPcuB1OOujrcXwVjeXjKYFPoxbQGzdyP+XIstR7kyerpJHUTaOe8cn2DwIPSsmrV8MYnHTrDNYr26ajrENu/ShPex3wuxTgk2mMtgruJ4Af0a5ebtvmAncgfrlTlt4XtBCo4/RD3wx6DihAm1a57bwJtCHoq8AGYCSNgw167cW48LlExTOmynfdF9FLzjb8Cv2tZx7Us+pZlH/xGYdLzhk0AJVnbXoEw92zDxroDaA5wXfpVal7rmEzaHt5RsL113Zo4HP5rFi+I6xKr3TeoYL+2jvX4LNLl1Y5+7C5Cu3wq2cgfuUsxO8+EyHHW+oSlwafmf0arfpsr+IZ6RXOUah3KPI9afC96Ajn7BSfFfhAUrMO2jMX+48rnLX5d9HfI4+Xo5CzuyE3Y9wzNZt/bfyvSN0zHb9Kq45X8DzHr9Cqz6yrUnMNyqtJcep91i+g4qxXH9Kt/mSas4ibO0lHPZbxMZnq/ddlYPyBTONmsqw3ke81Mq0GxK0xpAff2V8J5lLUsZosLyPdS2R6JhL3bEQZ41HWPDLl+zUHgUPAYrj9oOeAMuBH/hHSfI22NUcbO5OJMjn2qTr2ghZgXu4MmDoLUB31TifL8xrpnsNo71i0dxPaK9/D/QLMScgzE+18BG0sQp/l+5VfgHkd6nkGec6jfxz1rEI97yFvS/RvlWrfsOB7x+C7R+f9Y+CwegcZbLNbf7Dcf3Uc/9Vx+Xf1+5fabvKALd8PS7dzXoA97p4bkOcFNly23ROQR75L3hCw5ftkZXsSXQfMl3nAUwOoDf6+KN8tA5aUJ3WGrpSu0c8HbPkOGml7A4NUPVXlwD3XUuGXcwywagds+d7aeAGyp85COGciLscfaxHSZgfet54FzQ8ckO+hnfMUqn/q4G6QwiYg+Sk11ledq5XPXYnJ77i8SZf9p87hAkg7HmWMtxygPHV+lELOfDwkqWhP78gzFMBD7lmKpkBjkcHyJbTNtF7IMzVE67U3aNvla3X+yXZFLKL2MSlYd6tRLf4Q1RJeqhXqxtp4lHenx4FXzD/Tw0KnJeo5OvIbawP7JbT1gWXQIbUlD1lfe5R73vg+62rqaKyjJRJ6OhWJZNqHNCsVkJ43ppMyP9xj9cnUFm0uUmXuZC3EDPrEmE+1jJ20Cn5NnTv4GfE7aaJ0S7A//1LvLsPr+dRG2ZzzYTfOpyFAD6APcD1wjd6SFgeh9aAJwEh1Pgf55Bnc4Bnd35XftYWVbYn9imtTjpd2rzw349q+41W4PEMDO9GcQNcLaWs9SG2AR+W5YnVG6kGqEVkD+78nYP/I9boN9UTY1eLBwCk3bUpEdcjGg1QN6OiW4TX+Ch30IOQF8cBIGQb4YVsKoG0lLpQDV0u39QPJW2i1pU3p2UbbYQMstPYiLB/j/DUtFsvhf562W8uoi9mDosw0egtzuh2QqP+ZuoqHabTxPnXnrwfOmEcoTs5tz1q6Tp57Rtx4g5x3/+YC8hsL6UbjVnrDrEvdxVbaaNViwtsOeohYvuGlZMMDO2UNdIs8JymRFvhBe4G0inMkY6mPIZ9dvqvOX2eJd+lhYxp1U+cPZmJsdlFrYwD6/T5smn+ijTNpAeSnI/TmAO8hyGdv8OrzwHOiDcr7EthFqSi7iT4Va3AqdEAiMdjMV0GPdISdcS1si0xtn/2BUUp99CE0MXgmO+J0xdnscSF0ANDC9Q9x6QDXLZ8VFwXPcKI9xdZh99z7EfJGJJE3agjcP6lzFvnWj5QfcQ1supBz9tIWVu8NPoTdWgqd+rH7/H87ZXmOUVbEWbj3I6y2olmejyhLpXfPyUu58vakMbIsSUPPSaN9bTDfMOfY/aBTXSr99wHJF0PNTaShNMDrplvo5lvixg+8tLxgmSpvKJUoQ/wAYHEIPe3GJQH1gX+4/ueBP1bm1T6rrEeiwi/jC0PqGOymGRwSVnRxW2R/VXvvC+l/NNwvOFDuYPoBl/atKv9UuubwNwPt7NArQcbT7Q6Uf6rb/svxK+huXlFHIzXXh+oDqHXFnYz3qVA8hPUJwJxbJoH5eCrUjXl0yOhOyyXEPufeiDqP/yDkVd0ZYTfA/73QWGOpi7HmdHfRRchzPZuBnarMxyTg/hZr2ibo/qHAF5Iac1nTUOifUKY5njK9AylTn0cZ5jHq4Z1HDeBWfgnUf7uENoBmShp6F6UK7lL3Koie+4U0V8JfLhP2HnAS9tQh4LX/izKr4n2FPQ6sQnpYQnfae7n6q+JYFfxa+iO/CaFjUrWMW1zspL2/AY+FwuxFz4VCv8lB1fCqcOv+W9W2wFa4XcKdG/1R1jzsw/6zAsG0+2CnOBgmITSl+4+DbnbLuQQq3x2YR3eoubTPLWuzAzY7tB0RQ+hhiX+DPFTpH+8ubbggPNfSw5ebp0F3lfiHXXpKP05+4Dbo+jsrdZID/hXLCNpqQWrM0I4ZM9DvIJV3vHqSgTX2WTWf9iPdfrorSPVP2CeYt/U8LWi1REQvl95PM+BmRhktV+cu5fMVdy+ENTZNpkFcLuR93sXQBl0aVhlukDYZfdvk0FA3bZJtQRubmw/QHlmvkU8GdEQvsScwUPX/dZrxW6AfD5Q40FL04+wQ+NfGwZX8kgbdEsH8oeX8nviqqJr+fxqq8kOGsRmuf4aDqv39PeG/BTLvRe6nQhDk8ajKdGrcRoW0t4Ia+YGSfw08/tIwMenKcReHS/n9LRBjHQT9+kgHUu5DgY2kwpX8vzedwgXsw845FLjNpb8IvbnCHmM32nugEjwV+/wQXLY+OZexv70cH0LTWOdo4iXxVdsSWu4GxAPiQwcyDHrzGejcUaBFwGZgIbBIQl8Gfx0VttlMpzkSYjD2Z2k0x/MT3e9l9CDidgEvSejtaaVbzgpgi4s1so4Q/3b9Y3oI9HmXznHDZT1FYgBwHvu/Aqw/19FmfaBbP/JJKp5T7mfcsN+CMdZNtDkIJ0w7Lan+N3oOfFCAf71Zl90I7If7PKgOlMA9yO2fDP8SYZmg49w2XAc87cZtQ9w1oHJv9yncfwBeBHoDDS8T3t0JZ9cifDdoP9AzoO1BX6z001/469jTpEsesRnwF8P/goY9EP+YnhVlWGuy6U6Xh6t/BUE+u2CNsE4tvxx+O39lO1VbRwOvwx2l91FjOtMZW1Yb9FVQyBoTDuhbF0XicYyLh56zXsK6PwLj0FLaQSwKa9tR0HmgHocqlAMjEdbHkPuu/dL2Yc87Y8j6g26TMN6kGfD/B9AB6fqGQqY1nP1UX5d2CYmfAUjbYQdoHeBFoKlL5d3KexHXGPRbUA4qy5J7MuzdMNcugtwzsEjgajdsr9tuWc+NrvsmFw3d8IaXQYHTJlrhluN38wbLC0LGPeViKbAOGO8iWO86ty+rgQWuf4gLVQ7GZARwexXAFuQC+8ptgKG9Tls1aTtsp63ADKeP7HGgh1Mfk7y6A1gL94MOtAwHbDfwAZALtAT+AExH3EFgLNzyLva632q/OPLxb8VUdzxD6ZVwJgRuGCupkqaOA5bogOY6YG3cMXjSTRccu6B7MrAcWO9iKmzWccBouRbxL2CTfqHs2Hfl9w7EQXoX2BAy1nFAfU97mhoB2xYI0iu5JZ1q+LF/8LO6Vwa/8393/P/v+O/m/393/P/nqHi2xmIcqGeNzxsmIwW5Xx/s4jLPE5SdXPncolUQUV0rn2v9OgIHq4TJvJnqGx3/5mcPIXjfxf9t/L8Cuc7sD6HNjYpnpuo56GXiK56PSlwv8Ut7BWXry7BzVENBPjNwUF3uIxB2vYRIJa/8/oNIDZwWpylSfdthBLVXZyY2umdNgmdZgvf/P6Wh6o6jfD8q7963oizPQWprTVZnLHoE7+HK+6Xqbrs89zWD1sp74OpslvwODsoS11OBGEXZoivdKCzKBO1tXUN9xJ+oFmgz0YB6ib7UBu5eYii1EmOol9WVrhaTqI2ZTFcj/FoxndqI4VTX6oR0Haih1RxpR9EApG8j8wIDRCfUM5gaWL1U+ACxOGCLjjTAGqbiBojWVE8MpAbof1srF2nvoUnmPbCLALTzVheTUW7FO+GK582jYTv/DXxNQp/L4AcN5tUuIE0J1ZXvh8yegVdFIfyfA5NoufpuxnFajjYtNFrSJnWux/mGTbH0q7xv0U2hbVHfGrrg3G2uaJ+898phL8jzMO43cVQb3fLUuY+HXboH4yG/qyOfdVV5NibDf8ce638l1Fkz9wyrOkcm72lPpQj17RT5Pq5x4FW9rfvtoY+VbAysuFscvO8ty4B8y3kE1K44P79d3Q1vgvx7Qr/7JO8mVpGp5UoG5N1h98yrfFcnz4ZqDyPuYchnEeSnSLkbAct02I0SwW+yqO+73EWbg/dgPR9TkdWCanmKIEt/pputferM8hZrK80yh9Nk6zW6xexOk7yJCC+tPFtmdUcb/kH9Ivw0wjpF/cxt1Mp8AW3tTlbwjmrwzukVvovwm8Ab0zQJrTv2uS74ElrMs2ixfgNNlgiee7P8qP9DSg/eyVRnTg/QaO8R8lqjqZ+3I+hC6ufZAzoBfVhPXrMwhHZ2qLwXLr8BINqB7wug995EOX2hq6bRjbqfZpj9KMdYSN5g3yET8oyl11xOHc251DF411N86YRX0FRqoe7MBs/PyO+KJdFm+R0t+b0yxa/7sS+Xd7/zkO7BwNdiT+BryNbX4gbQ7aCAUTvwNf8e7gOBr3XATApM0b+iaWIhNZf3tSEn8mxfH/WOFPLiXUl+tof2su9oqFadmmnNKVdrT2nSf0k46G8KR/6q4Qh7Tf+CiiRESyoym6t7LgqiC/RyLbhfcvye6xGmATotMGtgrGQejjzDnTAhzwjHgZ/Jbnh7J71+HuEm4sdU+BcIr5NHf5AK9J/hjoRbtuMM8D38g5EftozVAPvnV1DXgitgYhUsr4Sx4lLon10e6iyd/EbTWaoD5FslACjGN9+qRaMj0ujhiDhaG2EAoFHYG8u7oURsqrzTKXpTD3MhbTV6YF4NxDrdBeV9qM7k7DH+iLAs9R70lLwPGgp5BzWIqndR+R3Un39C/eU9VD6L+l90D/Uw0gbvnwbvnl7m3qm8pyrLlflUmucwZ+R9yRk0n7NACe8QKPl3+9W9x7tpvmgbKBGvXuqvvJcp3b/fr+62rnHvuF6Oyruape6dTdDgfUr9KeQFfq9f3bNs7N63BA32U969NL20VNyPdnVGuhXQ/ftoKT+KfGOAnwNbhO7cx7wclXczrZRKvlWUWyX8950cutw/+c0Y+U9+W4VIK6ZW8s6vogfpVscfEnYxjXNpV0mDd5LRNnUvmTPnbrLsj7yfDP+q4L3TYPvV/QHm3FkOlRN1L/V9WvRr8vQvy0cVeVD3d3tCh32EumoESqr61b3er+Hfi7H49FK/uj/9IMZ+MfxHLvW796qniuloy52X+qvOB3U/uBl0XtAv7wVPpqUV8vcPegD69oEKfsi72R3pfv0c3IMq5bMqX4NyWVXeqsqX+CGwwIgPLBA/0LVGPHTID7CX4mG3u/RyEmV9Bb28C23uQ4fk/UjY34f0zQ449iViBh0yWynb55CYhfCP6JB3AR0yvkJ4kROH8g9h3TwkasF9A9IUgL6IsgYiXbRznsM4Bn8C4s46QNlFsl5ZrqQq3UcV7z7C+H9hRyeSz6jr3GkSs2mlhLSh+VZawjMCS4y+CG9DxdZNdFDZUXI/+AjsuseRpxbstk2wj2+DnXsWsrZeneW62T3TdbM8C69HYa/2tjrbL+8ayW/APSb+Q32rZAnkTJ5dHu9++/RmaaPp9Zxvn+rR1BxxRfpGyjTbYK96J9Y8+e3To8437X7pG696Gt357/jG63/Vt1z/Hd+qUn37he9VqXNW/wXfpVLnu+T3nuQ3qOT3pgbTLPfMRX33+wNrfuX7vuN/63eAvX+D3vlfAGPR/w7Anv+vg59O/ZfWVxX96FHPDOoGvdjW4698h+3pT4ND32m7eOAyYf9tuEwbc4PuyJOXpG+F9IWSyr5eDrA9x7nfDBznfhtwO3C3i20Inw66FrBoOXZVSysR9F+0xwi1n0Jsp2A8e/Hi9Jfak6G24y+79ZrKht4GPXpU3sfU9tnrxAw2vwqahLiHAO2r0GtDIP1jgR4uVXcnZR/V86jJzrdnQm2+UHtN2rDqXDRsvOC3XN1vt6mz3uoe4z7arL4bkabehz9Lzvd5Lgf1/R53nSqRUN91KZQU6A/93l9S566waK6+xVrifFtF0ovd+n4aq++X9OJw+T0Ys42kiFPfhZE06C7/XLqdb704953l92LEPEnR5yWUxZdICj7I74PVlxR5o9C2KEmxlq2W35SRtErbQtosvzNjdpe0Sl2bsFZtkvTiMkPzOt+fkbRK3iu4Q9OHuuX3QX/N3rL2aV2D3xST9oDaw1RFqbunCcFFe5oruC/a14TuaS7ev1TuVUL38VdwX7R3CXF769AC6xGUvdzZU6v9DPbFoXubUHfVPfjl3KFz4oru0D36Fdzq/0GwgZbgL/iv+7+Ae4BdlZDfvmIrLobWwgV0H5/n4tCVAWkiaCEyBgJnKmGiLCsS6OPA4wM6E3nhlp/UVZhXBZjjkYiP0n87olMA6IcYlB2Den3QTrHy/9TxHVHcDOBNB/EIjwdN2EKU2ATYT5Q00MUJopS6wF+JUicSpYUg/Suiamv/fcj47v8NMuuGEUYYYYQRRhhhhBFGGGGEEUYYYYQRRhhhhBFGGGGEEUYYYYQRRhhhhBFGGGGEEUYYYYQRRhj/k5HVJowwwggjjDDCCCOMMMIII4wwwggjjDDCCCOMMMIII4wwwggjjDDCCCOMMMIII4wwwggjjDDCCCOM//GYF0YYYYTxPwqMKKUW70F1aAZFkkY+8pNFJL7VckD1a+7U5rGaZBNneRSL3xosh1qRYDWoFL5cSsJvdTesukon3Zxlq/gs2ovfTCrCb4aKrUap+E2nTPymqZBU9ZuifpPVb5L6TWQJFI1SE5VPujmLV+449RvDomkO4mOUT7o5i2KRdD/ColRYFO0nnUWyCOqPMBnD8TsPYRHMSzURJmM4fv0IkyGceVROS/2a4Ij8lTmM7Y/UF9fEM0P1S6hfXaXiqkeaCmHql/yBOTxwNbdtXnahriiz+YW6vNTmP5/vJH6ew8934j+V8h9t/oPNz9n8n3v59zb/h82/s/nfM/lZm39b4hXf2rzEy0v8+jdfe8U3BfxrL/9bKf/qwSTxlc2/LOVflPLP4fnc5mds/pnNP7X5Jzb/q80/tvlHpfz0hynidBH/MIV/sDZTfFDE3z+VJ94v5afy+F+O54m/lPL33k0Q7yXxd0/6xLsJ/KSPn3gnQpzI5u9E8P9Eiv8s5cdR/vE8fuzhSHEslx99O0EcrcnffitOvJ3A34rjbyL6zQx+JIEffmOvOGzzNw4NEm/s5W/M0w/5A3/OE4cG8UN+/c95/HWbv1bEDy71iYM2P1CNv2rzV2y+/0+txP5S/qdn08WfWvF9L6eJfQX85eJY8XIaL94bI4pj+d49kWJvDN8TyXejst0232XzlxL5i3H8BZvvtPkOm29P5s+n8m1J/DmU81wp3wqytZQ/i/TPpvMtIFvm8Gdsvrkmf9rmm2z+lM032vxJL99g8yfWR4snbL4+mq/36+vAqHWlfC2yrM3ka0DWlPLH0fnHq/HHbL561V6x2uarVg4Sq/byVfP0lQ/kiZWD+Eq//qjNV0A6Vtj8kfp8OTIuz/QH+DJkXZbNH47kDyHooW78jyB/tPmD4MODSXypjz+Qx//D5ktsfr/N77P5vTZfbPN77s4T99j87jx+l80X2fzOAr5wOV9g8/k2n5fK53r5HTafY/PZNp9Vym8v5TNtPn3aRjHd5tM28qlT0sXUUj4lnU8u5bfN4ZNsPnFCXTGhLh9fyseV8rGlfIzNR9v8VpuPGhYpRhXwkTYfUcCHF3nFcJsXeXmRXx821CuGRfKhXj6kMFEMWc4LWawoTOSDvfwWmw+y+UD4B9r85gHp4mabD4BvQDrvb/N+pfwmm/eF3x/oa/M/2LxPJr8xgd/QO1XcUMp7I6J3Ku/VM1X0KuU9e8SKnqm8Ryy/PpN375Yguifybl1jRbcE3rVLtOgay7tE886lvFPHBNEpkXdM4NeV8g7XRosOMfzaaN7+mjzRvpRfgzKvyeP+djHCb/N2V0eLdjH86mjetk2UaJvE20Tx1kW8lc1bJvAWNm8ez5s1TRPN8njTJgmiaRpvul9v4o0STRJ4k3l644JI0TiBN/brBZG8UcONopHNG6L8hht5g0heP57Xq9tK1CvldRPzRN1WvE4Rv6qI17Z5rUSenxwr8jN5zWyel8lr5IIBdWpk8txYXp2iRPVSnhPDc/x6dgLP8vLMTJ5RLVVk5PFqMfGiWiqvtgs640E9PYqnpXYTaXN4KipN7cZTbJ4cy5NQW1IpT0RYYh5PKOLxsTzO5rHwx9rcV8Rjon0iJp7H7NejfTx6nh6FmKhSHlnAI9C1iCQeMU/3RnGvX/fY3LK5aXNDeIVhc+Hlwq/rpZwXcQ25NBvaK0qwWE5RnO1iRYuWsDr/O/7Rf3cD/h/+y6D/A01w4fIKZW5kc3RyZWFtCmVuZG9iagoxOSAwIG9iago8PC9EZXNjZW50IC0yNDAvQ2FwSGVpZ2h0IDY5OS9TdGVtViA4MC9UeXBlL0ZvbnREZXNjcmlwdG9yL0ZvbnRGaWxlMiAxOCAwIFIvRmxhZ3MgMjYyMTc2L0ZvbnRCQm94Wy0xMDY5IC00MTUgMTk3NSAxMTc1XS9Gb250TmFtZS9UT0JUSVYrRGVqYVZ1U2Fucy1Cb2xkL0l0YWxpY0FuZ2xlIDAvQXNjZW50IDc1OT4+CmVuZG9iagoyMCAwIG9iago8PC9EVyAxMDAwL1N1YnR5cGUvQ0lERm9udFR5cGUyL0NJRFN5c3RlbUluZm88PC9TdXBwbGVtZW50IDAvUmVnaXN0cnkoQWRvYmUpL09yZGVyaW5nKElkZW50aXR5KT4+L1R5cGUvRm9udC9CYXNlRm9udC9UT0JUSVYrRGVqYVZ1U2Fucy1Cb2xkL0ZvbnREZXNjcmlwdG9yIDE5IDAgUi9XIFszWzM0OF0xNVszNzkgNDE1XTE5WzY5NSA2OTVdMjRbNjk1XTI2WzY5NSA2OTVdMjlbMzk5XTM2Wzc3MyA3NjIgNzMzIDgzMF00Mls4MjAgODM2IDM3Ml00Nls3NzQgNjM3IDk5NSA4MzZdNTFbNzMyXTU1WzY4MiA4MTIgNzczXTY4WzY3NCA3MTUgNTkyIDcxNSA2NzggNDM1IDcxNSA3MTEgMzQyXTc4WzY2NSAzNDIgMTA0MSA3MTEgNjg3IDcxNV04NVs0OTMgNTk1IDQ3OCA3MTEgNjUxXTkyWzY1MSA1ODJdMTM0Wzc3M10yOTQ3WzY5NV1dL0NJRFRvR0lETWFwL0lkZW50aXR5Pj4KZW5kb2JqCjIxIDAgb2JqCjw8L0ZpbHRlci9GbGF0ZURlY29kZS9MZW5ndGggNDg3Pj5zdHJlYW0KeJxdlM2q2zAQRvd+Ci1burAjjSQHwmxaCln0h+a2dGvLcjA0jnGcRd6+yny3c6GGHPDnjEY62FN/PH46ztNm6u/rNZ3yZsZpHtZ8u97XlE2fz9Nc7awZprS93gnTpVuquhSfHrctX47zeK0OB1P/KA9v2/ow715efn9o3lf1t3XI6zSfS0L256+SnO7L8idf8ryZpmI2Qx7LUl+65Wt3yaaWwrfw5bFkY+V+hx2k65BvS5fy2s3nXB2acvHhc7m4yvPw32Pao6of3/7uWGkblmhkpU0S7RpW2gGRlIAOhTtipdshalnpPKKOlS4i6lnpWkQDK10nkZWFQcLy1rOSLKLASnKIIiuJEEl7kLAJK+1BwibK6ZW0R5RZST0imBISfLmGlQRfRYiSMiLIE3oodJGVHlt1LSs9FLo9K32QiIiVAXIIWoQBcghahAFyKLIyoCO1rAzoSHtWhteOkCcMUEg9KwMUUmJlgELKrAxQSJAnDFDoG1YGKPQiDwxQ6C0rw4gIPoURVr1nZYQJH1gZYcLDujDChId1YYQJD+vCCBNeTgdGnNHLiwtGvL6xYWWH3bfSHkzSsW+f+xbapkvyEf/7Wp/f83PU6HhI93Utk0PmkcyH52SY5qwja7kuzypTftVf0JgtKAplbmRzdHJlYW0KZW5kb2JqCjMgMCBvYmoKPDwvU3VidHlwZS9UeXBlMC9UeXBlL0ZvbnQvQmFzZUZvbnQvVE9CVElWK0RlamFWdVNhbnMtQm9sZC9FbmNvZGluZy9JZGVudGl0eS1IL0Rlc2NlbmRhbnRGb250c1syMCAwIFJdL1RvVW5pY29kZSAyMSAwIFI+PgplbmRvYmoKNCAwIG9iago8PC9TdWJ0eXBlL1R5cGUxL1R5cGUvRm9udC9CYXNlRm9udC9IZWx2ZXRpY2EvRW5jb2RpbmcvV2luQW5zaUVuY29kaW5nPj4KZW5kb2JqCjYgMCBvYmoKPDwvS2lkc1s3IDAgUiA5IDAgUl0vVHlwZS9QYWdlcy9Db3VudCAyL0lUWFQoNC4yLjApPj4KZW5kb2JqCjIyIDAgb2JqCjw8L1R5cGUvQ2F0YWxvZy9QYWdlcyA2IDAgUj4+CmVuZG9iagoyMyAwIG9iago8PC9Nb2REYXRlKEQ6MjAyMzEyMjIxMjA0NTkrMDEnMDAnKS9DcmVhdGlvbkRhdGUoRDoyMDIzMTIyMjEyMDQ1OSswMScwMCcpL1Byb2R1Y2VyKGlUZXh0IDQuMi4wIGJ5IDFUM1hUKT4+CmVuZG9iagp4cmVmCjAgMjQKMDAwMDAwMDAwMCA2NTUzNSBmIAowMDAwMDI4NjI4IDAwMDAwIG4gCjAwMDAwMzY4NDUgMDAwMDAgbiAKMDAwMDA1NTk4NCAwMDAwMCBuIAowMDAwMDU2MTIxIDAwMDAwIG4gCjAwMDAwMDAwMTUgMDAwMDAgbiAKMDAwMDA1NjIwOSAwMDAwMCBuIAowMDAwMDA0NTU0IDAwMDAwIG4gCjAwMDAwMDQ3MzggMDAwMDAgbiAKMDAwMDAwNjIxOCAwMDAwMCBuIAowMDAwMDA2NDAyIDAwMDAwIG4gCjAwMDAwMjcyMzkgMDAwMDAgbiAKMDAwMDAyNzQyNSAwMDAwMCBuIAowMDAwMDI3OTYzIDAwMDAwIG4gCjAwMDAwMjg3NjAgMDAwMDAgbiAKMDAwMDAzNjEyOCAwMDAwMCBuIAowMDAwMDM2MzEwIDAwMDAwIG4gCjAwMDAwMzY1MzYgMDAwMDAgbiAKMDAwMDAzNjk3NCAwMDAwMCBuIAowMDAwMDU0NzgyIDAwMDAwIG4gCjAwMDAwNTQ5NzcgMDAwMDAgbiAKMDAwMDA1NTQyOSAwMDAwMCBuIAowMDAwMDU2Mjc4IDAwMDAwIG4gCjAwMDAwNTYzMjQgMDAwMDAgbiAKdHJhaWxlcgo8PC9JbmZvIDIzIDAgUi9JRCBbPGMzYzUyOTgwZGJhMWRlMmVhYjZkMzAwMDI2YjhlZGE3Pjw3MDM2OGY1MjI0MjA3NGEwNjUzMDc5NWZmZmVmNTc4YT5dL1Jvb3QgMjIgMCBSL1NpemUgMjQ+PgpzdGFydHhyZWYKNTY0NDcKJSVFT0YK</ns1:ProtocolData>
                     </ns1:CalcProtocol>
                  </ns1:CalcResultCommon>
                  <ns1:CalcResultExtension>
                     <ns1:MaterialPositions>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>43712</ns1:DATProcessId>
                           <ns1:PartNumber>41355A03262</ns1:PartNumber>
                           <ns1:DATPartNumber>41355A03262</ns1:DATPartNumber>
                           <ns1:Description>SEITENWAND V.R.</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>408.34</ns1:ValuePerUnit>
                           <ns1:ValueTotal>408.34</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>408.34</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:SparePartHistoryPositions>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>41357248660</ns1:PartNumber>
                                 <ns1:LastUPE>349.55</ns1:LastUPE>
                                 <ns1:LastUPEDate>2022-05-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                           </ns1:SparePartHistoryPositions>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>44910</ns1:DATProcessId>
                           <ns1:PartNumber>51317333835</ns1:PartNumber>
                           <ns1:DATPartNumber>51317333835</ns1:DATPartNumber>
                           <ns1:Description>FRONTSCHEIBE</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>877.6</ns1:ValuePerUnit>
                           <ns1:ValueTotal>877.6</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>877.6</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:SparePartHistoryPositions>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51314899567</ns1:PartNumber>
                                 <ns1:LastUPE>593.19</ns1:LastUPE>
                                 <ns1:LastUPEDate>2014-02-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51317280748</ns1:PartNumber>
                                 <ns1:LastUPE>593.19</ns1:LastUPE>
                                 <ns1:LastUPEDate>2014-02-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51317280748</ns1:PartNumber>
                                 <ns1:LastUPE>593.19</ns1:LastUPE>
                                 <ns1:LastUPEDate>2012-11-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                           </ns1:SparePartHistoryPositions>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>40270</ns1:DATProcessId>
                           <ns1:PartNumber>51489162739</ns1:PartNumber>
                           <ns1:DATPartNumber>51489162739</ns1:DATPartNumber>
                           <ns1:Description>SCHALLISOLIERUNG FRONTSCHEIBE WINDLAUF</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>54.27</ns1:ValuePerUnit>
                           <ns1:ValueTotal>54.27</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>54.27</ns1:ValueTotalCorrected>
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
                           <ns1:Description>ABDECKUNG FRONTSCHEIBE O.</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>26.06</ns1:ValuePerUnit>
                           <ns1:ValueTotal>26.06</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>26.06</ns1:ValueTotalCorrected>
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
                           <ns1:Description>REP.-SATZ EINGLASUNG FRONTSCHEIBE</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>66.18</ns1:ValuePerUnit>
                           <ns1:ValueTotal>66.18</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>66.18</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:SparePartHistoryPositions>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51311958028</ns1:PartNumber>
                                 <ns1:LastUPE>32.69</ns1:LastUPE>
                                 <ns1:LastUPEDate>2016-04-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83199407850</ns1:PartNumber>
                                 <ns1:LastUPE>51.26</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>81220142749</ns1:PartNumber>
                                 <ns1:LastUPE>51.26</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>81229407497</ns1:PartNumber>
                                 <ns1:LastUPE>51.26</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147369</ns1:PartNumber>
                                 <ns1:LastUPE>42.44</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147370</ns1:PartNumber>
                                 <ns1:LastUPE>73.11</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147371</ns1:PartNumber>
                                 <ns1:LastUPE>42.44</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147372</ns1:PartNumber>
                                 <ns1:LastUPE>73.11</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190392461</ns1:PartNumber>
                                 <ns1:LastUPE>184.03</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190393939</ns1:PartNumber>
                                 <ns1:LastUPE>41.18</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190393940</ns1:PartNumber>
                                 <ns1:LastUPE>17.65</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190444141</ns1:PartNumber>
                                 <ns1:LastUPE>47.9</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-06-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51318109154</ns1:PartNumber>
                                 <ns1:LastUPE>81.59</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83199407714</ns1:PartNumber>
                                 <ns1:LastUPE>70.59</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>81220142749</ns1:PartNumber>
                                 <ns1:LastUPE>51.26</ns1:LastUPE>
                                 <ns1:LastUPEDate>2014-02-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>81229407497</ns1:PartNumber>
                                 <ns1:LastUPE>51.26</ns1:LastUPE>
                                 <ns1:LastUPEDate>2014-02-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147369</ns1:PartNumber>
                                 <ns1:LastUPE>42.44</ns1:LastUPE>
                                 <ns1:LastUPEDate>2009-05-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147370</ns1:PartNumber>
                                 <ns1:LastUPE>73.11</ns1:LastUPE>
                                 <ns1:LastUPEDate>2010-03-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147371</ns1:PartNumber>
                                 <ns1:LastUPE>42.44</ns1:LastUPE>
                                 <ns1:LastUPEDate>2014-02-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147372</ns1:PartNumber>
                                 <ns1:LastUPE>73.11</ns1:LastUPE>
                                 <ns1:LastUPEDate>2014-02-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                           </ns1:SparePartHistoryPositions>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>45335</ns1:DATProcessId>
                           <ns1:PartNumber>61359856157</ns1:PartNumber>
                           <ns1:DATPartNumber>61359856157</ns1:DATPartNumber>
                           <ns1:Description>SILIKONFOLIE REGEN-/LICHTSENSOR</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>27.08</ns1:ValuePerUnit>
                           <ns1:ValueTotal>27.08</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>27.08</ns1:ValueTotalCorrected>
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
                           <ns1:Description>PUFFER</ns1:Description>
                           <ns1:Amount>11</ns1:Amount>
                           <ns1:ValuePerUnit>1.95</ns1:ValuePerUnit>
                           <ns1:ValueTotal>21.45</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>21.45</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:SparePartHistoryPositions>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51314875651</ns1:PartNumber>
                                 <ns1:LastUPE>1.49</ns1:LastUPE>
                                 <ns1:LastUPEDate>2011-05-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                           </ns1:SparePartHistoryPositions>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:PartNumber>83192211217</ns1:PartNumber>
                           <ns1:DATPartNumber>83192211217</ns1:DATPartNumber>
                           <ns1:Description>REINIGER (100 ML.)</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>11.55</ns1:ValuePerUnit>
                           <ns1:ValueTotal>11.55</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>11.55</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:SparePartHistoryPositions>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83192157286</ns1:PartNumber>
                                 <ns1:LastUPE>9.05</ns1:LastUPE>
                                 <ns1:LastUPEDate>2011-07-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                           </ns1:SparePartHistoryPositions>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:PartNumber>51317288462</ns1:PartNumber>
                           <ns1:DATPartNumber>51317288462</ns1:DATPartNumber>
                           <ns1:Description>PUFFER</ns1:Description>
                           <ns1:Amount>6</ns1:Amount>
                           <ns1:ValuePerUnit>1.95</ns1:ValuePerUnit>
                           <ns1:ValueTotal>11.7</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>11.7</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:SparePartHistoryPositions>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51314875651</ns1:PartNumber>
                                 <ns1:LastUPE>1.49</ns1:LastUPE>
                                 <ns1:LastUPEDate>2011-05-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                           </ns1:SparePartHistoryPositions>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                     </ns1:MaterialPositions>
                     <ns1:LabourPositions>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>43712</ns1:DATProcessId>
                           <ns1:LabourPositionKind>1</ns1:LabourPositionKind>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:LabourPosId>41 35 555</ns1:LabourPosId>
                           <ns1:Description>SEITENWAND V.R. ERS.</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>1.58</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>165.9</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>165.9</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>41 35 555</ns1:WorkNumber>
                           <ns1:SparePartNumber>41355A03262</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>43712</ns1:DATProcessId>
                           <ns1:LabourPositionKind>4</ns1:LabourPositionKind>
                           <ns1:RepairType>body cavity protection</ns1:RepairType>
                           <ns1:LabourPosId>97 35 511</ns1:LabourPosId>
                           <ns1:Description>HOHLRAUMKONSERVIERUNG SEITENWAND V.R.</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>0.42</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>44.1</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>44.1</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>true</ns1:hasRequiredByPosition>
                           <ns1:RequiredByPosition>
                              <ns1:DATProcessId>43712</ns1:DATProcessId>
                              <ns1:RepairType>replace</ns1:RepairType>
                           </ns1:RequiredByPosition>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>97 35 511</ns1:WorkNumber>
                           <ns1:SparePartNumber>41355A03262</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>44910</ns1:DATProcessId>
                           <ns1:LabourPositionKind>1</ns1:LabourPositionKind>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:LabourPosId>51 31 513</ns1:LabourPosId>
                           <ns1:Description>FRONTSCHEIBE A+E/ERS.</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>2.58</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>270.9</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>270.9</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>51 31 513</ns1:WorkNumber>
                           <ns1:SparePartNumber>51317333835</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>14449</ns1:DATProcessId>
                           <ns1:LabourPositionKind>4</ns1:LabourPositionKind>
                           <ns1:RepairType>adjust</ns1:RepairType>
                           <ns1:LabourPosId>66 51 525</ns1:LabourPosId>
                           <ns1:Description>KAMERA FAHRASSISTENZ-SYSTEME KALIBRIEREN</ns1:Description>
                           <ns1:WageType>electric</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>0.33</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>34.65</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>34.65</ns1:ValueTotalCorrected>
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
                        <ns1:LabourPosition>
                           <ns1:LabourPositionKind>8</ns1:LabourPositionKind>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:LabourPosId>ARBEITSAUFWAND</ns1:LabourPosId>
                           <ns1:Description>ERGAENZUNG HAUPTARBEIT</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>0.17</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>17.85</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>17.85</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>DAT#</ns1:WorkNumber>
                        </ns1:LabourPosition>
                     </ns1:LabourPositions>
                     <ns1:LacquerPositions>
                        <ns1:LacquerPosition>
                           <ns1:DATProcessId>43712</ns1:DATProcessId>
                           <ns1:LabourPosId>99 35 011</ns1:LabourPosId>
                           <ns1:Description>SEITENWAND V.R. UMFASST: VORBEREITUNGSARBEITEN</ns1:Description>
                           <ns1:Level>4</ns1:Level>
                           <ns1:LevelDescription>new</ns1:LevelDescription>
                           <ns1:LevelManufacturer>ST.2</ns1:LevelManufacturer>
                           <ns1:Duration>2.42</ns1:Duration>
                           <ns1:ManualDuration>false</ns1:ManualDuration>
                           <ns1:Material>72.6</ns1:Material>
                           <ns1:ValueTotal>363</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>363</ns1:ValueTotalCorrected>
                           <ns1:WageLevel1>290.4</ns1:WageLevel1>
                           <ns1:WorkNumber>99 35 011</ns1:WorkNumber>
                           <ns1:LacquerPositionTimeState/>
                           <ns1:LacquerPositionMaterialState/>
                           <ns1:LacquerPositionPriceState/>
                           <ns1:MaterialType>2</ns1:MaterialType>
                           <ns1:SparePartNumber>41355A03262</ns1:SparePartNumber>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                        </ns1:LacquerPosition>
                     </ns1:LacquerPositions>
                     <ns1:PriceDate>2023-12-01+01:00</ns1:PriceDate>
                     <ns1:RepairCalculationSummary>
                        <ns1:SparePartsCosts>
                           <ns1:AllSum>1504.23</ns1:AllSum>
                           <ns1:ConsumablesSurcharge>30.08</ns1:ConsumablesSurcharge>
                           <ns1:ConsumablesSurchargePercentage>2</ns1:ConsumablesSurchargePercentage>
                           <ns1:TotalSum>1534.31</ns1:TotalSum>
                        </ns1:SparePartsCosts>
                        <ns1:AuxiliaryCosts/>
                        <ns1:LabourCosts>
                           <ns1:AllSum>533.4</ns1:AllSum>
                           <ns1:Bodywork>
                              <ns1:Type>CAR BODY</ns1:Type>
                              <ns1:Units>4.75</ns1:Units>
                              <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                              <ns1:Price>498.75</ns1:Price>
                           </ns1:Bodywork>
                           <ns1:Electric>
                              <ns1:Type>ELECTRICS</ns1:Type>
                              <ns1:Units>0.33</ns1:Units>
                              <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                              <ns1:Price>34.65</ns1:Price>
                           </ns1:Electric>
                           <ns1:Mechanic>
                              <ns1:Type>MECHANICS</ns1:Type>
                              <ns1:Units>0</ns1:Units>
                              <ns1:Price>0</ns1:Price>
                           </ns1:Mechanic>
                           <ns1:TotalSum>533.4</ns1:TotalSum>
                           <ns1:Wages/>
                           <ns1:Works>
                              <ns1:Work>
                                 <ns1:Type>CAR BODY</ns1:Type>
                                 <ns1:WageLevel>1</ns1:WageLevel>
                                 <ns1:Units>4.75</ns1:Units>
                                 <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                                 <ns1:Price>498.75</ns1:Price>
                              </ns1:Work>
                              <ns1:Work>
                                 <ns1:Type>ELECTRICS</ns1:Type>
                                 <ns1:WageLevel>1</ns1:WageLevel>
                                 <ns1:Units>0.33</ns1:Units>
                                 <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                                 <ns1:Price>34.65</ns1:Price>
                              </ns1:Work>
                           </ns1:Works>
                        </ns1:LabourCosts>
                        <ns1:LacquerCosts>
                           <ns1:Wage>
                              <ns1:Type>LACQUER WORK</ns1:Type>
                              <ns1:Units>2.42</ns1:Units>
                              <ns1:PricePerUnit>120.00</ns1:PricePerUnit>
                              <ns1:Price>290.40</ns1:Price>
                           </ns1:Wage>
                           <ns1:TotalWages>290.40</ns1:TotalWages>
                           <ns1:Material>
                              <ns1:FlatPercentage>25</ns1:FlatPercentage>
                              <ns1:FlatAmount>72.6</ns1:FlatAmount>
                              <ns1:MaterialGroups/>
                              <ns1:TotalSum>72.6</ns1:TotalSum>
                              <ns1:SumMaterialCorrected>72.6</ns1:SumMaterialCorrected>
                           </ns1:Material>
                           <ns1:TotalSum>363</ns1:TotalSum>
                        </ns1:LacquerCosts>
                        <ns1:TotalNetCosts>2430.71</ns1:TotalNetCosts>
                        <ns1:TotalVAT>461.83</ns1:TotalVAT>
                        <ns1:TotalGrossCosts>2892.54</ns1:TotalGrossCosts>
                        <ns1:TotalNetCorrected>2430.71</ns1:TotalNetCorrected>
                        <ns1:TotalVATCorrected>461.83</ns1:TotalVATCorrected>
                        <ns1:TotalGrossCorrected>2892.54</ns1:TotalGrossCorrected>
                        <ns1:SumNet>2430.71</ns1:SumNet>
                        <ns1:SumGross>2892.54</ns1:SumGross>
                        <ns1:SumSparePartCosts>1504.23</ns1:SumSparePartCosts>
                        <ns1:SumSmallSparePartCosts>30.08</ns1:SumSmallSparePartCosts>
                        <ns1:SumLabourCosts>533.4</ns1:SumLabourCosts>
                        <ns1:MetaPositions>
                           <ns1:MetaPosition key="TIME_UNIT_SYSTEM" value="STD"/>
                           <ns1:MetaPosition key="LACQUER_TIME_UNIT_SYSTEM" value="STD"/>
                           <ns1:MetaPosition key="DAT_EUROLACQUER_IN_HOURS" value="false"/>
                           <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EQUIPMENT" value="false"/>
                           <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EXTENSION" value="false"/>
                           <ns1:MetaPosition key="FLAT_PERCENTAGE_BASE" value="290.4"/>
                        </ns1:MetaPositions>
                     </ns1:RepairCalculationSummary>
                  </ns1:CalcResultExtension>
                  <ns1:CalculationSummary>
                     <ns1:SparePartsCosts>
                        <ns1:AllSum>1477.15</ns1:AllSum>
                        <ns1:ConsumablesSurcharge>29.54</ns1:ConsumablesSurcharge>
                        <ns1:ConsumablesSurchargePercentage>2</ns1:ConsumablesSurchargePercentage>
                        <ns1:TotalSum>1506.69</ns1:TotalSum>
                     </ns1:SparePartsCosts>
                     <ns1:AuxiliaryCosts/>
                     <ns1:LabourCosts>
                        <ns1:AllSum>533.4</ns1:AllSum>
                        <ns1:Bodywork>
                           <ns1:Type>CAR BODY</ns1:Type>
                           <ns1:Units>4.75</ns1:Units>
                           <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                           <ns1:Price>498.75</ns1:Price>
                        </ns1:Bodywork>
                        <ns1:Electric>
                           <ns1:Type>ELECTRICS</ns1:Type>
                           <ns1:Units>0.33</ns1:Units>
                           <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                           <ns1:Price>34.65</ns1:Price>
                        </ns1:Electric>
                        <ns1:Mechanic>
                           <ns1:Type>MECHANICS</ns1:Type>
                           <ns1:Units>0</ns1:Units>
                           <ns1:Price>0</ns1:Price>
                        </ns1:Mechanic>
                        <ns1:TotalSum>533.4</ns1:TotalSum>
                        <ns1:Wages/>
                        <ns1:Works>
                           <ns1:Work>
                              <ns1:Type>CAR BODY</ns1:Type>
                              <ns1:WageLevel>1</ns1:WageLevel>
                              <ns1:Units>4.75</ns1:Units>
                              <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                              <ns1:Price>498.75</ns1:Price>
                           </ns1:Work>
                           <ns1:Work>
                              <ns1:Type>ELECTRICS</ns1:Type>
                              <ns1:WageLevel>1</ns1:WageLevel>
                              <ns1:Units>0.33</ns1:Units>
                              <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                              <ns1:Price>34.65</ns1:Price>
                           </ns1:Work>
                        </ns1:Works>
                     </ns1:LabourCosts>
                     <ns1:LacquerCosts>
                        <ns1:Wage>
                           <ns1:Type>LACQUER WORK</ns1:Type>
                           <ns1:Units>2.42</ns1:Units>
                           <ns1:PricePerUnit>120.00</ns1:PricePerUnit>
                           <ns1:Price>290.40</ns1:Price>
                        </ns1:Wage>
                        <ns1:TotalWages>290.40</ns1:TotalWages>
                        <ns1:Material>
                           <ns1:FlatPercentage>25</ns1:FlatPercentage>
                           <ns1:FlatAmount>72.6</ns1:FlatAmount>
                           <ns1:MaterialGroups/>
                           <ns1:TotalSum>72.6</ns1:TotalSum>
                           <ns1:SumMaterialCorrected>72.6</ns1:SumMaterialCorrected>
                        </ns1:Material>
                        <ns1:TotalSum>363</ns1:TotalSum>
                     </ns1:LacquerCosts>
                     <ns1:TotalNetCosts>2403.09</ns1:TotalNetCosts>
                     <ns1:TotalVAT>456.59</ns1:TotalVAT>
                     <ns1:TotalGrossCosts>2859.68</ns1:TotalGrossCosts>
                     <ns1:TotalNetCorrected>2403.09</ns1:TotalNetCorrected>
                     <ns1:TotalVATCorrected>456.59</ns1:TotalVATCorrected>
                     <ns1:TotalGrossCorrected>2859.68</ns1:TotalGrossCorrected>
                     <ns1:SumNet>2403.09</ns1:SumNet>
                     <ns1:SumGross>2859.68</ns1:SumGross>
                     <ns1:SumSparePartCosts>1477.15</ns1:SumSparePartCosts>
                     <ns1:SumSmallSparePartCosts>29.54</ns1:SumSmallSparePartCosts>
                     <ns1:SumLabourCosts>533.4</ns1:SumLabourCosts>
                     <ns1:MetaPositions>
                        <ns1:MetaPosition key="TOTAL_NET_RISK" value="27.08"/>
                        <ns1:MetaPosition key="VAT_RISK" value="5.15"/>
                        <ns1:MetaPosition key="TOTAL_GROSS_RISK" value="32.23"/>
                        <ns1:MetaPosition key="TIME_UNIT_SYSTEM" value="STD"/>
                        <ns1:MetaPosition key="LACQUER_TIME_UNIT_SYSTEM" value="STD"/>
                        <ns1:MetaPosition key="DAT_EUROLACQUER_IN_HOURS" value="false"/>
                        <ns1:MetaPosition key="TOTAL_PRICE_SPARE_PARTS_RISK" value="27.08"/>
                        <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EQUIPMENT" value="false"/>
                        <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EXTENSION" value="false"/>
                        <ns1:MetaPosition key="FLAT_PERCENTAGE_BASE" value="290.4"/>
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
                  <ns1:OrderNumber>60774959    20231222120449501</ns1:OrderNumber>
                  <ns1:InvoiceDate>2023-12-22T12:05:00.056+01:00</ns1:InvoiceDate>
               </ns1:RepairOrder>
               <ns1:InsuranceClaim>false</ns1:InsuranceClaim>
               <ns1:ProcessManagement/>
            </ns1:Dossier>
         </contractResult>
      </ns4:getContractResponse>
   </S:Body>
</S:Envelope>

   
   <S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns4:getContractResponse xmlns:ns4="http://sphinx.dat.de/services/VehicleRepairService">
         <contractResult source="SD3" type="VehicleRepairOnline">
            <ns1:Dossier xmlns:ns1="http://www.dat.de/vxs">
               <ns1:Description>DAT-TEST_12:04:49,275</ns1:Description>
               <ns1:UUID>8b377208-37db-4e6c-9e0d-bf464abcc517</ns1:UUID>
               <ns1:DossierId>9999999</ns1:DossierId>
               <ns1:IdSD3Network>9999999</ns1:IdSD3Network>
               <ns1:Country>DE</ns1:Country>
               <ns1:Language>de_DE</ns1:Language>
               <ns1:DataVersion>1</ns1:DataVersion>
               <ns1:Currency>EUR</ns1:Currency>
               <ns1:DatCustomerId>111111111</ns1:DatCustomerId>
               <ns1:DossierType>repair</ns1:DossierType>
               <ns1:CreateDate>2023-12-22T12:04:49+01:00</ns1:CreateDate>
               <ns1:CreateUser>Anwender</ns1:CreateUser>
               <ns1:ChangeDate>2023-12-22T12:04:49+01:00</ns1:ChangeDate>
               <ns1:DatCustomerAddress>
                  <ns1:Title>titleCompany</ns1:Title>
                  <ns1:CompanyName>DAT - Intern</ns1:CompanyName>
                  <ns1:NameLong>Schulung SST-Partner</ns1:NameLong>
                  <ns1:Country>DE</ns1:Country>
                  <ns1:CustomerNumber>111111111</ns1:CustomerNumber>
                  <ns1:CustomerType>111111111</ns1:CustomerType>
                  <ns1:Street>Hellmuth-Hirth-Str.</ns1:Street>
                  <ns1:StreetNumber>1</ns1:StreetNumber>
                  <ns1:StreetZipCode>73760</ns1:StreetZipCode>
                  <ns1:StreetCity>Ostfildern</ns1:StreetCity>
                  <ns1:EMail>kundendienst@dat.de</ns1:EMail>
                  <ns1:PhoneBusiness>+49 711/4500000</ns1:PhoneBusiness>
                  <ns1:UsageFlag>9</ns1:UsageFlag>
               </ns1:DatCustomerAddress>
               <ns1:Vehicle>
                  <ns1:VehicleIdentNumber>WBADEXTESTSTUB001</ns1:VehicleIdentNumber>
                  <ns1:DatECode>011301110300002</ns1:DatECode>
                  <ns1:Container>DE006</ns1:Container>
                  <ns1:ConstructionTime>5297</ns1:ConstructionTime>
                  <ns1:InitialRegistration>2013-11-23+01:00</ns1:InitialRegistration>
                  <ns1:MileageEstimated>654321</ns1:MileageEstimated>
                  <ns1:MileageOdometer>654321</ns1:MileageOdometer>
                  <ns1:VehicleTypeName origin="dat">Pkw, SUV, Kleintransporter</ns1:VehicleTypeName>
                  <ns1:VehicleTypeNameN origin="dat">Pkw, SUV, Kleintransporter</ns1:VehicleTypeNameN>
                  <ns1:ManufacturerName origin="dat">BMW</ns1:ManufacturerName>
                  <ns1:BaseModelName origin="dat">Baureihe 5 Touring (F11)(2010->)</ns1:BaseModelName>
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
                  <ns1:RegistrationData>
                     <ns1:LicenseNumber>ES SM1122</ns1:LicenseNumber>
                  </ns1:RegistrationData>
                  <ns1:Engine/>
                  <ns1:TechInfo>
                     <ns1:FillingQuantities>
                        <ns1:Fluid code="N47D20" desc="Motor" type="1">
                           <ns1:Capacity condition="Servicebefüllung" desc="Füllmenge (gesamt)" min="5.20" unit="Liter"/>
                           <ns1:Recommendation>
                              <ns1:Usage type="0">Normal</ns1:Usage>
                              <ns1:Interval type="1">Wechseln 30000 km/ 24 Monate</ns1:Interval>
                              <ns1:Product>TITAN GT1 PRO FLEX SAE 5W-30 (XTL-Technology)</ns1:Product>
                              <ns1:Product>TITAN GT1 PRO C-3 SAE 5W-30 (XTL-Technology)</ns1:Product>
                              <ns1:Product>TITAN GT1 SAE 5W-40 (XTL-Technology)</ns1:Product>
                           </ns1:Recommendation>
                        </ns1:Fluid>
                        <ns1:Fluid desc="Kühlsystem" type="8">
                           <ns1:Capacity desc="Füllmenge (gesamt)" max="7.50" min="7.20" unit="Liter"/>
                           <ns1:Recommendation>
                              <ns1:Usage type="0">Normal</ns1:Usage>
                              <ns1:Product>MAINTAIN FRICOFIN</ns1:Product>
                           </ns1:Recommendation>
                        </ns1:Fluid>
                        <ns1:Fluid code="205AL" desc="Hinterachsgetriebe" type="3">
                           <ns1:Capacity desc="Füllmenge (gesamt)" min="0.80" unit="Liter"/>
                           <ns1:Recommendation>
                              <ns1:Usage type="0">Normal</ns1:Usage>
                              <ns1:Product>TITAN SINTOPOID LS SAE 75W-90</ns1:Product>
                           </ns1:Recommendation>
                        </ns1:Fluid>
                        <ns1:Fluid code="ZF GA8HP 8/1" desc="Automatikgetriebe" type="3">
                           <ns1:Capacity desc="Füllmenge (gesamt)" min="8.50" unit="Liter"/>
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
                           <ns1:Description>Airbag Beifahrerseite abschaltbar</ns1:Description>
                           <ns1:EquipmentGroup>AIR2</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26803</ns1:DatEquipmentId>
                           <ns1:Description>Airbag Fahrer-/Beifahrerseite</ns1:Description>
                           <ns1:EquipmentGroup>AIR1</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>34704</ns1:DatEquipmentId>
                           <ns1:Description>Aktive Kopfstützen</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>10715</ns1:DatEquipmentId>
                           <ns1:Description>Aktive Motorhaube</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40000</ns1:DatEquipmentId>
                           <ns1:Description>Anti-Blockier-System (ABS)</ns1:Description>
                           <ns1:EquipmentGroup>ABS</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18604</ns1:DatEquipmentId>
                           <ns1:Description>Automatische Fahrlichtschaltung</ns1:Description>
                           <ns1:EquipmentGroup>AUFL</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>24999</ns1:DatEquipmentId>
                           <ns1:Description>AUX-IN-Anschluss (AUX-IN)</ns1:Description>
                           <ns1:EquipmentGroup>MP3A</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>15200</ns1:DatEquipmentId>
                           <ns1:Description>Außenspiegel elektr. verstell- und heizbar</ns1:Description>
                           <ns1:EquipmentGroup>AUSP</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25702</ns1:DatEquipmentId>
                           <ns1:Description>Außentemperaturanzeige</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18505</ns1:DatEquipmentId>
                           <ns1:Description>Bi-Xenon-Scheinwerfer</ns1:Description>
                           <ns1:EquipmentGroup>XELI</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>19000</ns1:DatEquipmentId>
                                 <ns1:Description>Scheinwerfer-Reinigungsanlage (SRA)</ns1:Description>
                                 <ns1:EquipmentGroup>SWRA</ns1:EquipmentGroup>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>18913</ns1:DatEquipmentId>
                                 <ns1:Description>Tagfahrlicht LED</ns1:Description>
                                 <ns1:EquipmentGroup>TFAL</ns1:EquipmentGroup>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>18940</ns1:DatEquipmentId>
                                 <ns1:Description>Blinkleuchten LED</ns1:Description>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25508</ns1:DatEquipmentId>
                           <ns1:Description>Bordcomputer</ns1:Description>
                           <ns1:EquipmentGroup>COMP</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40801</ns1:DatEquipmentId>
                           <ns1:Description>Bremsassistent</ns1:Description>
                           <ns1:EquipmentGroup>FA01</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40050</ns1:DatEquipmentId>
                           <ns1:Description>Bremsenergierückgewinnung (Rekuperationssystem)</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25606</ns1:DatEquipmentId>
                           <ns1:Description>Check-Control-System</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25300</ns1:DatEquipmentId>
                           <ns1:Description>Drehzahlmesser</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18898</ns1:DatEquipmentId>
                           <ns1:Description>Dynamische Bremsleuchte</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>70100</ns1:DatEquipmentId>
                           <ns1:Description>Dynamische Stabilitäts-Control (DSC)</ns1:Description>
                           <ns1:EquipmentGroup>ESP</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>11406</ns1:DatEquipmentId>
                           <ns1:Description>Exterieurumfänge Wagenfarbe</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>70518</ns1:DatEquipmentId>
                           <ns1:Description>Fahrassistenz-System: Fahrerlebnisschalter</ns1:Description>
                           <ns1:EquipmentGroup>FA22</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35003</ns1:DatEquipmentId>
                           <ns1:Description>Fensterheber elektrisch vorn + hinten</ns1:Description>
                           <ns1:EquipmentGroup>FH4</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>24833</ns1:DatEquipmentId>
                           <ns1:Description>Freisprecheinrichtung mit USB-Schnittstelle</ns1:Description>
                           <ns1:EquipmentGroup>TEL3</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>28402</ns1:DatEquipmentId>
                           <ns1:Description>Fußmatten Velours</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27605</ns1:DatEquipmentId>
                           <ns1:Description>Gepäckraum-Abtrennung (Netz)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27400</ns1:DatEquipmentId>
                           <ns1:Description>Gepäckraumabdeckung / Rollo</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26710</ns1:DatEquipmentId>
                           <ns1:Description>Geschwindigkeits-Regelanlage mit Bremsfunktion</ns1:Description>
                           <ns1:EquipmentGroup>TEMP</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39402</ns1:DatEquipmentId>
                           <ns1:Description>Getränkehalter vorn und hinten</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35506</ns1:DatEquipmentId>
                           <ns1:Description>Heckklappenbetätigung automatisch</ns1:Description>
                           <ns1:EquipmentGroup>HKEL</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>19300</ns1:DatEquipmentId>
                           <ns1:Description>Heckscheibenwischer</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39308</ns1:DatEquipmentId>
                           <ns1:Description>Isofix-Aufnahmen für Kindersitz an Rücksitz</ns1:Description>
                           <ns1:EquipmentGroup>KISI</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                           <ns1:Description>Karosserie: 5-türig</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26805</ns1:DatEquipmentId>
                           <ns1:Description>Kopf-Airbag-System hinten</ns1:Description>
                           <ns1:EquipmentGroup>AIR4</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26804</ns1:DatEquipmentId>
                           <ns1:Description>Kopf-Airbag-System vorn</ns1:Description>
                           <ns1:EquipmentGroup>AIR4</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>69007</ns1:DatEquipmentId>
                           <ns1:Description>Lenkrad (Leder) mit Multifunktion</ns1:Description>
                           <ns1:EquipmentGroup>LEN2</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>69505</ns1:DatEquipmentId>
                                 <ns1:Description>Lenksäule (Lenkrad) mechan. verstellbar</ns1:Description>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>69505</ns1:DatEquipmentId>
                           <ns1:Description>Lenksäule (Lenkrad) mechan. verstellbar</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>48535</ns1:DatEquipmentId>
                           <ns1:Description>LM-Felgen 8x17 (V-Speiche 236)</ns1:Description>
                           <ns1:EquipmentGroup>ALU</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>42905</ns1:DatEquipmentId>
                           <ns1:Description>Luftfederung Hinterachse</ns1:Description>
                           <ns1:EquipmentGroup>LUFT</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>42805</ns1:DatEquipmentId>
                                 <ns1:Description>Niveauregulierung</ns1:Description>
                                 <ns1:EquipmentGroup>NIV</ns1:EquipmentGroup>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27300</ns1:DatEquipmentId>
                           <ns1:Description>Mittelarmlehne hinten</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27202</ns1:DatEquipmentId>
                           <ns1:Description>Mittelarmlehne vorn</ns1:Description>
                           <ns1:EquipmentGroup>MALV</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>87410</ns1:DatEquipmentId>
                           <ns1:Description>Motor 2,0 Ltr. - 135 kW Turbodiesel KAT (N 47 T)</ns1:Description>
                           <ns1:EquipmentType>engine</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>96508</ns1:DatEquipmentId>
                                 <ns1:Description>Motor 2,0 Ltr. - 135 kW Turbodiesel</ns1:Description>
                                 <ns1:EquipmentType>engine</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27309</ns1:DatEquipmentId>
                           <ns1:Description>Multifunktionsarmlehne im Fond</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>42805</ns1:DatEquipmentId>
                           <ns1:Description>Niveauregulierung</ns1:Description>
                           <ns1:EquipmentGroup>NIV</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>77015</ns1:DatEquipmentId>
                           <ns1:Description>NOx-Speicherkatalysator (BMW Blue Performance)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40803</ns1:DatEquipmentId>
                           <ns1:Description>Parkbremse elektrisch</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>62004</ns1:DatEquipmentId>
                           <ns1:Description>Reifen 225/55 R17 ..Z</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>68802</ns1:DatEquipmentId>
                           <ns1:Description>Reifen-Reparaturset (Mobility-Pack)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25906</ns1:DatEquipmentId>
                           <ns1:Description>Reifenpannen-Anzeige</ns1:Description>
                           <ns1:EquipmentGroup>RDK</ns1:EquipmentGroup>
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
                           <ns1:DatEquipmentId>33508</ns1:DatEquipmentId>
                           <ns1:Description>Rücksitzlehne geteilt/klappbar</ns1:Description>
                           <ns1:EquipmentGroup>SITH</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>77227</ns1:DatEquipmentId>
                           <ns1:Description>Schadstoffarm nach Abgasnorm Euro 6</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>19102</ns1:DatEquipmentId>
                           <ns1:Description>Scheibenwaschdüsen heizbar</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>19101</ns1:DatEquipmentId>
                           <ns1:Description>Scheibenwischer mit Regensensor</ns1:Description>
                           <ns1:EquipmentGroup>SWRE</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>19000</ns1:DatEquipmentId>
                           <ns1:Description>Scheinwerfer-Reinigungsanlage (SRA)</ns1:Description>
                           <ns1:EquipmentGroup>SWRA</ns1:EquipmentGroup>
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
                           <ns1:DatEquipmentId>25151</ns1:DatEquipmentId>
                           <ns1:Description>Service-System: Intelligenter Notruf inkl. TeleServices</ns1:Description>
                           <ns1:EquipmentGroup>FA10</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>69811</ns1:DatEquipmentId>
                           <ns1:Description>Servolenkung Servotronic</ns1:Description>
                           <ns1:EquipmentGroup>SL</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>32811</ns1:DatEquipmentId>
                           <ns1:Description>Sitze vorn teilelektr. verstellbar</ns1:Description>
                           <ns1:EquipmentGroup>SITE</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35408</ns1:DatEquipmentId>
                           <ns1:Description>Soft-Close-Automatik für Kofferraum / Heckklappe</ns1:Description>
                           <ns1:EquipmentGroup>HKEL</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35513</ns1:DatEquipmentId>
                           <ns1:Description>Start-Stop-Knopf</ns1:Description>
                           <ns1:EquipmentGroup>MSSA</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>77601</ns1:DatEquipmentId>
                           <ns1:Description>Start/Stop-Anlage (Funktion)</ns1:Description>
                           <ns1:EquipmentGroup>MSSA</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39016</ns1:DatEquipmentId>
                           <ns1:Description>Steckdose (12V-Anschluß) 3-fach</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>73017</ns1:DatEquipmentId>
                           <ns1:Description>Vlies-Batterie 80 Ah (AGM)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>38105</ns1:DatEquipmentId>
                           <ns1:Description>Wegfahrsperre</ns1:Description>
                           <ns1:EquipmentGroup>WFS</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>22218</ns1:DatEquipmentId>
                           <ns1:Description>Wärme-/Sonnenschutzverglasung kombiniert (hinten abgedunkelt)</ns1:Description>
                           <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
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
                           <ns1:DatEquipmentId>96508</ns1:DatEquipmentId>
                           <ns1:Description>Motor 2,0 Ltr. - 135 kW Turbodiesel</ns1:Description>
                           <ns1:EquipmentType>engine</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18913</ns1:DatEquipmentId>
                           <ns1:Description>Tagfahrlicht LED</ns1:Description>
                           <ns1:EquipmentGroup>TFAL</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18940</ns1:DatEquipmentId>
                           <ns1:Description>Blinkleuchten LED</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                     </ns1:SeriesEquipment>
                     <ns1:SpecialEquipment>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>37603</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Ambiente-Beleuchtung</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25804</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Audio-Navigationssystem Professional</ns1:Description>
                           <ns1:EquipmentGroup>GPS</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>24709</ns1:DatEquipmentId>
                                 <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                 <ns1:Description>Sprachbediensystem</ns1:Description>
                                 <ns1:EquipmentGroup>TEL4</ns1:EquipmentGroup>
                                 <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>8702</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Außenausstattung: Shadow-Line Hochglanz</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25930</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Control-Display mit Farbmonitor (9,2 Zoll)</ns1:Description>
                           <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27810</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Dachhimmel Anthrazit (BMW Individual)</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>16198</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Dachreling Hochglanz Shadow-Line</ns1:Description>
                           <ns1:EquipmentGroup>DARE</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25704</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Fahrassistenz-System: Speed-Limit-Anzeige</ns1:Description>
                           <ns1:EquipmentGroup>FA28</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>22505</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Frontscheibe (Ausführung: Klimakomfort)</ns1:Description>
                           <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>75914</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Getriebe Automatik - mit Steptronic (8-Stufen)</ns1:Description>
                           <ns1:EquipmentGroup>AG2</ns1:EquipmentGroup>
                           <ns1:GearBoxType>automatic</ns1:GearBoxType>
                           <ns1:NrOfGears>8</ns1:NrOfGears>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25204</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Head-up-Display</ns1:Description>
                           <ns1:EquipmentGroup>HUD</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>25930</ns1:DatEquipmentId>
                                 <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                 <ns1:Description>Control-Display mit Farbmonitor (9,2 Zoll)</ns1:Description>
                                 <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>25413</ns1:DatEquipmentId>
                                 <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                 <ns1:Description>Instrumentenkombination (erweiterter Umfang)</ns1:Description>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>24607</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>HiFi-Lautsprechersystem</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>31408</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Innenausstattung: Interieurleisten Aluminium Längsschliff fein</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>37901</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Innenspiegel mit Abblendautomatik</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25413</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Instrumentenkombination (erweiterter Umfang)</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>25930</ns1:DatEquipmentId>
                                 <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                 <ns1:Description>Control-Display mit Farbmonitor (9,2 Zoll)</ns1:Description>
                                 <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>28982</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Klimaautomatik 2-Zonen mit autom. Umluft-Control, erweiterter Umfang</ns1:Description>
                           <ns1:EquipmentGroup>KLI2</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>33403</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Lendenwirbelstütze Sitz vorn links und rechts, elektr. verstellbar</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>77240</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Modellvariante CO2-Umfang (Code 1CB)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18313</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Nebelscheinwerfer LED</ns1:Description>
                           <ns1:EquipmentGroup>BEL</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>16302</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Panoramadach (Glas)</ns1:Description>
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
                           <ns1:Description>Sitzbezug / Polsterung: Leder Dakota</ns1:Description>
                           <ns1:EquipmentGroup>LEDE</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>29500</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Sitzheizung vorn</ns1:Description>
                           <ns1:EquipmentGroup>SITB</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>22102</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Sonnenschutzverglasung (hinten abgedunkelt, BMW Individual)</ns1:Description>
                           <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>24709</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Sprachbediensystem</ns1:Description>
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
                        <ns1:Description>Motor 2,0 Ltr. - 135 kW Turbodiesel</ns1:Description>
                        <ns1:EquipmentClass>1</ns1:EquipmentClass>
                     </ns1:EquipmentPosition>
                     <ns1:EquipmentPosition>
                        <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                        <ns1:Description>Karosserie: 5-türig</ns1:Description>
                        <ns1:EquipmentClass>2</ns1:EquipmentClass>
                     </ns1:EquipmentPosition>
                     <ns1:EquipmentPosition>
                        <ns1:DatEquipmentId>75914</ns1:DatEquipmentId>
                        <ns1:Description>Getriebe Automatik - mit Steptronic (8-Stufen)</ns1:Description>
                        <ns1:EquipmentClass>11</ns1:EquipmentClass>
                     </ns1:EquipmentPosition>
                  </ns1:DATECodeEquipment>
               </ns1:Vehicle>
               <ns1:VAT>
                  <ns1:VatAtCalculationTime>19</ns1:VatAtCalculationTime>
               </ns1:VAT>
               <ns1:TradingData>
                  <ns1:Owner>
                     <ns1:Title>titleMrs</ns1:Title>
                     <ns1:TitleEntry>Frau</ns1:TitleEntry>
                     <ns1:LastName>Max</ns1:LastName>
                     <ns1:FirstName>Musterfrau</ns1:FirstName>
                     <ns1:Country>DE</ns1:Country>
                     <ns1:UsageFlag>2</ns1:UsageFlag>
                  </ns1:Owner>
                  <ns1:ClientContactAddresses>
                     <ns1:ClientContactAddress>
                        <ns1:Title>titleCompany</ns1:Title>
                        <ns1:CompanyName>DAT - Intern</ns1:CompanyName>
                        <ns1:NameLong>Schulung SST-Partner</ns1:NameLong>
                        <ns1:Country>DE</ns1:Country>
                        <ns1:CustomerNumber>111111111</ns1:CustomerNumber>
                        <ns1:CustomerType>111111111</ns1:CustomerType>
                        <ns1:Street>Hellmuth-Hirth-Str.</ns1:Street>
                        <ns1:StreetNumber>1</ns1:StreetNumber>
                        <ns1:StreetZipCode>73760</ns1:StreetZipCode>
                        <ns1:StreetCity>Ostfildern</ns1:StreetCity>
                        <ns1:EMail>kundendienst@dat.de</ns1:EMail>
                        <ns1:PhoneBusiness>+49 711/450000</ns1:PhoneBusiness>
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
                     <ns1:InitialRegistration>2013-11-23+01:00</ns1:InitialRegistration>
                     <ns1:MileageEstimated>654321</ns1:MileageEstimated>
                     <ns1:MileageOdometer>654321</ns1:MileageOdometer>
                     <ns1:VehicleTypeName origin="dat">Pkw, SUV, Kleintransporter</ns1:VehicleTypeName>
                     <ns1:VehicleTypeNameN origin="dat">Pkw, SUV, Kleintransporter</ns1:VehicleTypeNameN>
                     <ns1:ManufacturerName origin="dat">BMW</ns1:ManufacturerName>
                     <ns1:BaseModelName origin="dat">Baureihe 5 Touring (F11)(2010->)</ns1:BaseModelName>
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
                     <ns1:RegistrationData>
                        <ns1:LicenseNumber>ES SM1122</ns1:LicenseNumber>
                     </ns1:RegistrationData>
                     <ns1:Engine/>
                     <ns1:TechInfo>
                        <ns1:FillingQuantities>
                           <ns1:Fluid code="N47D20" desc="Motor" type="1">
                              <ns1:Capacity condition="Servicebefüllung" desc="Füllmenge (gesamt)" min="5.20" unit="Liter"/>
                              <ns1:Recommendation>
                                 <ns1:Usage type="0">Normal</ns1:Usage>
                                 <ns1:Interval type="1">Wechseln 30000 km/ 24 Monate</ns1:Interval>
                                 <ns1:Product>TITAN GT1 PRO FLEX SAE 5W-30 (XTL-Technology)</ns1:Product>
                                 <ns1:Product>TITAN GT1 PRO C-3 SAE 5W-30 (XTL-Technology)</ns1:Product>
                                 <ns1:Product>TITAN GT1 SAE 5W-40 (XTL-Technology)</ns1:Product>
                              </ns1:Recommendation>
                           </ns1:Fluid>
                           <ns1:Fluid desc="Kühlsystem" type="8">
                              <ns1:Capacity desc="Füllmenge (gesamt)" max="7.50" min="7.20" unit="Liter"/>
                              <ns1:Recommendation>
                                 <ns1:Usage type="0">Normal</ns1:Usage>
                                 <ns1:Product>MAINTAIN FRICOFIN</ns1:Product>
                              </ns1:Recommendation>
                           </ns1:Fluid>
                           <ns1:Fluid code="205AL" desc="Hinterachsgetriebe" type="3">
                              <ns1:Capacity desc="Füllmenge (gesamt)" min="0.80" unit="Liter"/>
                              <ns1:Recommendation>
                                 <ns1:Usage type="0">Normal</ns1:Usage>
                                 <ns1:Product>TITAN SINTOPOID LS SAE 75W-90</ns1:Product>
                              </ns1:Recommendation>
                           </ns1:Fluid>
                           <ns1:Fluid code="ZF GA8HP 8/1" desc="Automatikgetriebe" type="3">
                              <ns1:Capacity desc="Füllmenge (gesamt)" min="8.50" unit="Liter"/>
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
                              <ns1:Description>Airbag Beifahrerseite abschaltbar</ns1:Description>
                              <ns1:EquipmentGroup>AIR2</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>26803</ns1:DatEquipmentId>
                              <ns1:Description>Airbag Fahrer-/Beifahrerseite</ns1:Description>
                              <ns1:EquipmentGroup>AIR1</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>34704</ns1:DatEquipmentId>
                              <ns1:Description>Aktive Kopfstützen</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>10715</ns1:DatEquipmentId>
                              <ns1:Description>Aktive Motorhaube</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>40000</ns1:DatEquipmentId>
                              <ns1:Description>Anti-Blockier-System (ABS)</ns1:Description>
                              <ns1:EquipmentGroup>ABS</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>18604</ns1:DatEquipmentId>
                              <ns1:Description>Automatische Fahrlichtschaltung</ns1:Description>
                              <ns1:EquipmentGroup>AUFL</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>24999</ns1:DatEquipmentId>
                              <ns1:Description>AUX-IN-Anschluss (AUX-IN)</ns1:Description>
                              <ns1:EquipmentGroup>MP3A</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>15200</ns1:DatEquipmentId>
                              <ns1:Description>Außenspiegel elektr. verstell- und heizbar</ns1:Description>
                              <ns1:EquipmentGroup>AUSP</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25702</ns1:DatEquipmentId>
                              <ns1:Description>Außentemperaturanzeige</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>18505</ns1:DatEquipmentId>
                              <ns1:Description>Bi-Xenon-Scheinwerfer</ns1:Description>
                              <ns1:EquipmentGroup>XELI</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>19000</ns1:DatEquipmentId>
                                    <ns1:Description>Scheinwerfer-Reinigungsanlage (SRA)</ns1:Description>
                                    <ns1:EquipmentGroup>SWRA</ns1:EquipmentGroup>
                                    <ns1:EquipmentType>glass</ns1:EquipmentType>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>18913</ns1:DatEquipmentId>
                                    <ns1:Description>Tagfahrlicht LED</ns1:Description>
                                    <ns1:EquipmentGroup>TFAL</ns1:EquipmentGroup>
                                    <ns1:EquipmentType>glass</ns1:EquipmentType>
                                    <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>18940</ns1:DatEquipmentId>
                                    <ns1:Description>Blinkleuchten LED</ns1:Description>
                                    <ns1:EquipmentType>glass</ns1:EquipmentType>
                                    <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25508</ns1:DatEquipmentId>
                              <ns1:Description>Bordcomputer</ns1:Description>
                              <ns1:EquipmentGroup>COMP</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>40801</ns1:DatEquipmentId>
                              <ns1:Description>Bremsassistent</ns1:Description>
                              <ns1:EquipmentGroup>FA01</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>40050</ns1:DatEquipmentId>
                              <ns1:Description>Bremsenergierückgewinnung (Rekuperationssystem)</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25606</ns1:DatEquipmentId>
                              <ns1:Description>Check-Control-System</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25300</ns1:DatEquipmentId>
                              <ns1:Description>Drehzahlmesser</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>18898</ns1:DatEquipmentId>
                              <ns1:Description>Dynamische Bremsleuchte</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>70100</ns1:DatEquipmentId>
                              <ns1:Description>Dynamische Stabilitäts-Control (DSC)</ns1:Description>
                              <ns1:EquipmentGroup>ESP</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>11406</ns1:DatEquipmentId>
                              <ns1:Description>Exterieurumfänge Wagenfarbe</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>70518</ns1:DatEquipmentId>
                              <ns1:Description>Fahrassistenz-System: Fahrerlebnisschalter</ns1:Description>
                              <ns1:EquipmentGroup>FA22</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>35003</ns1:DatEquipmentId>
                              <ns1:Description>Fensterheber elektrisch vorn + hinten</ns1:Description>
                              <ns1:EquipmentGroup>FH4</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>24833</ns1:DatEquipmentId>
                              <ns1:Description>Freisprecheinrichtung mit USB-Schnittstelle</ns1:Description>
                              <ns1:EquipmentGroup>TEL3</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>28402</ns1:DatEquipmentId>
                              <ns1:Description>Fußmatten Velours</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27605</ns1:DatEquipmentId>
                              <ns1:Description>Gepäckraum-Abtrennung (Netz)</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27400</ns1:DatEquipmentId>
                              <ns1:Description>Gepäckraumabdeckung / Rollo</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>26710</ns1:DatEquipmentId>
                              <ns1:Description>Geschwindigkeits-Regelanlage mit Bremsfunktion</ns1:Description>
                              <ns1:EquipmentGroup>TEMP</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>39402</ns1:DatEquipmentId>
                              <ns1:Description>Getränkehalter vorn und hinten</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>35506</ns1:DatEquipmentId>
                              <ns1:Description>Heckklappenbetätigung automatisch</ns1:Description>
                              <ns1:EquipmentGroup>HKEL</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>19300</ns1:DatEquipmentId>
                              <ns1:Description>Heckscheibenwischer</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>39308</ns1:DatEquipmentId>
                              <ns1:Description>Isofix-Aufnahmen für Kindersitz an Rücksitz</ns1:Description>
                              <ns1:EquipmentGroup>KISI</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                              <ns1:Description>Karosserie: 5-türig</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>26805</ns1:DatEquipmentId>
                              <ns1:Description>Kopf-Airbag-System hinten</ns1:Description>
                              <ns1:EquipmentGroup>AIR4</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>26804</ns1:DatEquipmentId>
                              <ns1:Description>Kopf-Airbag-System vorn</ns1:Description>
                              <ns1:EquipmentGroup>AIR4</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>69007</ns1:DatEquipmentId>
                              <ns1:Description>Lenkrad (Leder) mit Multifunktion</ns1:Description>
                              <ns1:EquipmentGroup>LEN2</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>69505</ns1:DatEquipmentId>
                                    <ns1:Description>Lenksäule (Lenkrad) mechan. verstellbar</ns1:Description>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>69505</ns1:DatEquipmentId>
                              <ns1:Description>Lenksäule (Lenkrad) mechan. verstellbar</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>48535</ns1:DatEquipmentId>
                              <ns1:Description>LM-Felgen 8x17 (V-Speiche 236)</ns1:Description>
                              <ns1:EquipmentGroup>ALU</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>42905</ns1:DatEquipmentId>
                              <ns1:Description>Luftfederung Hinterachse</ns1:Description>
                              <ns1:EquipmentGroup>LUFT</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>42805</ns1:DatEquipmentId>
                                    <ns1:Description>Niveauregulierung</ns1:Description>
                                    <ns1:EquipmentGroup>NIV</ns1:EquipmentGroup>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27300</ns1:DatEquipmentId>
                              <ns1:Description>Mittelarmlehne hinten</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27202</ns1:DatEquipmentId>
                              <ns1:Description>Mittelarmlehne vorn</ns1:Description>
                              <ns1:EquipmentGroup>MALV</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>87410</ns1:DatEquipmentId>
                              <ns1:Description>Motor 2,0 Ltr. - 135 kW Turbodiesel KAT (N 47 T)</ns1:Description>
                              <ns1:EquipmentType>engine</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>96508</ns1:DatEquipmentId>
                                    <ns1:Description>Motor 2,0 Ltr. - 135 kW Turbodiesel</ns1:Description>
                                    <ns1:EquipmentType>engine</ns1:EquipmentType>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27309</ns1:DatEquipmentId>
                              <ns1:Description>Multifunktionsarmlehne im Fond</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>42805</ns1:DatEquipmentId>
                              <ns1:Description>Niveauregulierung</ns1:Description>
                              <ns1:EquipmentGroup>NIV</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>77015</ns1:DatEquipmentId>
                              <ns1:Description>NOx-Speicherkatalysator (BMW Blue Performance)</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>40803</ns1:DatEquipmentId>
                              <ns1:Description>Parkbremse elektrisch</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>62004</ns1:DatEquipmentId>
                              <ns1:Description>Reifen 225/55 R17 ..Z</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>68802</ns1:DatEquipmentId>
                              <ns1:Description>Reifen-Reparaturset (Mobility-Pack)</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25906</ns1:DatEquipmentId>
                              <ns1:Description>Reifenpannen-Anzeige</ns1:Description>
                              <ns1:EquipmentGroup>RDK</ns1:EquipmentGroup>
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
                              <ns1:DatEquipmentId>33508</ns1:DatEquipmentId>
                              <ns1:Description>Rücksitzlehne geteilt/klappbar</ns1:Description>
                              <ns1:EquipmentGroup>SITH</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>77227</ns1:DatEquipmentId>
                              <ns1:Description>Schadstoffarm nach Abgasnorm Euro 6</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>19102</ns1:DatEquipmentId>
                              <ns1:Description>Scheibenwaschdüsen heizbar</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>19101</ns1:DatEquipmentId>
                              <ns1:Description>Scheibenwischer mit Regensensor</ns1:Description>
                              <ns1:EquipmentGroup>SWRE</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>19000</ns1:DatEquipmentId>
                              <ns1:Description>Scheinwerfer-Reinigungsanlage (SRA)</ns1:Description>
                              <ns1:EquipmentGroup>SWRA</ns1:EquipmentGroup>
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
                              <ns1:DatEquipmentId>25151</ns1:DatEquipmentId>
                              <ns1:Description>Service-System: Intelligenter Notruf inkl. TeleServices</ns1:Description>
                              <ns1:EquipmentGroup>FA10</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>69811</ns1:DatEquipmentId>
                              <ns1:Description>Servolenkung Servotronic</ns1:Description>
                              <ns1:EquipmentGroup>SL</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>32811</ns1:DatEquipmentId>
                              <ns1:Description>Sitze vorn teilelektr. verstellbar</ns1:Description>
                              <ns1:EquipmentGroup>SITE</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>35408</ns1:DatEquipmentId>
                              <ns1:Description>Soft-Close-Automatik für Kofferraum / Heckklappe</ns1:Description>
                              <ns1:EquipmentGroup>HKEL</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>35513</ns1:DatEquipmentId>
                              <ns1:Description>Start-Stop-Knopf</ns1:Description>
                              <ns1:EquipmentGroup>MSSA</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>77601</ns1:DatEquipmentId>
                              <ns1:Description>Start/Stop-Anlage (Funktion)</ns1:Description>
                              <ns1:EquipmentGroup>MSSA</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>39016</ns1:DatEquipmentId>
                              <ns1:Description>Steckdose (12V-Anschluß) 3-fach</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>73017</ns1:DatEquipmentId>
                              <ns1:Description>Vlies-Batterie 80 Ah (AGM)</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>38105</ns1:DatEquipmentId>
                              <ns1:Description>Wegfahrsperre</ns1:Description>
                              <ns1:EquipmentGroup>WFS</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>22218</ns1:DatEquipmentId>
                              <ns1:Description>Wärme-/Sonnenschutzverglasung kombiniert (hinten abgedunkelt)</ns1:Description>
                              <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
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
                              <ns1:DatEquipmentId>96508</ns1:DatEquipmentId>
                              <ns1:Description>Motor 2,0 Ltr. - 135 kW Turbodiesel</ns1:Description>
                              <ns1:EquipmentType>engine</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>18913</ns1:DatEquipmentId>
                              <ns1:Description>Tagfahrlicht LED</ns1:Description>
                              <ns1:EquipmentGroup>TFAL</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>18940</ns1:DatEquipmentId>
                              <ns1:Description>Blinkleuchten LED</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                        </ns1:SeriesEquipment>
                        <ns1:SpecialEquipment>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>37603</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Ambiente-Beleuchtung</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25804</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Audio-Navigationssystem Professional</ns1:Description>
                              <ns1:EquipmentGroup>GPS</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>24709</ns1:DatEquipmentId>
                                    <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                    <ns1:Description>Sprachbediensystem</ns1:Description>
                                    <ns1:EquipmentGroup>TEL4</ns1:EquipmentGroup>
                                    <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>8702</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Außenausstattung: Shadow-Line Hochglanz</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25930</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Control-Display mit Farbmonitor (9,2 Zoll)</ns1:Description>
                              <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27810</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Dachhimmel Anthrazit (BMW Individual)</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>16198</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Dachreling Hochglanz Shadow-Line</ns1:Description>
                              <ns1:EquipmentGroup>DARE</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25704</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Fahrassistenz-System: Speed-Limit-Anzeige</ns1:Description>
                              <ns1:EquipmentGroup>FA28</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>22505</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Frontscheibe (Ausführung: Klimakomfort)</ns1:Description>
                              <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>75914</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Getriebe Automatik - mit Steptronic (8-Stufen)</ns1:Description>
                              <ns1:EquipmentGroup>AG2</ns1:EquipmentGroup>
                              <ns1:GearBoxType>automatic</ns1:GearBoxType>
                              <ns1:NrOfGears>8</ns1:NrOfGears>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25204</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Head-up-Display</ns1:Description>
                              <ns1:EquipmentGroup>HUD</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>25930</ns1:DatEquipmentId>
                                    <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                    <ns1:Description>Control-Display mit Farbmonitor (9,2 Zoll)</ns1:Description>
                                    <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                                    <ns1:EquipmentType>glass</ns1:EquipmentType>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>25413</ns1:DatEquipmentId>
                                    <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                    <ns1:Description>Instrumentenkombination (erweiterter Umfang)</ns1:Description>
                                    <ns1:EquipmentType>glass</ns1:EquipmentType>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>24607</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>HiFi-Lautsprechersystem</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>31408</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Innenausstattung: Interieurleisten Aluminium Längsschliff fein</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>37901</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Innenspiegel mit Abblendautomatik</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25413</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Instrumentenkombination (erweiterter Umfang)</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>25930</ns1:DatEquipmentId>
                                    <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                    <ns1:Description>Control-Display mit Farbmonitor (9,2 Zoll)</ns1:Description>
                                    <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                                    <ns1:EquipmentType>glass</ns1:EquipmentType>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>28982</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Klimaautomatik 2-Zonen mit autom. Umluft-Control, erweiterter Umfang</ns1:Description>
                              <ns1:EquipmentGroup>KLI2</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>33403</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Lendenwirbelstütze Sitz vorn links und rechts, elektr. verstellbar</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>77240</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Modellvariante CO2-Umfang (Code 1CB)</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>18313</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Nebelscheinwerfer LED</ns1:Description>
                              <ns1:EquipmentGroup>BEL</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>16302</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Panoramadach (Glas)</ns1:Description>
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
                              <ns1:Description>Sitzbezug / Polsterung: Leder Dakota</ns1:Description>
                              <ns1:EquipmentGroup>LEDE</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>29500</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Sitzheizung vorn</ns1:Description>
                              <ns1:EquipmentGroup>SITB</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>22102</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Sonnenschutzverglasung (hinten abgedunkelt, BMW Individual)</ns1:Description>
                              <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>24709</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Sprachbediensystem</ns1:Description>
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
                           <ns1:Description>Motor 2,0 Ltr. - 135 kW Turbodiesel</ns1:Description>
                           <ns1:EquipmentClass>1</ns1:EquipmentClass>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                           <ns1:Description>Karosserie: 5-türig</ns1:Description>
                           <ns1:EquipmentClass>2</ns1:EquipmentClass>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>75914</ns1:DatEquipmentId>
                           <ns1:Description>Getriebe Automatik - mit Steptronic (8-Stufen)</ns1:Description>
                           <ns1:EquipmentClass>11</ns1:EquipmentClass>
                        </ns1:EquipmentPosition>
                     </ns1:DATECodeEquipment>
                  </ns1:Vehicle>
                  <ns1:RepairParameters>
                     <ns1:PhantomCalculation>false</ns1:PhantomCalculation>
                     <ns1:LacquerType>Metallic (2-Schicht)</ns1:LacquerType>
                     <ns1:LacquerTypeLayers>2</ns1:LacquerTypeLayers>
                     <ns1:TimeUnitsOfManufacturer>false</ns1:TimeUnitsOfManufacturer>
                     <ns1:DMSCalculation>false</ns1:DMSCalculation>
                  </ns1:RepairParameters>
                  <ns1:ProcedureRelatedParameters>
                     <ns1:ProcedureRelatedParameter attribute="referenceSetName" factor="CalculationFactor" type="String">Standard D</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="biwOptimizationMode" factor="CalculationFactor" type="BiwOptimizationMode">AUTOMATIC</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="selectedLacquerMethod" factor="CalculationFactor" type="LacquerMethod">MANUFACTURER_SPECIFIC</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="crossSeries" factor="CalculationFactor" type="CrossSeriesState">NO</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="withoutValuesOfAdditionallyRequiredPositions" factor="CalculationFactor" type="Boolean">false</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnit" factor="CalculationFactor" type="TimeUnitSystem">HOUR</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="CalculationFactor" type="Integer">1</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="dataCurrency" factor="CalculationFactor" type="String">EUR</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="increaseDecrease" factor="SparePartFactor" type="Double">10.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="surchargeInProtocolOly" factor="SparePartFactor" type="Boolean">true</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="smallSparePartCalculationModel" factor="SparePartFactor" type="SmallPartsCalculationModel">PERCENT_OF_PARTS</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="priceSource" factor="SparePartFactor" type="PriceSource">DAT</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="smallSparePartPercentOfPart" factor="SparePartFactor" type="Double">2.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="dentWage" factor="LabourCostFactor" mode="PER_HOUR" type="Price">78.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="mechanicWage1" factor="LabourCostFactor" mode="PER_HOUR" type="Price">105.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="electricWage1" factor="LabourCostFactor" mode="PER_HOUR" type="Price">105.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnit" factor="LabourCostFactor" type="TimeUnitSystem">HOUR</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="LabourCostFactor" type="Integer">1</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="bodyWage1" factor="LabourCostFactor" mode="PER_HOUR" type="Price">105.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="materialMode" factor="EuroLacquerFactor" type="LacquerMaterialMode">LACQUER_METHOD</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="type" description="Metallic (2-Schicht)" factor="EuroLacquerFactor" type="String">12</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wage" factor="EuroLacquerFactor" mode="PER_HOUR" type="Price">100.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="materialIndex" factor="EuroLacquerFactor" type="Double">100.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="typeSaved" factor="EuroLacquerFactor" type="Boolean">false</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wageMode" factor="EuroLacquerFactor" type="LacquerWageMode">PER_TIME</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wageInclMaterialMode" factor="EuroLacquerFactor" type="LacquerWageMode">PER_TIME</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="calculationType" factor="EuroLacquerFactor" type="LacquerCalculationMode">WAGE_MATERIAL_SEPARATELY</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="disposalCostPercent" factor="EuroLacquerFactor" type="Double">0.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnit" factor="EuroLacquerFactor" type="TimeUnitSystem">HOUR</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="EuroLacquerFactor" type="Integer">1</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="materialMode" factor="ManufacturerLacquerFactor" type="LacquerMaterialMode">PERCENT</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="type" description="Metallic (2-Schicht)" factor="ManufacturerLacquerFactor" type="String">12</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="materialFlatRatePercent" factor="ManufacturerLacquerFactor" type="Double">25.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wage" factor="ManufacturerLacquerFactor" mode="PER_HOUR" type="Price">120.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="typeSaved" factor="ManufacturerLacquerFactor" type="Boolean">false</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wageMode" factor="ManufacturerLacquerFactor" type="LacquerWageMode">PER_TIME</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wageInclMaterialMode" factor="ManufacturerLacquerFactor" type="LacquerWageMode">PER_TIME</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="calculationType" factor="ManufacturerLacquerFactor" type="LacquerCalculationMode">WAGE_MATERIAL_SEPARATELY</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnit" factor="ManufacturerLacquerFactor" type="TimeUnitSystem">HOUR</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="ManufacturerLacquerFactor" type="Integer">1</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="fourLayerLacquerMode" factor="AztLacquerFactor" type="AztLacquerMode">WET_IN_WET</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="materialMode" factor="AztLacquerFactor" type="LacquerMaterialMode">LACQUER_METHOD</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="materialIndex" factor="AztLacquerFactor" type="Double">100.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="aztDataset" factor="AztLacquerFactor" type="Integer">1</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="typeSaved" factor="AztLacquerFactor" type="Boolean">false</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wageMode" factor="AztLacquerFactor" type="LacquerWageMode">PER_TIME</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wageInclMaterialMode" factor="AztLacquerFactor" type="LacquerWageMode">PER_TIME</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="calculationType" factor="AztLacquerFactor" type="LacquerCalculationMode">WAGE_MATERIAL_SEPARATELY</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="disposalCostPercent" factor="AztLacquerFactor" type="Double">0.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnit" factor="AztLacquerFactor" type="TimeUnitSystem">HOUR</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="isSurchargeForWaterBased" factor="AztLacquerFactor" type="Boolean">false</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="threeLayerLacquerMode" factor="AztLacquerFactor" type="AztLacquerMode">WET_IN_WET</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="AztLacquerFactor" type="Integer">1</ns1:ProcedureRelatedParameter>
                  </ns1:ProcedureRelatedParameters>
                  <ns1:RepairPositions>
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>43712</ns1:DATProcessId>
                        <ns1:RepairType>replace</ns1:RepairType>
                        <ns1:Description>Seitenwand grundiert</ns1:Description>
                        <ns1:DescriptionId>36419456</ns1:DescriptionId>
                        <ns1:IsManualDescription>false</ns1:IsManualDescription>
                        <ns1:ConstructionGroupId>1</ns1:ConstructionGroupId>
                        <ns1:ConstructionGroup>VORDERWAGEN AUSSEN</ns1:ConstructionGroup>
                        <ns1:ConstructionGroupPolygon>63</ns1:ConstructionGroupPolygon>
                        <ns1:PositionEntryType>graphical</ns1:PositionEntryType>
                        <ns1:IsRepairExtension>false</ns1:IsRepairExtension>
                        <ns1:PreDamage>false</ns1:PreDamage>
                     </ns1:RepairPosition>
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>44910</ns1:DATProcessId>
                        <ns1:RepairType>replace</ns1:RepairType>
                        <ns1:Description>Frontscheibe</ns1:Description>
                        <ns1:DescriptionId>128880</ns1:DescriptionId>
                        <ns1:IsManualDescription>false</ns1:IsManualDescription>
                        <ns1:ConstructionGroupId>1</ns1:ConstructionGroupId>
                        <ns1:ConstructionGroup>VORDERWAGEN AUSSEN</ns1:ConstructionGroup>
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
                           <ns1:DATProcessId>43712</ns1:DATProcessId>
                           <ns1:PartNumber>41355A03262</ns1:PartNumber>
                           <ns1:DATPartNumber>41355A03262</ns1:DATPartNumber>
                           <ns1:Description>SEITENWAND V.R.</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>408.34</ns1:ValuePerUnit>
                           <ns1:ValueTotal>408.34</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>408.34</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:SparePartHistoryPositions>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>41357248660</ns1:PartNumber>
                                 <ns1:LastUPE>349.55</ns1:LastUPE>
                                 <ns1:LastUPEDate>2022-05-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                           </ns1:SparePartHistoryPositions>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>44910</ns1:DATProcessId>
                           <ns1:PartNumber>51317333835</ns1:PartNumber>
                           <ns1:DATPartNumber>51317333835</ns1:DATPartNumber>
                           <ns1:Description>FRONTSCHEIBE</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>877.6</ns1:ValuePerUnit>
                           <ns1:ValueTotal>877.6</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>877.6</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:SparePartHistoryPositions>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51314899567</ns1:PartNumber>
                                 <ns1:LastUPE>593.19</ns1:LastUPE>
                                 <ns1:LastUPEDate>2014-02-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51317280748</ns1:PartNumber>
                                 <ns1:LastUPE>593.19</ns1:LastUPE>
                                 <ns1:LastUPEDate>2014-02-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51317280748</ns1:PartNumber>
                                 <ns1:LastUPE>593.19</ns1:LastUPE>
                                 <ns1:LastUPEDate>2012-11-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                           </ns1:SparePartHistoryPositions>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>40270</ns1:DATProcessId>
                           <ns1:PartNumber>51489162739</ns1:PartNumber>
                           <ns1:DATPartNumber>51489162739</ns1:DATPartNumber>
                           <ns1:Description>SCHALLISOLIERUNG FRONTSCHEIBE WINDLAUF</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>54.27</ns1:ValuePerUnit>
                           <ns1:ValueTotal>54.27</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>54.27</ns1:ValueTotalCorrected>
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
                           <ns1:Description>ABDECKUNG FRONTSCHEIBE O.</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>26.06</ns1:ValuePerUnit>
                           <ns1:ValueTotal>26.06</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>26.06</ns1:ValueTotalCorrected>
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
                           <ns1:Description>REP.-SATZ EINGLASUNG FRONTSCHEIBE</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>66.18</ns1:ValuePerUnit>
                           <ns1:ValueTotal>66.18</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>66.18</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:SparePartHistoryPositions>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51311958028</ns1:PartNumber>
                                 <ns1:LastUPE>32.69</ns1:LastUPE>
                                 <ns1:LastUPEDate>2016-04-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83199407850</ns1:PartNumber>
                                 <ns1:LastUPE>51.26</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>81220142749</ns1:PartNumber>
                                 <ns1:LastUPE>51.26</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>81229407497</ns1:PartNumber>
                                 <ns1:LastUPE>51.26</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147369</ns1:PartNumber>
                                 <ns1:LastUPE>42.44</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147370</ns1:PartNumber>
                                 <ns1:LastUPE>73.11</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147371</ns1:PartNumber>
                                 <ns1:LastUPE>42.44</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147372</ns1:PartNumber>
                                 <ns1:LastUPE>73.11</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190392461</ns1:PartNumber>
                                 <ns1:LastUPE>184.03</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190393939</ns1:PartNumber>
                                 <ns1:LastUPE>41.18</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190393940</ns1:PartNumber>
                                 <ns1:LastUPE>17.65</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190444141</ns1:PartNumber>
                                 <ns1:LastUPE>47.9</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-06-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51318109154</ns1:PartNumber>
                                 <ns1:LastUPE>81.59</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83199407714</ns1:PartNumber>
                                 <ns1:LastUPE>70.59</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>81220142749</ns1:PartNumber>
                                 <ns1:LastUPE>51.26</ns1:LastUPE>
                                 <ns1:LastUPEDate>2014-02-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>81229407497</ns1:PartNumber>
                                 <ns1:LastUPE>51.26</ns1:LastUPE>
                                 <ns1:LastUPEDate>2014-02-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147369</ns1:PartNumber>
                                 <ns1:LastUPE>42.44</ns1:LastUPE>
                                 <ns1:LastUPEDate>2009-05-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147370</ns1:PartNumber>
                                 <ns1:LastUPE>73.11</ns1:LastUPE>
                                 <ns1:LastUPEDate>2010-03-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147371</ns1:PartNumber>
                                 <ns1:LastUPE>42.44</ns1:LastUPE>
                                 <ns1:LastUPEDate>2014-02-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147372</ns1:PartNumber>
                                 <ns1:LastUPE>73.11</ns1:LastUPE>
                                 <ns1:LastUPEDate>2014-02-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                           </ns1:SparePartHistoryPositions>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:PartNumber>51317288462</ns1:PartNumber>
                           <ns1:DATPartNumber>51317288462</ns1:DATPartNumber>
                           <ns1:Description>PUFFER</ns1:Description>
                           <ns1:Amount>11</ns1:Amount>
                           <ns1:ValuePerUnit>1.95</ns1:ValuePerUnit>
                           <ns1:ValueTotal>21.45</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>21.45</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:SparePartHistoryPositions>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51314875651</ns1:PartNumber>
                                 <ns1:LastUPE>1.49</ns1:LastUPE>
                                 <ns1:LastUPEDate>2011-05-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                           </ns1:SparePartHistoryPositions>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:PartNumber>83192211217</ns1:PartNumber>
                           <ns1:DATPartNumber>83192211217</ns1:DATPartNumber>
                           <ns1:Description>REINIGER (100 ML.)</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>11.55</ns1:ValuePerUnit>
                           <ns1:ValueTotal>11.55</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>11.55</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:SparePartHistoryPositions>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83192157286</ns1:PartNumber>
                                 <ns1:LastUPE>9.05</ns1:LastUPE>
                                 <ns1:LastUPEDate>2011-07-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                           </ns1:SparePartHistoryPositions>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:PartNumber>51317288462</ns1:PartNumber>
                           <ns1:DATPartNumber>51317288462</ns1:DATPartNumber>
                           <ns1:Description>PUFFER</ns1:Description>
                           <ns1:Amount>6</ns1:Amount>
                           <ns1:ValuePerUnit>1.95</ns1:ValuePerUnit>
                           <ns1:ValueTotal>11.7</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>11.7</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:SparePartHistoryPositions>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51314875651</ns1:PartNumber>
                                 <ns1:LastUPE>1.49</ns1:LastUPE>
                                 <ns1:LastUPEDate>2011-05-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                           </ns1:SparePartHistoryPositions>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                     </ns1:MaterialPositions>
                     <ns1:ExtensionPositions>
                        <ns1:ExtensionPosition>
                           <ns1:DATProcessId>45335</ns1:DATProcessId>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:Description>SILIKONFOLIE REGEN-/LICHTSENSOR</ns1:Description>
                           <ns1:PartsSum>27.62</ns1:PartsSum>
                        </ns1:ExtensionPosition>
                     </ns1:ExtensionPositions>
                     <ns1:LabourPositions>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>43712</ns1:DATProcessId>
                           <ns1:LabourPositionKind>1</ns1:LabourPositionKind>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:LabourPosId>41 35 555</ns1:LabourPosId>
                           <ns1:Description>SEITENWAND V.R. ERS.</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>1.58</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>165.9</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>165.9</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>41 35 555</ns1:WorkNumber>
                           <ns1:SparePartNumber>41355A03262</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>43712</ns1:DATProcessId>
                           <ns1:LabourPositionKind>4</ns1:LabourPositionKind>
                           <ns1:RepairType>body cavity protection</ns1:RepairType>
                           <ns1:LabourPosId>97 35 511</ns1:LabourPosId>
                           <ns1:Description>HOHLRAUMKONSERVIERUNG SEITENWAND V.R.</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>0.42</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>44.1</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>44.1</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>true</ns1:hasRequiredByPosition>
                           <ns1:RequiredByPosition>
                              <ns1:DATProcessId>43712</ns1:DATProcessId>
                              <ns1:RepairType>replace</ns1:RepairType>
                           </ns1:RequiredByPosition>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>97 35 511</ns1:WorkNumber>
                           <ns1:SparePartNumber>41355A03262</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>44910</ns1:DATProcessId>
                           <ns1:LabourPositionKind>1</ns1:LabourPositionKind>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:LabourPosId>51 31 513</ns1:LabourPosId>
                           <ns1:Description>FRONTSCHEIBE A+E/ERS.</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>2.58</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>270.9</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>270.9</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>51 31 513</ns1:WorkNumber>
                           <ns1:SparePartNumber>51317333835</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>14449</ns1:DATProcessId>
                           <ns1:LabourPositionKind>4</ns1:LabourPositionKind>
                           <ns1:RepairType>adjust</ns1:RepairType>
                           <ns1:LabourPosId>66 51 525</ns1:LabourPosId>
                           <ns1:Description>KAMERA FAHRASSISTENZ-SYSTEME KALIBRIEREN</ns1:Description>
                           <ns1:WageType>electric</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>0.33</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>34.65</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>34.65</ns1:ValueTotalCorrected>
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
                        <ns1:LabourPosition>
                           <ns1:LabourPositionKind>8</ns1:LabourPositionKind>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:LabourPosId>ARBEITSAUFWAND</ns1:LabourPosId>
                           <ns1:Description>ERGAENZUNG HAUPTARBEIT</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>0.17</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>17.85</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>17.85</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>DAT#</ns1:WorkNumber>
                        </ns1:LabourPosition>
                     </ns1:LabourPositions>
                     <ns1:LacquerPositions>
                        <ns1:LacquerPosition>
                           <ns1:DATProcessId>43712</ns1:DATProcessId>
                           <ns1:LabourPosId>99 35 011</ns1:LabourPosId>
                           <ns1:Description>SEITENWAND V.R. UMFASST: VORBEREITUNGSARBEITEN</ns1:Description>
                           <ns1:Level>4</ns1:Level>
                           <ns1:LevelDescription>new</ns1:LevelDescription>
                           <ns1:LevelManufacturer>ST.2</ns1:LevelManufacturer>
                           <ns1:Duration>2.42</ns1:Duration>
                           <ns1:ManualDuration>false</ns1:ManualDuration>
                           <ns1:Material>72.6</ns1:Material>
                           <ns1:ValueTotal>363</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>363</ns1:ValueTotalCorrected>
                           <ns1:WageLevel1>290.4</ns1:WageLevel1>
                           <ns1:WorkNumber>99 35 011</ns1:WorkNumber>
                           <ns1:LacquerPositionTimeState/>
                           <ns1:LacquerPositionMaterialState/>
                           <ns1:LacquerPositionPriceState/>
                           <ns1:MaterialType>2</ns1:MaterialType>
                           <ns1:SparePartNumber>41355A03262</ns1:SparePartNumber>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                        </ns1:LacquerPosition>
                     </ns1:LacquerPositions>
                     <ns1:PriceDate>2023-12-01+01:00</ns1:PriceDate>
                     <ns1:RepairCalculationSummary>
                        <ns1:SparePartsCosts>
                           <ns1:AllSum>1477.15</ns1:AllSum>
                           <ns1:ConsumablesSurcharge>29.54</ns1:ConsumablesSurcharge>
                           <ns1:ConsumablesSurchargePercentage>2</ns1:ConsumablesSurchargePercentage>
                           <ns1:TotalSum>1506.69</ns1:TotalSum>
                        </ns1:SparePartsCosts>
                        <ns1:AuxiliaryCosts/>
                        <ns1:LabourCosts>
                           <ns1:AllSum>533.4</ns1:AllSum>
                           <ns1:Bodywork>
                              <ns1:Type>CAR BODY</ns1:Type>
                              <ns1:Units>4.75</ns1:Units>
                              <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                              <ns1:Price>498.75</ns1:Price>
                           </ns1:Bodywork>
                           <ns1:Electric>
                              <ns1:Type>ELECTRICS</ns1:Type>
                              <ns1:Units>0.33</ns1:Units>
                              <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                              <ns1:Price>34.65</ns1:Price>
                           </ns1:Electric>
                           <ns1:Mechanic>
                              <ns1:Type>MECHANICS</ns1:Type>
                              <ns1:Units>0</ns1:Units>
                              <ns1:Price>0</ns1:Price>
                           </ns1:Mechanic>
                           <ns1:TotalSum>533.4</ns1:TotalSum>
                           <ns1:Wages/>
                           <ns1:Works>
                              <ns1:Work>
                                 <ns1:Type>CAR BODY</ns1:Type>
                                 <ns1:WageLevel>1</ns1:WageLevel>
                                 <ns1:Units>4.75</ns1:Units>
                                 <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                                 <ns1:Price>498.75</ns1:Price>
                              </ns1:Work>
                              <ns1:Work>
                                 <ns1:Type>ELECTRICS</ns1:Type>
                                 <ns1:WageLevel>1</ns1:WageLevel>
                                 <ns1:Units>0.33</ns1:Units>
                                 <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                                 <ns1:Price>34.65</ns1:Price>
                              </ns1:Work>
                           </ns1:Works>
                        </ns1:LabourCosts>
                        <ns1:LacquerCosts>
                           <ns1:Wage>
                              <ns1:Type>LACQUER WORK</ns1:Type>
                              <ns1:Units>2.42</ns1:Units>
                              <ns1:PricePerUnit>120.00</ns1:PricePerUnit>
                              <ns1:Price>290.40</ns1:Price>
                           </ns1:Wage>
                           <ns1:TotalWages>290.40</ns1:TotalWages>
                           <ns1:Material>
                              <ns1:FlatPercentage>25</ns1:FlatPercentage>
                              <ns1:FlatAmount>72.6</ns1:FlatAmount>
                              <ns1:MaterialGroups/>
                              <ns1:TotalSum>72.6</ns1:TotalSum>
                              <ns1:SumMaterialCorrected>72.6</ns1:SumMaterialCorrected>
                           </ns1:Material>
                           <ns1:TotalSum>363</ns1:TotalSum>
                        </ns1:LacquerCosts>
                        <ns1:TotalNetCosts>2403.09</ns1:TotalNetCosts>
                        <ns1:TotalVAT>456.59</ns1:TotalVAT>
                        <ns1:TotalGrossCosts>2859.68</ns1:TotalGrossCosts>
                        <ns1:TotalNetCorrected>2403.09</ns1:TotalNetCorrected>
                        <ns1:TotalVATCorrected>456.59</ns1:TotalVATCorrected>
                        <ns1:TotalGrossCorrected>2859.68</ns1:TotalGrossCorrected>
                        <ns1:SumNet>2403.09</ns1:SumNet>
                        <ns1:SumGross>2859.68</ns1:SumGross>
                        <ns1:SumSparePartCosts>1477.15</ns1:SumSparePartCosts>
                        <ns1:SumSmallSparePartCosts>29.54</ns1:SumSmallSparePartCosts>
                        <ns1:SumLabourCosts>533.4</ns1:SumLabourCosts>
                        <ns1:MetaPositions>
                           <ns1:MetaPosition key="TOTAL_NET_RISK" value="27.08"/>
                           <ns1:MetaPosition key="VAT_RISK" value="5.15"/>
                           <ns1:MetaPosition key="TOTAL_GROSS_RISK" value="32.23"/>
                           <ns1:MetaPosition key="TIME_UNIT_SYSTEM" value="STD"/>
                           <ns1:MetaPosition key="LACQUER_TIME_UNIT_SYSTEM" value="STD"/>
                           <ns1:MetaPosition key="DAT_EUROLACQUER_IN_HOURS" value="false"/>
                           <ns1:MetaPosition key="TOTAL_PRICE_SPARE_PARTS_RISK" value="27.08"/>
                           <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EQUIPMENT" value="false"/>
                           <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EXTENSION" value="false"/>
                           <ns1:MetaPosition key="FLAT_PERCENTAGE_BASE" value="290.4"/>
                        </ns1:MetaPositions>
                     </ns1:RepairCalculationSummary>
                     <ns1:CalcProtocol>
                        <ns1:ProtocolHints>
                           <ns1:ProtocolHint>
                              <ns1:Identifier>H001</ns1:Identifier>
                              <ns1:Description>Serientreue Kalkulation</ns1:Description>
                           </ns1:ProtocolHint>
                        </ns1:ProtocolHints>
                        <ns1:ProtocolData>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AXIIWoQBcghahAFyKLIyoCO1rAzoSHtWhteOkCcMUEg9KwMUUmJlgELKrAxQSJAnDFDoG1YGKPQiDwxQ6C0rw4gIPoURVr1nZYQJH1gZYcLDujDChId1YYQJD+vCCBNeTgdGnNHLiwtGvL6xYWWH3bfSHkzSsW+f+xbapkvyEf/7Wp/f83PU6HhI93Utk0PmkcyH52SY5qwja7kuzypTftVf0JgtKAplbmRzdHJlYW0KZW5kb2JqCjMgMCBvYmoKPDwvU3VidHlwZS9UeXBlMC9UeXBlL0ZvbnQvQmFzZUZvbnQvVE9CVElWK0RlamFWdVNhbnMtQm9sZC9FbmNvZGluZy9JZGVudGl0eS1IL0Rlc2NlbmRhbnRGb250c1syMCAwIFJdL1RvVW5pY29kZSAyMSAwIFI+PgplbmRvYmoKNCAwIG9iago8PC9TdWJ0eXBlL1R5cGUxL1R5cGUvRm9udC9CYXNlRm9udC9IZWx2ZXRpY2EvRW5jb2RpbmcvV2luQW5zaUVuY29kaW5nPj4KZW5kb2JqCjYgMCBvYmoKPDwvS2lkc1s3IDAgUiA5IDAgUl0vVHlwZS9QYWdlcy9Db3VudCAyL0lUWFQoNC4yLjApPj4KZW5kb2JqCjIyIDAgb2JqCjw8L1R5cGUvQ2F0YWxvZy9QYWdlcyA2IDAgUj4+CmVuZG9iagoyMyAwIG9iago8PC9Nb2REYXRlKEQ6MjAyMzEyMjIxMjA0NTkrMDEnMDAnKS9DcmVhdGlvbkRhdGUoRDoyMDIzMTIyMjEyMDQ1OSswMScwMCcpL1Byb2R1Y2VyKGlUZXh0IDQuMi4wIGJ5IDFUM1hUKT4+CmVuZG9iagp4cmVmCjAgMjQKMDAwMDAwMDAwMCA2NTUzNSBmIAowMDAwMDI4NjI4IDAwMDAwIG4gCjAwMDAwMzY4NDUgMDAwMDAgbiAKMDAwMDA1NTk4NCAwMDAwMCBuIAowMDAwMDU2MTIxIDAwMDAwIG4gCjAwMDAwMDAwMTUgMDAwMDAgbiAKMDAwMDA1NjIwOSAwMDAwMCBuIAowMDAwMDA0NTU0IDAwMDAwIG4gCjAwMDAwMDQ3MzggMDAwMDAgbiAKMDAwMDAwNjIxOCAwMDAwMCBuIAowMDAwMDA2NDAyIDAwMDAwIG4gCjAwMDAwMjcyMzkgMDAwMDAgbiAKMDAwMDAyNzQyNSAwMDAwMCBuIAowMDAwMDI3OTYzIDAwMDAwIG4gCjAwMDAwMjg3NjAgMDAwMDAgbiAKMDAwMDAzNjEyOCAwMDAwMCBuIAowMDAwMDM2MzEwIDAwMDAwIG4gCjAwMDAwMzY1MzYgMDAwMDAgbiAKMDAwMDAzNjk3NCAwMDAwMCBuIAowMDAwMDU0NzgyIDAwMDAwIG4gCjAwMDAwNTQ5NzcgMDAwMDAgbiAKMDAwMDA1NTQyOSAwMDAwMCBuIAowMDAwMDU2Mjc4IDAwMDAwIG4gCjAwMDAwNTYzMjQgMDAwMDAgbiAKdHJhaWxlcgo8PC9JbmZvIDIzIDAgUi9JRCBbPGMzYzUyOTgwZGJhMWRlMmVhYjZkMzAwMDI2YjhlZGE3Pjw3MDM2OGY1MjI0MjA3NGEwNjUzMDc5NWZmZmVmNTc4YT5dL1Jvb3QgMjIgMCBSL1NpemUgMjQ+PgpzdGFydHhyZWYKNTY0NDcKJSVFT0YK</ns1:ProtocolData>
                     </ns1:CalcProtocol>
                  </ns1:CalcResultCommon>
                  <ns1:CalcResultExtension>
                     <ns1:MaterialPositions>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>43712</ns1:DATProcessId>
                           <ns1:PartNumber>41355A03262</ns1:PartNumber>
                           <ns1:DATPartNumber>41355A03262</ns1:DATPartNumber>
                           <ns1:Description>SEITENWAND V.R.</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>408.34</ns1:ValuePerUnit>
                           <ns1:ValueTotal>408.34</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>408.34</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:SparePartHistoryPositions>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>41357248660</ns1:PartNumber>
                                 <ns1:LastUPE>349.55</ns1:LastUPE>
                                 <ns1:LastUPEDate>2022-05-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                           </ns1:SparePartHistoryPositions>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>44910</ns1:DATProcessId>
                           <ns1:PartNumber>51317333835</ns1:PartNumber>
                           <ns1:DATPartNumber>51317333835</ns1:DATPartNumber>
                           <ns1:Description>FRONTSCHEIBE</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>877.6</ns1:ValuePerUnit>
                           <ns1:ValueTotal>877.6</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>877.6</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:SparePartHistoryPositions>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51314899567</ns1:PartNumber>
                                 <ns1:LastUPE>593.19</ns1:LastUPE>
                                 <ns1:LastUPEDate>2014-02-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51317280748</ns1:PartNumber>
                                 <ns1:LastUPE>593.19</ns1:LastUPE>
                                 <ns1:LastUPEDate>2014-02-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51317280748</ns1:PartNumber>
                                 <ns1:LastUPE>593.19</ns1:LastUPE>
                                 <ns1:LastUPEDate>2012-11-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                           </ns1:SparePartHistoryPositions>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>40270</ns1:DATProcessId>
                           <ns1:PartNumber>51489162739</ns1:PartNumber>
                           <ns1:DATPartNumber>51489162739</ns1:DATPartNumber>
                           <ns1:Description>SCHALLISOLIERUNG FRONTSCHEIBE WINDLAUF</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>54.27</ns1:ValuePerUnit>
                           <ns1:ValueTotal>54.27</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>54.27</ns1:ValueTotalCorrected>
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
                           <ns1:Description>ABDECKUNG FRONTSCHEIBE O.</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>26.06</ns1:ValuePerUnit>
                           <ns1:ValueTotal>26.06</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>26.06</ns1:ValueTotalCorrected>
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
                           <ns1:Description>REP.-SATZ EINGLASUNG FRONTSCHEIBE</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>66.18</ns1:ValuePerUnit>
                           <ns1:ValueTotal>66.18</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>66.18</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:SparePartHistoryPositions>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51311958028</ns1:PartNumber>
                                 <ns1:LastUPE>32.69</ns1:LastUPE>
                                 <ns1:LastUPEDate>2016-04-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83199407850</ns1:PartNumber>
                                 <ns1:LastUPE>51.26</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>81220142749</ns1:PartNumber>
                                 <ns1:LastUPE>51.26</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>81229407497</ns1:PartNumber>
                                 <ns1:LastUPE>51.26</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147369</ns1:PartNumber>
                                 <ns1:LastUPE>42.44</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147370</ns1:PartNumber>
                                 <ns1:LastUPE>73.11</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147371</ns1:PartNumber>
                                 <ns1:LastUPE>42.44</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147372</ns1:PartNumber>
                                 <ns1:LastUPE>73.11</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190392461</ns1:PartNumber>
                                 <ns1:LastUPE>184.03</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190393939</ns1:PartNumber>
                                 <ns1:LastUPE>41.18</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190393940</ns1:PartNumber>
                                 <ns1:LastUPE>17.65</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190444141</ns1:PartNumber>
                                 <ns1:LastUPE>47.9</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-06-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51318109154</ns1:PartNumber>
                                 <ns1:LastUPE>81.59</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83199407714</ns1:PartNumber>
                                 <ns1:LastUPE>70.59</ns1:LastUPE>
                                 <ns1:LastUPEDate>2015-10-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>81220142749</ns1:PartNumber>
                                 <ns1:LastUPE>51.26</ns1:LastUPE>
                                 <ns1:LastUPEDate>2014-02-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>81229407497</ns1:PartNumber>
                                 <ns1:LastUPE>51.26</ns1:LastUPE>
                                 <ns1:LastUPEDate>2014-02-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147369</ns1:PartNumber>
                                 <ns1:LastUPE>42.44</ns1:LastUPE>
                                 <ns1:LastUPEDate>2009-05-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147370</ns1:PartNumber>
                                 <ns1:LastUPE>73.11</ns1:LastUPE>
                                 <ns1:LastUPEDate>2010-03-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147371</ns1:PartNumber>
                                 <ns1:LastUPE>42.44</ns1:LastUPE>
                                 <ns1:LastUPEDate>2014-02-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83190147372</ns1:PartNumber>
                                 <ns1:LastUPE>73.11</ns1:LastUPE>
                                 <ns1:LastUPEDate>2014-02-01+01:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                           </ns1:SparePartHistoryPositions>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>45335</ns1:DATProcessId>
                           <ns1:PartNumber>61359856157</ns1:PartNumber>
                           <ns1:DATPartNumber>61359856157</ns1:DATPartNumber>
                           <ns1:Description>SILIKONFOLIE REGEN-/LICHTSENSOR</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>27.08</ns1:ValuePerUnit>
                           <ns1:ValueTotal>27.08</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>27.08</ns1:ValueTotalCorrected>
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
                           <ns1:Description>PUFFER</ns1:Description>
                           <ns1:Amount>11</ns1:Amount>
                           <ns1:ValuePerUnit>1.95</ns1:ValuePerUnit>
                           <ns1:ValueTotal>21.45</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>21.45</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:SparePartHistoryPositions>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51314875651</ns1:PartNumber>
                                 <ns1:LastUPE>1.49</ns1:LastUPE>
                                 <ns1:LastUPEDate>2011-05-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                           </ns1:SparePartHistoryPositions>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:PartNumber>83192211217</ns1:PartNumber>
                           <ns1:DATPartNumber>83192211217</ns1:DATPartNumber>
                           <ns1:Description>REINIGER (100 ML.)</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>11.55</ns1:ValuePerUnit>
                           <ns1:ValueTotal>11.55</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>11.55</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:SparePartHistoryPositions>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>83192157286</ns1:PartNumber>
                                 <ns1:LastUPE>9.05</ns1:LastUPE>
                                 <ns1:LastUPEDate>2011-07-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                           </ns1:SparePartHistoryPositions>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:PartNumber>51317288462</ns1:PartNumber>
                           <ns1:DATPartNumber>51317288462</ns1:DATPartNumber>
                           <ns1:Description>PUFFER</ns1:Description>
                           <ns1:Amount>6</ns1:Amount>
                           <ns1:ValuePerUnit>1.95</ns1:ValuePerUnit>
                           <ns1:ValueTotal>11.7</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>11.7</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>44910</ns1:RequiredByProcessId>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:SparePartHistoryPositions>
                              <ns1:SparePartHistoryPosition>
                                 <ns1:PartNumber>51314875651</ns1:PartNumber>
                                 <ns1:LastUPE>1.49</ns1:LastUPE>
                                 <ns1:LastUPEDate>2011-05-01+02:00</ns1:LastUPEDate>
                              </ns1:SparePartHistoryPosition>
                           </ns1:SparePartHistoryPositions>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                     </ns1:MaterialPositions>
                     <ns1:LabourPositions>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>43712</ns1:DATProcessId>
                           <ns1:LabourPositionKind>1</ns1:LabourPositionKind>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:LabourPosId>41 35 555</ns1:LabourPosId>
                           <ns1:Description>SEITENWAND V.R. ERS.</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>1.58</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>165.9</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>165.9</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>41 35 555</ns1:WorkNumber>
                           <ns1:SparePartNumber>41355A03262</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>43712</ns1:DATProcessId>
                           <ns1:LabourPositionKind>4</ns1:LabourPositionKind>
                           <ns1:RepairType>body cavity protection</ns1:RepairType>
                           <ns1:LabourPosId>97 35 511</ns1:LabourPosId>
                           <ns1:Description>HOHLRAUMKONSERVIERUNG SEITENWAND V.R.</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>0.42</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>44.1</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>44.1</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>true</ns1:hasRequiredByPosition>
                           <ns1:RequiredByPosition>
                              <ns1:DATProcessId>43712</ns1:DATProcessId>
                              <ns1:RepairType>replace</ns1:RepairType>
                           </ns1:RequiredByPosition>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>97 35 511</ns1:WorkNumber>
                           <ns1:SparePartNumber>41355A03262</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>44910</ns1:DATProcessId>
                           <ns1:LabourPositionKind>1</ns1:LabourPositionKind>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:LabourPosId>51 31 513</ns1:LabourPosId>
                           <ns1:Description>FRONTSCHEIBE A+E/ERS.</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>2.58</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>270.9</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>270.9</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>51 31 513</ns1:WorkNumber>
                           <ns1:SparePartNumber>51317333835</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>14449</ns1:DATProcessId>
                           <ns1:LabourPositionKind>4</ns1:LabourPositionKind>
                           <ns1:RepairType>adjust</ns1:RepairType>
                           <ns1:LabourPosId>66 51 525</ns1:LabourPosId>
                           <ns1:Description>KAMERA FAHRASSISTENZ-SYSTEME KALIBRIEREN</ns1:Description>
                           <ns1:WageType>electric</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>0.33</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>34.65</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>34.65</ns1:ValueTotalCorrected>
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
                        <ns1:LabourPosition>
                           <ns1:LabourPositionKind>8</ns1:LabourPositionKind>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:LabourPosId>ARBEITSAUFWAND</ns1:LabourPosId>
                           <ns1:Description>ERGAENZUNG HAUPTARBEIT</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>0.17</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>17.85</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>17.85</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>DAT#</ns1:WorkNumber>
                        </ns1:LabourPosition>
                     </ns1:LabourPositions>
                     <ns1:LacquerPositions>
                        <ns1:LacquerPosition>
                           <ns1:DATProcessId>43712</ns1:DATProcessId>
                           <ns1:LabourPosId>99 35 011</ns1:LabourPosId>
                           <ns1:Description>SEITENWAND V.R. UMFASST: VORBEREITUNGSARBEITEN</ns1:Description>
                           <ns1:Level>4</ns1:Level>
                           <ns1:LevelDescription>new</ns1:LevelDescription>
                           <ns1:LevelManufacturer>ST.2</ns1:LevelManufacturer>
                           <ns1:Duration>2.42</ns1:Duration>
                           <ns1:ManualDuration>false</ns1:ManualDuration>
                           <ns1:Material>72.6</ns1:Material>
                           <ns1:ValueTotal>363</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>363</ns1:ValueTotalCorrected>
                           <ns1:WageLevel1>290.4</ns1:WageLevel1>
                           <ns1:WorkNumber>99 35 011</ns1:WorkNumber>
                           <ns1:LacquerPositionTimeState/>
                           <ns1:LacquerPositionMaterialState/>
                           <ns1:LacquerPositionPriceState/>
                           <ns1:MaterialType>2</ns1:MaterialType>
                           <ns1:SparePartNumber>41355A03262</ns1:SparePartNumber>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                        </ns1:LacquerPosition>
                     </ns1:LacquerPositions>
                     <ns1:PriceDate>2023-12-01+01:00</ns1:PriceDate>
                     <ns1:RepairCalculationSummary>
                        <ns1:SparePartsCosts>
                           <ns1:AllSum>1504.23</ns1:AllSum>
                           <ns1:ConsumablesSurcharge>30.08</ns1:ConsumablesSurcharge>
                           <ns1:ConsumablesSurchargePercentage>2</ns1:ConsumablesSurchargePercentage>
                           <ns1:TotalSum>1534.31</ns1:TotalSum>
                        </ns1:SparePartsCosts>
                        <ns1:AuxiliaryCosts/>
                        <ns1:LabourCosts>
                           <ns1:AllSum>533.4</ns1:AllSum>
                           <ns1:Bodywork>
                              <ns1:Type>CAR BODY</ns1:Type>
                              <ns1:Units>4.75</ns1:Units>
                              <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                              <ns1:Price>498.75</ns1:Price>
                           </ns1:Bodywork>
                           <ns1:Electric>
                              <ns1:Type>ELECTRICS</ns1:Type>
                              <ns1:Units>0.33</ns1:Units>
                              <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                              <ns1:Price>34.65</ns1:Price>
                           </ns1:Electric>
                           <ns1:Mechanic>
                              <ns1:Type>MECHANICS</ns1:Type>
                              <ns1:Units>0</ns1:Units>
                              <ns1:Price>0</ns1:Price>
                           </ns1:Mechanic>
                           <ns1:TotalSum>533.4</ns1:TotalSum>
                           <ns1:Wages/>
                           <ns1:Works>
                              <ns1:Work>
                                 <ns1:Type>CAR BODY</ns1:Type>
                                 <ns1:WageLevel>1</ns1:WageLevel>
                                 <ns1:Units>4.75</ns1:Units>
                                 <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                                 <ns1:Price>498.75</ns1:Price>
                              </ns1:Work>
                              <ns1:Work>
                                 <ns1:Type>ELECTRICS</ns1:Type>
                                 <ns1:WageLevel>1</ns1:WageLevel>
                                 <ns1:Units>0.33</ns1:Units>
                                 <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                                 <ns1:Price>34.65</ns1:Price>
                              </ns1:Work>
                           </ns1:Works>
                        </ns1:LabourCosts>
                        <ns1:LacquerCosts>
                           <ns1:Wage>
                              <ns1:Type>LACQUER WORK</ns1:Type>
                              <ns1:Units>2.42</ns1:Units>
                              <ns1:PricePerUnit>120.00</ns1:PricePerUnit>
                              <ns1:Price>290.40</ns1:Price>
                           </ns1:Wage>
                           <ns1:TotalWages>290.40</ns1:TotalWages>
                           <ns1:Material>
                              <ns1:FlatPercentage>25</ns1:FlatPercentage>
                              <ns1:FlatAmount>72.6</ns1:FlatAmount>
                              <ns1:MaterialGroups/>
                              <ns1:TotalSum>72.6</ns1:TotalSum>
                              <ns1:SumMaterialCorrected>72.6</ns1:SumMaterialCorrected>
                           </ns1:Material>
                           <ns1:TotalSum>363</ns1:TotalSum>
                        </ns1:LacquerCosts>
                        <ns1:TotalNetCosts>2430.71</ns1:TotalNetCosts>
                        <ns1:TotalVAT>461.83</ns1:TotalVAT>
                        <ns1:TotalGrossCosts>2892.54</ns1:TotalGrossCosts>
                        <ns1:TotalNetCorrected>2430.71</ns1:TotalNetCorrected>
                        <ns1:TotalVATCorrected>461.83</ns1:TotalVATCorrected>
                        <ns1:TotalGrossCorrected>2892.54</ns1:TotalGrossCorrected>
                        <ns1:SumNet>2430.71</ns1:SumNet>
                        <ns1:SumGross>2892.54</ns1:SumGross>
                        <ns1:SumSparePartCosts>1504.23</ns1:SumSparePartCosts>
                        <ns1:SumSmallSparePartCosts>30.08</ns1:SumSmallSparePartCosts>
                        <ns1:SumLabourCosts>533.4</ns1:SumLabourCosts>
                        <ns1:MetaPositions>
                           <ns1:MetaPosition key="TIME_UNIT_SYSTEM" value="STD"/>
                           <ns1:MetaPosition key="LACQUER_TIME_UNIT_SYSTEM" value="STD"/>
                           <ns1:MetaPosition key="DAT_EUROLACQUER_IN_HOURS" value="false"/>
                           <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EQUIPMENT" value="false"/>
                           <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EXTENSION" value="false"/>
                           <ns1:MetaPosition key="FLAT_PERCENTAGE_BASE" value="290.4"/>
                        </ns1:MetaPositions>
                     </ns1:RepairCalculationSummary>
                  </ns1:CalcResultExtension>
                  <ns1:CalculationSummary>
                     <ns1:SparePartsCosts>
                        <ns1:AllSum>1477.15</ns1:AllSum>
                        <ns1:ConsumablesSurcharge>29.54</ns1:ConsumablesSurcharge>
                        <ns1:ConsumablesSurchargePercentage>2</ns1:ConsumablesSurchargePercentage>
                        <ns1:TotalSum>1506.69</ns1:TotalSum>
                     </ns1:SparePartsCosts>
                     <ns1:AuxiliaryCosts/>
                     <ns1:LabourCosts>
                        <ns1:AllSum>533.4</ns1:AllSum>
                        <ns1:Bodywork>
                           <ns1:Type>CAR BODY</ns1:Type>
                           <ns1:Units>4.75</ns1:Units>
                           <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                           <ns1:Price>498.75</ns1:Price>
                        </ns1:Bodywork>
                        <ns1:Electric>
                           <ns1:Type>ELECTRICS</ns1:Type>
                           <ns1:Units>0.33</ns1:Units>
                           <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                           <ns1:Price>34.65</ns1:Price>
                        </ns1:Electric>
                        <ns1:Mechanic>
                           <ns1:Type>MECHANICS</ns1:Type>
                           <ns1:Units>0</ns1:Units>
                           <ns1:Price>0</ns1:Price>
                        </ns1:Mechanic>
                        <ns1:TotalSum>533.4</ns1:TotalSum>
                        <ns1:Wages/>
                        <ns1:Works>
                           <ns1:Work>
                              <ns1:Type>CAR BODY</ns1:Type>
                              <ns1:WageLevel>1</ns1:WageLevel>
                              <ns1:Units>4.75</ns1:Units>
                              <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                              <ns1:Price>498.75</ns1:Price>
                           </ns1:Work>
                           <ns1:Work>
                              <ns1:Type>ELECTRICS</ns1:Type>
                              <ns1:WageLevel>1</ns1:WageLevel>
                              <ns1:Units>0.33</ns1:Units>
                              <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                              <ns1:Price>34.65</ns1:Price>
                           </ns1:Work>
                        </ns1:Works>
                     </ns1:LabourCosts>
                     <ns1:LacquerCosts>
                        <ns1:Wage>
                           <ns1:Type>LACQUER WORK</ns1:Type>
                           <ns1:Units>2.42</ns1:Units>
                           <ns1:PricePerUnit>120.00</ns1:PricePerUnit>
                           <ns1:Price>290.40</ns1:Price>
                        </ns1:Wage>
                        <ns1:TotalWages>290.40</ns1:TotalWages>
                        <ns1:Material>
                           <ns1:FlatPercentage>25</ns1:FlatPercentage>
                           <ns1:FlatAmount>72.6</ns1:FlatAmount>
                           <ns1:MaterialGroups/>
                           <ns1:TotalSum>72.6</ns1:TotalSum>
                           <ns1:SumMaterialCorrected>72.6</ns1:SumMaterialCorrected>
                        </ns1:Material>
                        <ns1:TotalSum>363</ns1:TotalSum>
                     </ns1:LacquerCosts>
                     <ns1:TotalNetCosts>2403.09</ns1:TotalNetCosts>
                     <ns1:TotalVAT>456.59</ns1:TotalVAT>
                     <ns1:TotalGrossCosts>2859.68</ns1:TotalGrossCosts>
                     <ns1:TotalNetCorrected>2403.09</ns1:TotalNetCorrected>
                     <ns1:TotalVATCorrected>456.59</ns1:TotalVATCorrected>
                     <ns1:TotalGrossCorrected>2859.68</ns1:TotalGrossCorrected>
                     <ns1:SumNet>2403.09</ns1:SumNet>
                     <ns1:SumGross>2859.68</ns1:SumGross>
                     <ns1:SumSparePartCosts>1477.15</ns1:SumSparePartCosts>
                     <ns1:SumSmallSparePartCosts>29.54</ns1:SumSmallSparePartCosts>
                     <ns1:SumLabourCosts>533.4</ns1:SumLabourCosts>
                     <ns1:MetaPositions>
                        <ns1:MetaPosition key="TOTAL_NET_RISK" value="27.08"/>
                        <ns1:MetaPosition key="VAT_RISK" value="5.15"/>
                        <ns1:MetaPosition key="TOTAL_GROSS_RISK" value="32.23"/>
                        <ns1:MetaPosition key="TIME_UNIT_SYSTEM" value="STD"/>
                        <ns1:MetaPosition key="LACQUER_TIME_UNIT_SYSTEM" value="STD"/>
                        <ns1:MetaPosition key="DAT_EUROLACQUER_IN_HOURS" value="false"/>
                        <ns1:MetaPosition key="TOTAL_PRICE_SPARE_PARTS_RISK" value="27.08"/>
                        <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EQUIPMENT" value="false"/>
                        <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EXTENSION" value="false"/>
                        <ns1:MetaPosition key="FLAT_PERCENTAGE_BASE" value="290.4"/>
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
                  <ns1:OrderNumber>60774959    20231222120449501</ns1:OrderNumber>
                  <ns1:InvoiceDate>2023-12-22T12:05:00.056+01:00</ns1:InvoiceDate>
               </ns1:RepairOrder>
               <ns1:InsuranceClaim>false</ns1:InsuranceClaim>
               <ns1:ProcessManagement/>
            </ns1:Dossier>
         </contractResult>
      </ns4:getContractResponse>
   </S:Body>
</S:Envelope>
