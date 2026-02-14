---
title: "Response calculateContract"
topic_id: "18903"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > (Nach-) Kalkulieren eines bestehenden Vorgangs > Response calculateContract"
---

# Response calculateContract

<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns3:calculateNResponse xmlns:ns3="http://sphinx.dat.de/services/VehicleRepairService">
         <calculationResult source="SD3" type="VehicleRepairOnline">
            <ns1:Dossier xmlns:ns1="http://www.dat.de/vxs">
               <ns1:UUID>68bd10cb-8893-42ee-bd16-aab500a1bea2</ns1:UUID>
               <ns1:Country>DE</ns1:Country>
               <ns1:Language>de_DE</ns1:Language>
               <ns1:DataVersion>1</ns1:DataVersion>
               <ns1:Currency>EUR</ns1:Currency>
               <ns1:DatCustomerId>999999</ns1:DatCustomerId>
               <ns1:DossierType>repair</ns1:DossierType>
               <ns1:CreateDate>2023-12-22T09:20:39.261+01:00</ns1:CreateDate>
               <ns1:ChangeDate>2023-12-22T09:20:39.355+01:00</ns1:ChangeDate>
               <ns1:DatCustomerAddress>
                  <ns1:Title>titleCompany</ns1:Title>
                  <ns1:CompanyName>DAT - Intern</ns1:CompanyName>
                  <ns1:NameLong>Schulung SST-Partner</ns1:NameLong>
                  <ns1:Country>DE</ns1:Country>
                  <ns1:CustomerNumber>999999</ns1:CustomerNumber>
                  <ns1:CustomerType>999999</ns1:CustomerType>
                  <ns1:Street>Hellmuth-Hirth-Str.</ns1:Street>
                  <ns1:StreetNumber>1</ns1:StreetNumber>
                  <ns1:StreetZipCode>73760</ns1:StreetZipCode>
                  <ns1:StreetCity>Ostfildern</ns1:StreetCity>
                  <ns1:EMail>kundendienst@dat.de</ns1:EMail>
                  <ns1:PhoneBusiness>+49 711/450000</ns1:PhoneBusiness>
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
                     <ns1:DeselectedSeriesEquipment>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>24115</ns1:DatEquipmentId>
                           <ns1:Description>Audiosystem BMW Professional (Radio/CD-Player MP3-fähig)</ns1:Description>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25699</ns1:DatEquipmentId>
                           <ns1:Description>Schaltpunktanzeige</ns1:Description>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25924</ns1:DatEquipmentId>
                           <ns1:Description>Control-Display mit Farbmonitor (6,5 Zoll)</ns1:Description>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26302</ns1:DatEquipmentId>
                           <ns1:Description>Innenausstattung: Interieurleisten, schwarz hochglänzend</ns1:Description>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>29003</ns1:DatEquipmentId>
                           <ns1:Description>Klimaautomatik 2-Zonen</ns1:Description>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>30470</ns1:DatEquipmentId>
                           <ns1:Description>Sitzbezug / Polsterung: Stoff Diagonal</ns1:Description>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>75205</ns1:DatEquipmentId>
                           <ns1:Description>Getriebe 6-Gang</ns1:Description>
                        </ns1:EquipmentPosition>
                     </ns1:DeselectedSeriesEquipment>
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
                     <ns1:LastName>Test</ns1:LastName>
                     <ns1:FirstName>Heiner</ns1:FirstName>
                     <ns1:Country>DE</ns1:Country>
                     <ns1:UsageFlag>2</ns1:UsageFlag>
                  </ns1:Owner>
                  <ns1:ClientContactAddresses>
                     <ns1:ClientContactAddress>
                        <ns1:Title>titleCompany</ns1:Title>
                        <ns1:CompanyName>DAT - Intern</ns1:CompanyName>
                        <ns1:NameLong>Schulung SST-Partner</ns1:NameLong>
                        <ns1:Country>DE</ns1:Country>
                        <ns1:CustomerNumber>1300553</ns1:CustomerNumber>
                        <ns1:CustomerType>1300553</ns1:CustomerType>
                        <ns1:Street>Hellmuth-Hirth-Str.</ns1:Street>
                        <ns1:StreetNumber>1</ns1:StreetNumber>
                        <ns1:StreetZipCode>73760</ns1:StreetZipCode>
                        <ns1:StreetCity>Ostfildern</ns1:StreetCity>
                        <ns1:EMail>kundendienst@dat.de</ns1:EMail>
                        <ns1:PhoneBusiness>+49 711/4503-0</ns1:PhoneBusiness>
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
                        <ns1:DeselectedSeriesEquipment>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>24115</ns1:DatEquipmentId>
                              <ns1:Description>Audiosystem BMW Professional (Radio/CD-Player MP3-fähig)</ns1:Description>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25699</ns1:DatEquipmentId>
                              <ns1:Description>Schaltpunktanzeige</ns1:Description>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25924</ns1:DatEquipmentId>
                              <ns1:Description>Control-Display mit Farbmonitor (6,5 Zoll)</ns1:Description>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>26302</ns1:DatEquipmentId>
                              <ns1:Description>Innenausstattung: Interieurleisten, schwarz hochglänzend</ns1:Description>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>29003</ns1:DatEquipmentId>
                              <ns1:Description>Klimaautomatik 2-Zonen</ns1:Description>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>30470</ns1:DatEquipmentId>
                              <ns1:Description>Sitzbezug / Polsterung: Stoff Diagonal</ns1:Description>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>75205</ns1:DatEquipmentId>
                              <ns1:Description>Getriebe 6-Gang</ns1:Description>
                           </ns1:EquipmentPosition>
                        </ns1:DeselectedSeriesEquipment>
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
                     <ns1:ProcedureRelatedParameter attribute="biwOptimizationMode" factor="CalculationFactor" type="BiwOptimizationMode">AUTOMATIC</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="selectedLacquerMethod" factor="CalculationFactor" type="LacquerMethod">MANUFACTURER_SPECIFIC</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="crossSeries" factor="CalculationFactor" type="CrossSeriesState">NO</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="withoutValuesOfAdditionallyRequiredPositions" factor="CalculationFactor" type="Boolean">false</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnit" factor="CalculationFactor" type="TimeUnitSystem">HOUR</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="CalculationFactor" type="Integer">1</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="dataCurrency" factor="CalculationFactor" type="String">EUR</ns1:ProcedureRelatedParameter>
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
                     <ns1:ProcedureRelatedParameter attribute="typeSaved" factor="EuroLacquerFactor" type="Boolean">false</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wageMode" factor="EuroLacquerFactor" type="LacquerWageMode">PER_TIME</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wageInclMaterialMode" factor="EuroLacquerFactor" type="LacquerWageMode">PER_TIME</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="calculationType" factor="EuroLacquerFactor" type="LacquerCalculationMode">WAGE_MATERIAL_SEPARATELY</ns1:ProcedureRelatedParameter>
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
                     <ns1:ProcedureRelatedParameter attribute="aztDataset" factor="AztLacquerFactor" type="Integer">1</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="typeSaved" factor="AztLacquerFactor" type="Boolean">false</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wageMode" factor="AztLacquerFactor" type="LacquerWageMode">PER_TIME</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wageInclMaterialMode" factor="AztLacquerFactor" type="LacquerWageMode">PER_TIME</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="calculationType" factor="AztLacquerFactor" type="LacquerCalculationMode">WAGE_MATERIAL_SEPARATELY</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnit" factor="AztLacquerFactor" type="TimeUnitSystem">HOUR</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="threeLayerLacquerMode" factor="AztLacquerFactor" type="AztLacquerMode">WET_IN_WET</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="AztLacquerFactor" type="Integer">1</ns1:ProcedureRelatedParameter>
                  </ns1:ProcedureRelatedParameters>
                  <ns1:RepairPositions>
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>0</ns1:DATProcessId>
                        <ns1:RepairType>lacquer</ns1:RepairType>
                        <ns1:Description>Spoiler lackieren</ns1:Description>
                        <ns1:IsManualDescription>false</ns1:IsManualDescription>
                        <ns1:PositionEntryType>manual</ns1:PositionEntryType>
                        <ns1:IsRepairExtension>false</ns1:IsRepairExtension>
                        <ns1:WorkTime>3.0</ns1:WorkTime>
                        <ns1:LacquerLevel>surface</ns1:LacquerLevel>
                        <ns1:LacquerLevelId>1</ns1:LacquerLevelId>
                        <ns1:PreDamage>false</ns1:PreDamage>
                        <ns1:WorkIndication>1</ns1:WorkIndication>
                     </ns1:RepairPosition>
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>44210</ns1:DATProcessId>
                        <ns1:RepairType>replace</ns1:RepairType>
                        <ns1:Description>Frontklappe</ns1:Description>
                        <ns1:IsManualDescription>false</ns1:IsManualDescription>
                        <ns1:ConstructionGroupId>1</ns1:ConstructionGroupId>
                        <ns1:ConstructionGroup>VORDERWAGEN AUSSEN</ns1:ConstructionGroup>
                        <ns1:ConstructionGroupPolygon>20</ns1:ConstructionGroupPolygon>
                        <ns1:PositionEntryType>graphical</ns1:PositionEntryType>
                        <ns1:IsRepairExtension>false</ns1:IsRepairExtension>
                        <ns1:PreDamage>false</ns1:PreDamage>
                     </ns1:RepairPosition>
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>43711</ns1:DATProcessId>
                        <ns1:RepairType>overhaul</ns1:RepairType>
                        <ns1:Description>Seitenwand grundiert</ns1:Description>
                        <ns1:DescriptionId>36419456</ns1:DescriptionId>
                        <ns1:IsManualDescription>false</ns1:IsManualDescription>
                        <ns1:ConstructionGroupId>1</ns1:ConstructionGroupId>
                        <ns1:ConstructionGroup>VORDERWAGEN AUSSEN</ns1:ConstructionGroup>
                        <ns1:ConstructionGroupPolygon>63</ns1:ConstructionGroupPolygon>
                        <ns1:PositionEntryType>graphical</ns1:PositionEntryType>
                        <ns1:IsRepairExtension>false</ns1:IsRepairExtension>
                        <ns1:WorkTime>1.0</ns1:WorkTime>
                        <ns1:PreDamage>false</ns1:PreDamage>
                        <ns1:WorkIndication>1</ns1:WorkIndication>
                     </ns1:RepairPosition>
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>99051</ns1:DATProcessId>
                        <ns1:RepairType>replace</ns1:RepairType>
                        <ns1:Description>Hohlraumschutz</ns1:Description>
                        <ns1:IsManualDescription>false</ns1:IsManualDescription>
                        <ns1:PositionEntryType>additional</ns1:PositionEntryType>
                        <ns1:IsRepairExtension>false</ns1:IsRepairExtension>
                        <ns1:SparePartPrice>200.0</ns1:SparePartPrice>
                        <ns1:PreDamage>false</ns1:PreDamage>
                        <ns1:WorkIndication>0</ns1:WorkIndication>
                     </ns1:RepairPosition>
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>47151</ns1:DATProcessId>
                        <ns1:RepairType>lacquer</ns1:RepairType>
                        <ns1:Description>Verkleidung Stoßfänger grundiert</ns1:Description>
                        <ns1:DescriptionId>155061</ns1:DescriptionId>
                        <ns1:IsManualDescription>false</ns1:IsManualDescription>
                        <ns1:ConstructionGroupId>43</ns1:ConstructionGroupId>
                        <ns1:ConstructionGroup>STOSSFAENGER VORN / NIGHT VISION - / SIDE VIEW KAMERA</ns1:ConstructionGroup>
                        <ns1:ConstructionGroupPolygon>30</ns1:ConstructionGroupPolygon>
                        <ns1:PositionEntryType>graphical</ns1:PositionEntryType>
                        <ns1:IsRepairExtension>false</ns1:IsRepairExtension>
                        <ns1:LacquerLevel>major</ns1:LacquerLevel>
                        <ns1:LacquerLevelId>3</ns1:LacquerLevelId>
                        <ns1:PreDamage>false</ns1:PreDamage>
                     </ns1:RepairPosition>
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>44910</ns1:DATProcessId>
                        <ns1:RepairType>dis- and mounting</ns1:RepairType>
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
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>99045</ns1:DATProcessId>
                        <ns1:RepairType>replace</ns1:RepairType>
                        <ns1:Description>Entsorgungskosten</ns1:Description>
                        <ns1:IsManualDescription>false</ns1:IsManualDescription>
                        <ns1:PositionEntryType>additional</ns1:PositionEntryType>
                        <ns1:IsRepairExtension>false</ns1:IsRepairExtension>
                        <ns1:SparePartPrice>100.0</ns1:SparePartPrice>
                        <ns1:PreDamage>false</ns1:PreDamage>
                        <ns1:WorkIndication>0</ns1:WorkIndication>
                     </ns1:RepairPosition>
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>20111</ns1:DATProcessId>
                        <ns1:RepairType>overhaul</ns1:RepairType>
                        <ns1:Description>Tür</ns1:Description>
                        <ns1:DescriptionId>77066</ns1:DescriptionId>
                        <ns1:IsManualDescription>false</ns1:IsManualDescription>
                        <ns1:ConstructionGroupId>11</ns1:ConstructionGroupId>
                        <ns1:ConstructionGroup>TUER V.</ns1:ConstructionGroup>
                        <ns1:ConstructionGroupPolygon>13</ns1:ConstructionGroupPolygon>
                        <ns1:PositionEntryType>graphical</ns1:PositionEntryType>
                        <ns1:CrossSeries>false</ns1:CrossSeries>
                        <ns1:IsRepairExtension>true</ns1:IsRepairExtension>
                        <ns1:WorkTime>1.0</ns1:WorkTime>
                        <ns1:PreDamage>false</ns1:PreDamage>
                        <ns1:WorkIndication>1</ns1:WorkIndication>
                     </ns1:RepairPosition>
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>110</ns1:DATProcessId>
                        <ns1:RepairType>overhaul</ns1:RepairType>
                        <ns1:Description>Dach</ns1:Description>
                        <ns1:DescriptionId>11489568</ns1:DescriptionId>
                        <ns1:IsManualDescription>false</ns1:IsManualDescription>
                        <ns1:ConstructionGroupId>10</ns1:ConstructionGroupId>
                        <ns1:ConstructionGroup>FAHRGASTZELLE</ns1:ConstructionGroup>
                        <ns1:ConstructionGroupPolygon>15</ns1:ConstructionGroupPolygon>
                        <ns1:PositionEntryType>dents</ns1:PositionEntryType>
                        <ns1:IsRepairExtension>false</ns1:IsRepairExtension>
                        <ns1:DentsCount>10</ns1:DentsCount>
                        <ns1:DentsSize>20</ns1:DentsSize>
                        <ns1:DentsPartOrientation>horizontal</ns1:DentsPartOrientation>
                        <ns1:DentsCalculationMethod>bvat</ns1:DentsCalculationMethod>
                        <ns1:DentsWithFinishing>true</ns1:DentsWithFinishing>
                        <ns1:DentsWithSetupTime>true</ns1:DentsWithSetupTime>
                        <ns1:IsAdditionalLM>true</ns1:IsAdditionalLM>
                        <ns1:PreDamage>false</ns1:PreDamage>
                     </ns1:RepairPosition>
                  </ns1:RepairPositions>
                  <ns1:CalcResultToUse>common</ns1:CalcResultToUse>
                  <ns1:CalcResultCommon>
                     <ns1:MaterialPositions>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>44210</ns1:DATProcessId>
                           <ns1:PartNumber>41617207194</ns1:PartNumber>
                           <ns1:DATPartNumber>41617207194</ns1:DATPartNumber>
                           <ns1:Description>FRONTKLAPPE ALUMINIUM</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>1017.20</ns1:ValuePerUnit>
                           <ns1:ValueTotal>1017.20</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>1017.20</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                     </ns1:MaterialPositions>
                     <ns1:AdditionalCostsPositions>
                        <ns1:AdditionalCostsPosition>
                           <ns1:DATProcessId>99045</ns1:DATProcessId>
                           <ns1:Description>ENTSORGUNGSKOSTEN</ns1:Description>
                           <ns1:ValueTotal>100.00</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>true</ns1:ManualPrice>
                           <ns1:ValuePerUnit>100.00</ns1:ValuePerUnit>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:PartNumber/>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:AdditionalCostsPositionPriceState>*</ns1:AdditionalCostsPositionPriceState>
                        </ns1:AdditionalCostsPosition>
                        <ns1:AdditionalCostsPosition>
                           <ns1:DATProcessId>99051</ns1:DATProcessId>
                           <ns1:Description>HOHLRAUMSCHUTZMATERIAL: HOHLRAUMSCHUTZ</ns1:Description>
                           <ns1:ValueTotal>200.00</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>true</ns1:ManualPrice>
                           <ns1:ValuePerUnit>200.00</ns1:ValuePerUnit>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:PartNumber/>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:AdditionalCostsPositionPriceState>*</ns1:AdditionalCostsPositionPriceState>
                        </ns1:AdditionalCostsPosition>
                     </ns1:AdditionalCostsPositions>
                     <ns1:ExtensionPositions>
                        <ns1:ExtensionPosition>
                           <ns1:DATProcessId>20111</ns1:DATProcessId>
                           <ns1:RepairType>overhaul</ns1:RepairType>
                           <ns1:Description>TUER</ns1:Description>
                           <ns1:LabourTime>1.00</ns1:LabourTime>
                           <ns1:LabourSum>105.00</ns1:LabourSum>
                           <ns1:LacquerTime>4.67</ns1:LacquerTime>
                           <ns1:LacquerWageSum>560.40</ns1:LacquerWageSum>
                           <ns1:LacquerMaterialSum>140.10</ns1:LacquerMaterialSum>
                        </ns1:ExtensionPosition>
                     </ns1:ExtensionPositions>
                     <ns1:LabourPositions>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>44210</ns1:DATProcessId>
                           <ns1:LabourPositionKind>1</ns1:LabourPositionKind>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:LabourPosId>41 61 502</ns1:LabourPosId>
                           <ns1:Description>FRONTKLAPPE ERS.
UMFASST: FRONTKLAPPE A+E</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>1.17</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>122.85</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>122.85</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>41 61 502</ns1:WorkNumber>
                           <ns1:SparePartNumber>41617207194</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>44910</ns1:DATProcessId>
                           <ns1:LabourPositionKind>1</ns1:LabourPositionKind>
                           <ns1:RepairType>dis- and mounting</ns1:RepairType>
                           <ns1:LabourPosId>51 31 503</ns1:LabourPosId>
                           <ns1:Description>FRONTSCHEIBE A+E</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>1.92</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>201.60</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>201.60</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>51 31 503</ns1:WorkNumber>
                           <ns1:SparePartNumber>51317333835</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>43711</ns1:DATProcessId>
                           <ns1:LabourPositionKind>1</ns1:LabourPositionKind>
                           <ns1:RepairType>overhaul</ns1:RepairType>
                           <ns1:LabourPosId>41 99 000</ns1:LabourPosId>
                           <ns1:Description>SEITENWAND V.L. INST.</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>1.00</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>105.00</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>105.00</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState>*</ns1:LabourPositionTimeState>
                           <ns1:TimeOrigin>MANUAL</ns1:TimeOrigin>
                           <ns1:WorkNumber>41 99 000</ns1:WorkNumber>
                           <ns1:SparePartNumber>41355A03261</ns1:SparePartNumber>
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
                        <ns1:DentBvatPosition>
                           <ns1:DATProcessId>110</ns1:DATProcessId>
                           <ns1:RepairType>overhaul</ns1:RepairType>
                           <ns1:Description>DACHAUSSENHAUT
(GROESSE: 20 MM)</ns1:Description>
                           <ns1:WageType>dents</ns1:WageType>
                           <ns1:Duration>1.50</ns1:Duration>
                           <ns1:ValueTotal>117.00</ns1:ValueTotal>
                           <ns1:ValueTotalCorrected>146.64</ns1:ValueTotalCorrected>
                           <ns1:Amount>10</ns1:Amount>
                           <ns1:size>20</ns1:size>
                           <ns1:DentsCalculationMethod>press</ns1:DentsCalculationMethod>
                           <ns1:SparePartNumber>41317240446</ns1:SparePartNumber>
                        </ns1:DentBvatPosition>
                        <ns1:DentBvatPosition>
                           <ns1:Description>AUFSCHLAG LEICHTMETALL 25%</ns1:Description>
                           <ns1:WageType>dents</ns1:WageType>
                           <ns1:Duration>0.38</ns1:Duration>
                           <ns1:ValueTotal>29.64</ns1:ValueTotal>
                           <ns1:DentsCalculationMethod>press</ns1:DentsCalculationMethod>
                           <ns1:ValueInPosition>true</ns1:ValueInPosition>
                        </ns1:DentBvatPosition>
                        <ns1:DentBvatPosition>
                           <ns1:Description>RUESTZEIT</ns1:Description>
                           <ns1:WageType>dents</ns1:WageType>
                           <ns1:Duration>0.60</ns1:Duration>
                           <ns1:ValueTotal>46.80</ns1:ValueTotal>
                           <ns1:ValueTotalCorrected>46.80</ns1:ValueTotalCorrected>
                           <ns1:DentsCalculationMethod>global</ns1:DentsCalculationMethod>
                        </ns1:DentBvatPosition>
                        <ns1:DentBvatPosition>
                           <ns1:Description>FINISHARBEIT (1 TEILE)</ns1:Description>
                           <ns1:WageType>dents</ns1:WageType>
                           <ns1:Duration>0.25</ns1:Duration>
                           <ns1:ValueTotal>19.50</ns1:ValueTotal>
                           <ns1:ValueTotalCorrected>19.50</ns1:ValueTotalCorrected>
                           <ns1:DentsCalculationMethod>global</ns1:DentsCalculationMethod>
                        </ns1:DentBvatPosition>
                     </ns1:LabourPositions>
                     <ns1:LacquerPositions>
                        <ns1:LacquerPosition>
                           <ns1:DATProcessId>43711</ns1:DATProcessId>
                           <ns1:LabourPosId>99 35 013</ns1:LabourPosId>
                           <ns1:Description>SEITENWAND V.L. UMFASST: VORBEREITUNGSARBEITEN</ns1:Description>
                           <ns1:Level>2</ns1:Level>
                           <ns1:LevelDescription>minor</ns1:LevelDescription>
                           <ns1:LevelManufacturer>ST.3</ns1:LevelManufacturer>
                           <ns1:Duration>3.00</ns1:Duration>
                           <ns1:ManualDuration>false</ns1:ManualDuration>
                           <ns1:Material>90.00</ns1:Material>
                           <ns1:ValueTotal>450.00</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>450.00</ns1:ValueTotalCorrected>
                           <ns1:WageLevel1>360.00</ns1:WageLevel1>
                           <ns1:WorkNumber>99 35 013</ns1:WorkNumber>
                           <ns1:LacquerPositionTimeState/>
                           <ns1:LacquerPositionMaterialState/>
                           <ns1:LacquerPositionPriceState/>
                           <ns1:MaterialType>2</ns1:MaterialType>
                           <ns1:SparePartNumber>41355A03261</ns1:SparePartNumber>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                        </ns1:LacquerPosition>
                        <ns1:LacquerPosition>
                           <ns1:DATProcessId>44210</ns1:DATProcessId>
                           <ns1:LabourPosId>99 61 529</ns1:LabourPosId>
                           <ns1:Description>FRONTKLAPPE</ns1:Description>
                           <ns1:Level>4</ns1:Level>
                           <ns1:LevelDescription>new</ns1:LevelDescription>
                           <ns1:LevelManufacturer>ST.2</ns1:LevelManufacturer>
                           <ns1:Duration>2.50</ns1:Duration>
                           <ns1:ManualDuration>false</ns1:ManualDuration>
                           <ns1:Material>75.00</ns1:Material>
                           <ns1:ValueTotal>375.00</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>375.00</ns1:ValueTotalCorrected>
                           <ns1:WageLevel1>300.00</ns1:WageLevel1>
                           <ns1:WorkNumber>99 61 529</ns1:WorkNumber>
                           <ns1:LacquerPositionTimeState/>
                           <ns1:LacquerPositionMaterialState/>
                           <ns1:LacquerPositionPriceState/>
                           <ns1:MaterialType>2</ns1:MaterialType>
                           <ns1:SparePartNumber>41617207194</ns1:SparePartNumber>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                        </ns1:LacquerPosition>
                        <ns1:LacquerPosition>
                           <ns1:DATProcessId>47151</ns1:DATProcessId>
                           <ns1:LabourPosId>99 68 539</ns1:LabourPosId>
                           <ns1:Description>STOSSFAENGER V.</ns1:Description>
                           <ns1:Level>3</ns1:Level>
                           <ns1:LevelDescription>major</ns1:LevelDescription>
                           <ns1:LevelManufacturer>ST.3</ns1:LevelManufacturer>
                           <ns1:Duration>2.25</ns1:Duration>
                           <ns1:ManualDuration>false</ns1:ManualDuration>
                           <ns1:Material>67.50</ns1:Material>
                           <ns1:ValueTotal>337.50</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>337.50</ns1:ValueTotalCorrected>
                           <ns1:WageLevel1>270.00</ns1:WageLevel1>
                           <ns1:WorkNumber>99 68 539</ns1:WorkNumber>
                           <ns1:LacquerPositionTimeState/>
                           <ns1:LacquerPositionMaterialState/>
                           <ns1:LacquerPositionPriceState/>
                           <ns1:MaterialType>1</ns1:MaterialType>
                           <ns1:SparePartNumber>51117332676</ns1:SparePartNumber>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                        </ns1:LacquerPosition>
                        <ns1:LacquerPosition>
                           <ns1:Description>SPOILER LACKIEREN</ns1:Description>
                           <ns1:Level>1</ns1:Level>
                           <ns1:LevelDescription>surface</ns1:LevelDescription>
                           <ns1:Duration>3.00</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:Material>90.00</ns1:Material>
                           <ns1:ValueTotal>450.00</ns1:ValueTotal>
                           <ns1:ManualPosition>true</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>450.00</ns1:ValueTotalCorrected>
                           <ns1:WageLevel1>360.00</ns1:WageLevel1>
                           <ns1:TimeOrigin>MANUAL</ns1:TimeOrigin>
                           <ns1:LacquerPositionTimeState>*</ns1:LacquerPositionTimeState>
                           <ns1:LacquerPositionMaterialState>*</ns1:LacquerPositionMaterialState>
                           <ns1:LacquerPositionPriceState/>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                        </ns1:LacquerPosition>
                     </ns1:LacquerPositions>
                     <ns1:PriceDate>2023-12-01+01:00</ns1:PriceDate>
                     <ns1:RepairCalculationSummary>
                        <ns1:SparePartsCosts>
                           <ns1:AllSum>1017.20</ns1:AllSum>
                           <ns1:ConsumablesSurcharge>20.34</ns1:ConsumablesSurcharge>
                           <ns1:ConsumablesSurchargePercentage>2.00</ns1:ConsumablesSurchargePercentage>
                           <ns1:TotalSum>1037.54</ns1:TotalSum>
                        </ns1:SparePartsCosts>
                        <ns1:AuxiliaryCosts>
                           <ns1:AuxiliaryCosts>300.00</ns1:AuxiliaryCosts>
                           <ns1:TotalSum>300.00</ns1:TotalSum>
                        </ns1:AuxiliaryCosts>
                        <ns1:LabourCosts>
                           <ns1:AllSum>660.24</ns1:AllSum>
                           <ns1:Bodywork>
                              <ns1:Type>CAR BODY</ns1:Type>
                              <ns1:Units>4.26</ns1:Units>
                              <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                              <ns1:Price>447.30</ns1:Price>
                           </ns1:Bodywork>
                           <ns1:Electric>
                              <ns1:Type>ELECTRICS</ns1:Type>
                              <ns1:Units>0</ns1:Units>
                              <ns1:Price>0</ns1:Price>
                           </ns1:Electric>
                           <ns1:Mechanic>
                              <ns1:Type>MECHANICS</ns1:Type>
                              <ns1:Units>0</ns1:Units>
                              <ns1:Price>0</ns1:Price>
                           </ns1:Mechanic>
                           <ns1:DentsPress>
                              <ns1:Type>HAIL DAMAGE PRESS</ns1:Type>
                              <ns1:Units>1.88</ns1:Units>
                              <ns1:PricePerUnit>78.00</ns1:PricePerUnit>
                              <ns1:Price>146.64</ns1:Price>
                           </ns1:DentsPress>
                           <ns1:DentsGlobal>
                              <ns1:Type>HAIL DAMAGE GENERAL</ns1:Type>
                              <ns1:Units>0.85</ns1:Units>
                              <ns1:PricePerUnit>78.00</ns1:PricePerUnit>
                              <ns1:Price>66.30</ns1:Price>
                           </ns1:DentsGlobal>
                           <ns1:TotalSum>660.24</ns1:TotalSum>
                           <ns1:Wages/>
                           <ns1:Works>
                              <ns1:Work>
                                 <ns1:Type>CAR BODY</ns1:Type>
                                 <ns1:WageLevel>1</ns1:WageLevel>
                                 <ns1:Units>4.26</ns1:Units>
                                 <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                                 <ns1:Price>447.30</ns1:Price>
                              </ns1:Work>
                              <ns1:Work>
                                 <ns1:Type>HAIL DAMAGE PRESS</ns1:Type>
                                 <ns1:Units>1.88</ns1:Units>
                                 <ns1:PricePerUnit>78.00</ns1:PricePerUnit>
                                 <ns1:Price>146.64</ns1:Price>
                              </ns1:Work>
                              <ns1:Work>
                                 <ns1:Type>HAIL DAMAGE GENERAL</ns1:Type>
                                 <ns1:Units>0.85</ns1:Units>
                                 <ns1:PricePerUnit>78.00</ns1:PricePerUnit>
                                 <ns1:Price>66.30</ns1:Price>
                              </ns1:Work>
                           </ns1:Works>
                        </ns1:LabourCosts>
                        <ns1:LacquerCosts>
                           <ns1:Wage>
                              <ns1:Type>LACQUER WORK</ns1:Type>
                              <ns1:Units>10.75</ns1:Units>
                              <ns1:PricePerUnit>120.00</ns1:PricePerUnit>
                              <ns1:Price>1290.00</ns1:Price>
                           </ns1:Wage>
                           <ns1:TotalWages>1290.00</ns1:TotalWages>
                           <ns1:Material>
                              <ns1:FlatPercentage>25.0</ns1:FlatPercentage>
                              <ns1:FlatAmount>322.50</ns1:FlatAmount>
                              <ns1:MaterialGroups/>
                              <ns1:TotalSum>322.50</ns1:TotalSum>
                              <ns1:SumMaterialCorrected>322.50</ns1:SumMaterialCorrected>
                           </ns1:Material>
                           <ns1:TotalSum>1612.50</ns1:TotalSum>
                        </ns1:LacquerCosts>
                        <ns1:TotalNetCosts>3610.28</ns1:TotalNetCosts>
                        <ns1:TotalVAT>685.95</ns1:TotalVAT>
                        <ns1:TotalGrossCosts>4296.23</ns1:TotalGrossCosts>
                        <ns1:TotalNetCorrected>3610.28</ns1:TotalNetCorrected>
                        <ns1:TotalVATCorrected>685.95</ns1:TotalVATCorrected>
                        <ns1:TotalGrossCorrected>4296.23</ns1:TotalGrossCorrected>
                        <ns1:SumNet>3610.28</ns1:SumNet>
                        <ns1:SumGross>4296.23</ns1:SumGross>
                        <ns1:SumSparePartCosts>1017.20</ns1:SumSparePartCosts>
                        <ns1:SumSmallSparePartCosts>20.34</ns1:SumSmallSparePartCosts>
                        <ns1:SumMiscellaneousCosts>300.00</ns1:SumMiscellaneousCosts>
                        <ns1:SumLabourCosts>660.24</ns1:SumLabourCosts>
                        <ns1:MetaPositions>
                           <ns1:MetaPosition key="TIME_UNIT_SYSTEM" value="STD"/>
                           <ns1:MetaPosition key="LACQUER_TIME_UNIT_SYSTEM" value="STD"/>
                           <ns1:MetaPosition key="DAT_EUROLACQUER_IN_HOURS" value="false"/>
                           <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EQUIPMENT" value="false"/>
                           <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EXTENSION" value="false"/>
                           <ns1:MetaPosition key="FLAT_PERCENTAGE_BASE" value="1290.00"/>
                        </ns1:MetaPositions>
                     </ns1:RepairCalculationSummary>
                     <ns1:CalcProtocol>
                        <ns1:ProtocolHints>
                           <ns1:ProtocolHint>
                              <ns1:Identifier>H001</ns1:Identifier>
                              <ns1:Description>Serientreue Kalkulation</ns1:Description>
                           </ns1:ProtocolHint>
                        </ns1:ProtocolHints>
                        <ns1:DentPositionsProtocol>
                           <ns1:DentPositionsProtocolEntry>
                              <ns1:DATProcessId>110</ns1:DATProcessId>
                              <ns1:Description>Dach</ns1:Description>
                              <ns1:CalculationMethod>bvat</ns1:CalculationMethod>
                              <ns1:CalculationMethodDescription>Bundesverband Ausbeultechnik (BVAT), Drücken</ns1:CalculationMethodDescription>
                              <ns1:DentsCount>10</ns1:DentsCount>
                              <ns1:DentsSize>20</ns1:DentsSize>
                           </ns1:DentPositionsProtocolEntry>
                        </ns1:DentPositionsProtocol>
                     </ns1:CalcProtocol>
                  </ns1:CalcResultCommon>
                  <ns1:CalcResultExtension>
                     <ns1:MaterialPositions>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>44210</ns1:DATProcessId>
                           <ns1:PartNumber>41617207194</ns1:PartNumber>
                           <ns1:DATPartNumber>41617207194</ns1:DATPartNumber>
                           <ns1:Description>FRONTKLAPPE ALUMINIUM</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>1017.20</ns1:ValuePerUnit>
                           <ns1:ValueTotal>1017.20</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>1017.20</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                     </ns1:MaterialPositions>
                     <ns1:AdditionalCostsPositions>
                        <ns1:AdditionalCostsPosition>
                           <ns1:DATProcessId>99045</ns1:DATProcessId>
                           <ns1:Description>ENTSORGUNGSKOSTEN</ns1:Description>
                           <ns1:ValueTotal>100.00</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>true</ns1:ManualPrice>
                           <ns1:ValuePerUnit>100.00</ns1:ValuePerUnit>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:PartNumber/>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:AdditionalCostsPositionPriceState>*</ns1:AdditionalCostsPositionPriceState>
                        </ns1:AdditionalCostsPosition>
                        <ns1:AdditionalCostsPosition>
                           <ns1:DATProcessId>99051</ns1:DATProcessId>
                           <ns1:Description>HOHLRAUMSCHUTZMATERIAL: HOHLRAUMSCHUTZ</ns1:Description>
                           <ns1:ValueTotal>200.00</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>true</ns1:ManualPrice>
                           <ns1:ValuePerUnit>200.00</ns1:ValuePerUnit>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:PartNumber/>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:AdditionalCostsPositionPriceState>*</ns1:AdditionalCostsPositionPriceState>
                        </ns1:AdditionalCostsPosition>
                     </ns1:AdditionalCostsPositions>
                     <ns1:LabourPositions>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>44210</ns1:DATProcessId>
                           <ns1:LabourPositionKind>1</ns1:LabourPositionKind>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:LabourPosId>41 61 502</ns1:LabourPosId>
                           <ns1:Description>FRONTKLAPPE ERS.
UMFASST: FRONTKLAPPE A+E</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>1.17</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>122.85</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>122.85</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>41 61 502</ns1:WorkNumber>
                           <ns1:SparePartNumber>41617207194</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>44910</ns1:DATProcessId>
                           <ns1:LabourPositionKind>1</ns1:LabourPositionKind>
                           <ns1:RepairType>dis- and mounting</ns1:RepairType>
                           <ns1:LabourPosId>51 31 503</ns1:LabourPosId>
                           <ns1:Description>FRONTSCHEIBE A+E</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>1.92</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>201.60</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>201.60</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>51 31 503</ns1:WorkNumber>
                           <ns1:SparePartNumber>51317333835</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>20111</ns1:DATProcessId>
                           <ns1:LabourPositionKind>1</ns1:LabourPositionKind>
                           <ns1:RepairType>overhaul</ns1:RepairType>
                           <ns1:LabourPosId>41 99 000</ns1:LabourPosId>
                           <ns1:Description>VORDERTUER L. INST.</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>1.00</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>105.00</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>105.00</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState>*</ns1:LabourPositionTimeState>
                           <ns1:TimeOrigin>MANUAL</ns1:TimeOrigin>
                           <ns1:WorkNumber>41 99 000</ns1:WorkNumber>
                           <ns1:WorkIndication>1</ns1:WorkIndication>
                           <ns1:SparePartNumber>41007206107</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>43711</ns1:DATProcessId>
                           <ns1:LabourPositionKind>1</ns1:LabourPositionKind>
                           <ns1:RepairType>overhaul</ns1:RepairType>
                           <ns1:LabourPosId>41 99 000</ns1:LabourPosId>
                           <ns1:Description>SEITENWAND V.L. INST.</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>1.00</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>105.00</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>105.00</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState>*</ns1:LabourPositionTimeState>
                           <ns1:TimeOrigin>MANUAL</ns1:TimeOrigin>
                           <ns1:WorkNumber>41 99 000</ns1:WorkNumber>
                           <ns1:WorkIndication>1</ns1:WorkIndication>
                           <ns1:SparePartNumber>41355A03261</ns1:SparePartNumber>
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
                        <ns1:DentBvatPosition>
                           <ns1:DATProcessId>110</ns1:DATProcessId>
                           <ns1:RepairType>overhaul</ns1:RepairType>
                           <ns1:Description>DACHAUSSENHAUT
(GROESSE: 20 MM)</ns1:Description>
                           <ns1:WageType>dents</ns1:WageType>
                           <ns1:Duration>1.50</ns1:Duration>
                           <ns1:ValueTotal>117.00</ns1:ValueTotal>
                           <ns1:ValueTotalCorrected>146.64</ns1:ValueTotalCorrected>
                           <ns1:Amount>10</ns1:Amount>
                           <ns1:size>20</ns1:size>
                           <ns1:DentsCalculationMethod>press</ns1:DentsCalculationMethod>
                           <ns1:SparePartNumber>41317240446</ns1:SparePartNumber>
                        </ns1:DentBvatPosition>
                        <ns1:DentBvatPosition>
                           <ns1:Description>AUFSCHLAG LEICHTMETALL 25%</ns1:Description>
                           <ns1:WageType>dents</ns1:WageType>
                           <ns1:Duration>0.38</ns1:Duration>
                           <ns1:ValueTotal>29.64</ns1:ValueTotal>
                           <ns1:DentsCalculationMethod>press</ns1:DentsCalculationMethod>
                           <ns1:ValueInPosition>true</ns1:ValueInPosition>
                        </ns1:DentBvatPosition>
                        <ns1:DentBvatPosition>
                           <ns1:Description>RUESTZEIT</ns1:Description>
                           <ns1:WageType>dents</ns1:WageType>
                           <ns1:Duration>0.60</ns1:Duration>
                           <ns1:ValueTotal>46.80</ns1:ValueTotal>
                           <ns1:ValueTotalCorrected>46.80</ns1:ValueTotalCorrected>
                           <ns1:DentsCalculationMethod>global</ns1:DentsCalculationMethod>
                        </ns1:DentBvatPosition>
                        <ns1:DentBvatPosition>
                           <ns1:Description>FINISHARBEIT (1 TEILE)</ns1:Description>
                           <ns1:WageType>dents</ns1:WageType>
                           <ns1:Duration>0.25</ns1:Duration>
                           <ns1:ValueTotal>19.50</ns1:ValueTotal>
                           <ns1:ValueTotalCorrected>19.50</ns1:ValueTotalCorrected>
                           <ns1:DentsCalculationMethod>global</ns1:DentsCalculationMethod>
                        </ns1:DentBvatPosition>
                     </ns1:LabourPositions>
                     <ns1:LacquerPositions>
                        <ns1:LacquerPosition>
                           <ns1:DATProcessId>20111</ns1:DATProcessId>
                           <ns1:LabourPosId>99 51 013</ns1:LabourPosId>
                           <ns1:Description>VORDERTUER L. UMFASST: VORBEREITUNGSARBEITEN</ns1:Description>
                           <ns1:Level>2</ns1:Level>
                           <ns1:LevelDescription>minor</ns1:LevelDescription>
                           <ns1:LevelManufacturer>ST.3</ns1:LevelManufacturer>
                           <ns1:Duration>4.67</ns1:Duration>
                           <ns1:ManualDuration>false</ns1:ManualDuration>
                           <ns1:Material>140.10</ns1:Material>
                           <ns1:ValueTotal>700.50</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>700.50</ns1:ValueTotalCorrected>
                           <ns1:WageLevel1>560.40</ns1:WageLevel1>
                           <ns1:WorkNumber>99 51 013</ns1:WorkNumber>
                           <ns1:LacquerPositionTimeState/>
                           <ns1:LacquerPositionMaterialState/>
                           <ns1:LacquerPositionPriceState/>
                           <ns1:MaterialType>2</ns1:MaterialType>
                           <ns1:SparePartNumber>41007206107</ns1:SparePartNumber>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                        </ns1:LacquerPosition>
                        <ns1:LacquerPosition>
                           <ns1:DATProcessId>43711</ns1:DATProcessId>
                           <ns1:LabourPosId>99 35 529</ns1:LabourPosId>
                           <ns1:Description>SEITENWAND V.L.</ns1:Description>
                           <ns1:Level>2</ns1:Level>
                           <ns1:LevelDescription>minor</ns1:LevelDescription>
                           <ns1:LevelManufacturer>ST.3</ns1:LevelManufacturer>
                           <ns1:Duration>1.17</ns1:Duration>
                           <ns1:ManualDuration>false</ns1:ManualDuration>
                           <ns1:Material>35.10</ns1:Material>
                           <ns1:ValueTotal>175.50</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>175.50</ns1:ValueTotalCorrected>
                           <ns1:WageLevel1>140.40</ns1:WageLevel1>
                           <ns1:WorkNumber>99 35 529</ns1:WorkNumber>
                           <ns1:LacquerPositionTimeState/>
                           <ns1:LacquerPositionMaterialState/>
                           <ns1:LacquerPositionPriceState/>
                           <ns1:MaterialType>2</ns1:MaterialType>
                           <ns1:SparePartNumber>41355A03261</ns1:SparePartNumber>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                        </ns1:LacquerPosition>
                        <ns1:LacquerPosition>
                           <ns1:DATProcessId>44210</ns1:DATProcessId>
                           <ns1:LabourPosId>99 61 529</ns1:LabourPosId>
                           <ns1:Description>FRONTKLAPPE</ns1:Description>
                           <ns1:Level>4</ns1:Level>
                           <ns1:LevelDescription>new</ns1:LevelDescription>
                           <ns1:LevelManufacturer>ST.2</ns1:LevelManufacturer>
                           <ns1:Duration>2.50</ns1:Duration>
                           <ns1:ManualDuration>false</ns1:ManualDuration>
                           <ns1:Material>75.00</ns1:Material>
                           <ns1:ValueTotal>375.00</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>375.00</ns1:ValueTotalCorrected>
                           <ns1:WageLevel1>300.00</ns1:WageLevel1>
                           <ns1:WorkNumber>99 61 529</ns1:WorkNumber>
                           <ns1:LacquerPositionTimeState/>
                           <ns1:LacquerPositionMaterialState/>
                           <ns1:LacquerPositionPriceState/>
                           <ns1:MaterialType>2</ns1:MaterialType>
                           <ns1:SparePartNumber>41617207194</ns1:SparePartNumber>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                        </ns1:LacquerPosition>
                        <ns1:LacquerPosition>
                           <ns1:DATProcessId>47151</ns1:DATProcessId>
                           <ns1:LabourPosId>99 68 539</ns1:LabourPosId>
                           <ns1:Description>STOSSFAENGER V.</ns1:Description>
                           <ns1:Level>3</ns1:Level>
                           <ns1:LevelDescription>major</ns1:LevelDescription>
                           <ns1:LevelManufacturer>ST.3</ns1:LevelManufacturer>
                           <ns1:Duration>2.25</ns1:Duration>
                           <ns1:ManualDuration>false</ns1:ManualDuration>
                           <ns1:Material>67.50</ns1:Material>
                           <ns1:ValueTotal>337.50</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>337.50</ns1:ValueTotalCorrected>
                           <ns1:WageLevel1>270.00</ns1:WageLevel1>
                           <ns1:WorkNumber>99 68 539</ns1:WorkNumber>
                           <ns1:LacquerPositionTimeState/>
                           <ns1:LacquerPositionMaterialState/>
                           <ns1:LacquerPositionPriceState/>
                           <ns1:MaterialType>1</ns1:MaterialType>
                           <ns1:SparePartNumber>51117332676</ns1:SparePartNumber>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                        </ns1:LacquerPosition>
                        <ns1:LacquerPosition>
                           <ns1:Description>SPOILER LACKIEREN</ns1:Description>
                           <ns1:Level>1</ns1:Level>
                           <ns1:LevelDescription>surface</ns1:LevelDescription>
                           <ns1:Duration>3.00</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:Material>90.00</ns1:Material>
                           <ns1:ValueTotal>450.00</ns1:ValueTotal>
                           <ns1:ManualPosition>true</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>450.00</ns1:ValueTotalCorrected>
                           <ns1:WageLevel1>360.00</ns1:WageLevel1>
                           <ns1:TimeOrigin>MANUAL</ns1:TimeOrigin>
                           <ns1:LacquerPositionTimeState>*</ns1:LacquerPositionTimeState>
                           <ns1:LacquerPositionMaterialState>*</ns1:LacquerPositionMaterialState>
                           <ns1:LacquerPositionPriceState/>
                           <ns1:WorkIndication>1</ns1:WorkIndication>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                        </ns1:LacquerPosition>
                     </ns1:LacquerPositions>
                     <ns1:PriceDate>2023-12-01+01:00</ns1:PriceDate>
                     <ns1:RepairCalculationSummary>
                        <ns1:SparePartsCosts>
                           <ns1:AllSum>1017.20</ns1:AllSum>
                           <ns1:ConsumablesSurcharge>20.34</ns1:ConsumablesSurcharge>
                           <ns1:ConsumablesSurchargePercentage>2.00</ns1:ConsumablesSurchargePercentage>
                           <ns1:TotalSum>1037.54</ns1:TotalSum>
                        </ns1:SparePartsCosts>
                        <ns1:AuxiliaryCosts>
                           <ns1:AuxiliaryCosts>300.00</ns1:AuxiliaryCosts>
                           <ns1:TotalSum>300.00</ns1:TotalSum>
                        </ns1:AuxiliaryCosts>
                        <ns1:LabourCosts>
                           <ns1:AllSum>765.24</ns1:AllSum>
                           <ns1:Bodywork>
                              <ns1:Type>CAR BODY</ns1:Type>
                              <ns1:Units>5.26</ns1:Units>
                              <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                              <ns1:Price>552.30</ns1:Price>
                           </ns1:Bodywork>
                           <ns1:Electric>
                              <ns1:Type>ELECTRICS</ns1:Type>
                              <ns1:Units>0</ns1:Units>
                              <ns1:Price>0</ns1:Price>
                           </ns1:Electric>
                           <ns1:Mechanic>
                              <ns1:Type>MECHANICS</ns1:Type>
                              <ns1:Units>0</ns1:Units>
                              <ns1:Price>0</ns1:Price>
                           </ns1:Mechanic>
                           <ns1:DentsPress>
                              <ns1:Type>HAIL DAMAGE PRESS</ns1:Type>
                              <ns1:Units>1.88</ns1:Units>
                              <ns1:PricePerUnit>78.00</ns1:PricePerUnit>
                              <ns1:Price>146.64</ns1:Price>
                           </ns1:DentsPress>
                           <ns1:DentsGlobal>
                              <ns1:Type>HAIL DAMAGE GENERAL</ns1:Type>
                              <ns1:Units>0.85</ns1:Units>
                              <ns1:PricePerUnit>78.00</ns1:PricePerUnit>
                              <ns1:Price>66.30</ns1:Price>
                           </ns1:DentsGlobal>
                           <ns1:TotalSum>765.24</ns1:TotalSum>
                           <ns1:Wages/>
                           <ns1:Works>
                              <ns1:Work>
                                 <ns1:Type>CAR BODY</ns1:Type>
                                 <ns1:WageLevel>1</ns1:WageLevel>
                                 <ns1:Units>5.26</ns1:Units>
                                 <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                                 <ns1:Price>552.30</ns1:Price>
                              </ns1:Work>
                              <ns1:Work>
                                 <ns1:Type>HAIL DAMAGE PRESS</ns1:Type>
                                 <ns1:Units>1.88</ns1:Units>
                                 <ns1:PricePerUnit>78.00</ns1:PricePerUnit>
                                 <ns1:Price>146.64</ns1:Price>
                              </ns1:Work>
                              <ns1:Work>
                                 <ns1:Type>HAIL DAMAGE GENERAL</ns1:Type>
                                 <ns1:Units>0.85</ns1:Units>
                                 <ns1:PricePerUnit>78.00</ns1:PricePerUnit>
                                 <ns1:Price>66.30</ns1:Price>
                              </ns1:Work>
                           </ns1:Works>
                        </ns1:LabourCosts>
                        <ns1:LacquerCosts>
                           <ns1:Wage>
                              <ns1:Type>LACQUER WORK</ns1:Type>
                              <ns1:Units>13.59</ns1:Units>
                              <ns1:PricePerUnit>120.00</ns1:PricePerUnit>
                              <ns1:Price>1630.80</ns1:Price>
                           </ns1:Wage>
                           <ns1:TotalWages>1630.80</ns1:TotalWages>
                           <ns1:Material>
                              <ns1:FlatPercentage>25.0</ns1:FlatPercentage>
                              <ns1:FlatAmount>407.70</ns1:FlatAmount>
                              <ns1:MaterialGroups/>
                              <ns1:TotalSum>407.70</ns1:TotalSum>
                              <ns1:SumMaterialCorrected>407.70</ns1:SumMaterialCorrected>
                           </ns1:Material>
                           <ns1:TotalSum>2038.50</ns1:TotalSum>
                        </ns1:LacquerCosts>
                        <ns1:TotalNetCosts>4141.28</ns1:TotalNetCosts>
                        <ns1:TotalVAT>786.84</ns1:TotalVAT>
                        <ns1:TotalGrossCosts>4928.12</ns1:TotalGrossCosts>
                        <ns1:TotalNetCorrected>4141.28</ns1:TotalNetCorrected>
                        <ns1:TotalVATCorrected>786.84</ns1:TotalVATCorrected>
                        <ns1:TotalGrossCorrected>4928.12</ns1:TotalGrossCorrected>
                        <ns1:SumNet>4141.28</ns1:SumNet>
                        <ns1:SumGross>4928.12</ns1:SumGross>
                        <ns1:SumSparePartCosts>1017.20</ns1:SumSparePartCosts>
                        <ns1:SumSmallSparePartCosts>20.34</ns1:SumSmallSparePartCosts>
                        <ns1:SumMiscellaneousCosts>300.00</ns1:SumMiscellaneousCosts>
                        <ns1:SumLabourCosts>765.24</ns1:SumLabourCosts>
                        <ns1:MetaPositions>
                           <ns1:MetaPosition key="TIME_UNIT_SYSTEM" value="STD"/>
                           <ns1:MetaPosition key="LACQUER_TIME_UNIT_SYSTEM" value="STD"/>
                           <ns1:MetaPosition key="DAT_EUROLACQUER_IN_HOURS" value="false"/>
                           <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EQUIPMENT" value="false"/>
                           <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EXTENSION" value="false"/>
                           <ns1:MetaPosition key="FLAT_PERCENTAGE_BASE" value="1290.00"/>
                        </ns1:MetaPositions>
                     </ns1:RepairCalculationSummary>
                  </ns1:CalcResultExtension>
                  <ns1:CalculationSummary>
                     <ns1:SparePartsCosts>
                        <ns1:AllSum>1017.20</ns1:AllSum>
                        <ns1:ConsumablesSurcharge>20.34</ns1:ConsumablesSurcharge>
                        <ns1:ConsumablesSurchargePercentage>2.00</ns1:ConsumablesSurchargePercentage>
                        <ns1:TotalSum>1037.54</ns1:TotalSum>
                     </ns1:SparePartsCosts>
                     <ns1:AuxiliaryCosts>
                        <ns1:AuxiliaryCosts>300.00</ns1:AuxiliaryCosts>
                        <ns1:TotalSum>300.00</ns1:TotalSum>
                     </ns1:AuxiliaryCosts>
                     <ns1:LabourCosts>
                        <ns1:AllSum>660.24</ns1:AllSum>
                        <ns1:Bodywork>
                           <ns1:Type>CAR BODY</ns1:Type>
                           <ns1:Units>4.26</ns1:Units>
                           <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                           <ns1:Price>447.30</ns1:Price>
                        </ns1:Bodywork>
                        <ns1:Electric>
                           <ns1:Type>ELECTRICS</ns1:Type>
                           <ns1:Units>0</ns1:Units>
                           <ns1:Price>0</ns1:Price>
                        </ns1:Electric>
                        <ns1:Mechanic>
                           <ns1:Type>MECHANICS</ns1:Type>
                           <ns1:Units>0</ns1:Units>
                           <ns1:Price>0</ns1:Price>
                        </ns1:Mechanic>
                        <ns1:DentsPress>
                           <ns1:Type>HAIL DAMAGE PRESS</ns1:Type>
                           <ns1:Units>1.88</ns1:Units>
                           <ns1:PricePerUnit>78.00</ns1:PricePerUnit>
                           <ns1:Price>146.64</ns1:Price>
                        </ns1:DentsPress>
                        <ns1:DentsGlobal>
                           <ns1:Type>HAIL DAMAGE GENERAL</ns1:Type>
                           <ns1:Units>0.85</ns1:Units>
                           <ns1:PricePerUnit>78.00</ns1:PricePerUnit>
                           <ns1:Price>66.30</ns1:Price>
                        </ns1:DentsGlobal>
                        <ns1:TotalSum>660.24</ns1:TotalSum>
                        <ns1:Wages/>
                        <ns1:Works>
                           <ns1:Work>
                              <ns1:Type>CAR BODY</ns1:Type>
                              <ns1:WageLevel>1</ns1:WageLevel>
                              <ns1:Units>4.26</ns1:Units>
                              <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                              <ns1:Price>447.30</ns1:Price>
                           </ns1:Work>
                           <ns1:Work>
                              <ns1:Type>HAIL DAMAGE PRESS</ns1:Type>
                              <ns1:Units>1.88</ns1:Units>
                              <ns1:PricePerUnit>78.00</ns1:PricePerUnit>
                              <ns1:Price>146.64</ns1:Price>
                           </ns1:Work>
                           <ns1:Work>
                              <ns1:Type>HAIL DAMAGE GENERAL</ns1:Type>
                              <ns1:Units>0.85</ns1:Units>
                              <ns1:PricePerUnit>78.00</ns1:PricePerUnit>
                              <ns1:Price>66.30</ns1:Price>
                           </ns1:Work>
                        </ns1:Works>
                     </ns1:LabourCosts>
                     <ns1:LacquerCosts>
                        <ns1:Wage>
                           <ns1:Type>LACQUER WORK</ns1:Type>
                           <ns1:Units>10.75</ns1:Units>
                           <ns1:PricePerUnit>120.00</ns1:PricePerUnit>
                           <ns1:Price>1290.00</ns1:Price>
                        </ns1:Wage>
                        <ns1:TotalWages>1290.00</ns1:TotalWages>
                        <ns1:Material>
                           <ns1:FlatPercentage>25.0</ns1:FlatPercentage>
                           <ns1:FlatAmount>322.50</ns1:FlatAmount>
                           <ns1:MaterialGroups/>
                           <ns1:TotalSum>322.50</ns1:TotalSum>
                           <ns1:SumMaterialCorrected>322.50</ns1:SumMaterialCorrected>
                        </ns1:Material>
                        <ns1:TotalSum>1612.50</ns1:TotalSum>
                     </ns1:LacquerCosts>
                     <ns1:TotalNetCosts>3610.28</ns1:TotalNetCosts>
                     <ns1:TotalVAT>685.95</ns1:TotalVAT>
                     <ns1:TotalGrossCosts>4296.23</ns1:TotalGrossCosts>
                     <ns1:TotalNetCorrected>3610.28</ns1:TotalNetCorrected>
                     <ns1:TotalVATCorrected>685.95</ns1:TotalVATCorrected>
                     <ns1:TotalGrossCorrected>4296.23</ns1:TotalGrossCorrected>
                     <ns1:SumNet>3610.28</ns1:SumNet>
                     <ns1:SumGross>4296.23</ns1:SumGross>
                     <ns1:SumSparePartCosts>1017.20</ns1:SumSparePartCosts>
                     <ns1:SumSmallSparePartCosts>20.34</ns1:SumSmallSparePartCosts>
                     <ns1:SumMiscellaneousCosts>300.00</ns1:SumMiscellaneousCosts>
                     <ns1:SumLabourCosts>660.24</ns1:SumLabourCosts>
                     <ns1:MetaPositions>
                        <ns1:MetaPosition key="TIME_UNIT_SYSTEM" value="STD"/>
                        <ns1:MetaPosition key="LACQUER_TIME_UNIT_SYSTEM" value="STD"/>
                        <ns1:MetaPosition key="DAT_EUROLACQUER_IN_HOURS" value="false"/>
                        <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EQUIPMENT" value="false"/>
                        <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EXTENSION" value="false"/>
                        <ns1:MetaPosition key="FLAT_PERCENTAGE_BASE" value="1290.00"/>
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
                  <ns1:OrderNumber>20231222092039260</ns1:OrderNumber>
                  <ns1:InvoiceDate>2023-12-22T09:20:40.930+01:00</ns1:InvoiceDate>
               </ns1:RepairOrder>
               <ns1:InsuranceClaim>false</ns1:InsuranceClaim>
               <ns1:ProcessManagement/>
            </ns1:Dossier>
         </calculationResult>
      </ns3:calculateNResponse>
   </S:Body>
</S:Envelope>
