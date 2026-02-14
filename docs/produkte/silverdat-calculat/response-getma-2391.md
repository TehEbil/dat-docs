---
title: "Response getMaintenanceIntervals"
topic_id: "2391"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abruf von Wartungsintervallen: getMaintenanceIntervals > Response getMaintenanceIntervals"
---

# Response getMaintenanceIntervals

<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns3:getMaintenanceIntervalsResponse xmlns:ns3="http://sphinx.dat.de/services/VehicleRepairService">
         <maintenance source="SD3" type="VehicleRepairOnline">
            <ns1:Dossier xmlns:ns1="http://www.dat.de/vxs">
               <ns1:UUID>69c6fd33-2a6a-4563-a61b-608b4ad48125</ns1:UUID>
               <ns1:Country>DE</ns1:Country>
               <ns1:Language>de_DE</ns1:Language>
               <ns1:DataVersion>1</ns1:DataVersion>
               <ns1:Currency>EUR</ns1:Currency>
               <ns1:DatCustomerId>9999999</ns1:DatCustomerId>
               <ns1:DossierType>repair</ns1:DossierType>
               <ns1:CreateDate>2023-12-22T14:03:05.542+01:00</ns1:CreateDate>
               <ns1:CreateUser>Anwender</ns1:CreateUser>
               <ns1:ChangeDate>2023-12-22T14:03:05.542+01:00</ns1:ChangeDate>
               <ns1:DatCustomerAddress>
                  <ns1:Title>titleCompany</ns1:Title>
                  <ns1:CompanyName>DAT - Intern</ns1:CompanyName>
                  <ns1:NameLong>Schulung SST-Partner</ns1:NameLong>
                  <ns1:Country>DE</ns1:Country>
                  <ns1:CustomerNumber>9999999</ns1:CustomerNumber>
                  <ns1:CustomerType>9999999</ns1:CustomerType>
                  <ns1:Street>Hellmuth-Hirth-Str.</ns1:Street>
                  <ns1:StreetNumber>1</ns1:StreetNumber>
                  <ns1:StreetZipCode>73760</ns1:StreetZipCode>
                  <ns1:StreetCity>Ostfildern</ns1:StreetCity>
                  <ns1:EMail>kundendienst@dat.de</ns1:EMail>
                  <ns1:PhoneBusiness>+49 711/450000</ns1:PhoneBusiness>
                  <ns1:UsageFlag>9</ns1:UsageFlag>
               </ns1:DatCustomerAddress>
               <ns1:Vehicle>
                  <ns1:DatECode>011301110300002</ns1:DatECode>
                  <ns1:ConstructionTime>5297</ns1:ConstructionTime>
                  <ns1:VehicleTypeName origin="dat">Pkw, SUV, Kleintransporter</ns1:VehicleTypeName>
                  <ns1:VehicleTypeNameN origin="dat">Pkw, SUV, Kleintransporter</ns1:VehicleTypeNameN>
                  <ns1:ManufacturerName origin="dat">BMW</ns1:ManufacturerName>
                  <ns1:BaseModelName origin="dat">Baureihe 5 Touring (F11)(2010->)</ns1:BaseModelName>
                  <ns1:SubModelName origin="dat">520d</ns1:SubModelName>
                  <ns1:VehicleType>1</ns1:VehicleType>
                  <ns1:Manufacturer>130</ns1:Manufacturer>
                  <ns1:BaseModel>111</ns1:BaseModel>
                  <ns1:SubModel>30</ns1:SubModel>
                  <ns1:Country>DE</ns1:Country>
                  <ns1:SubModelVariant>2</ns1:SubModelVariant>
                  <ns1:RegistrationData/>
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
                     <ns1:ProductGroupName/>
                     <ns1:TechInfoWltp/>
                  </ns1:TechInfo>
                  <ns1:Equipment>
                     <ns1:SeriesEquipment>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>10715</ns1:DatEquipmentId>
                           <ns1:Description>Aktive Motorhaube</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>11406</ns1:DatEquipmentId>
                           <ns1:Description>Exterieurumfänge Wagenfarbe</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
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
                           <ns1:DatEquipmentId>18505</ns1:DatEquipmentId>
                           <ns1:Description>Bi-Xenon-Scheinwerfer</ns1:Description>
                           <ns1:EquipmentGroup>XELI</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>18913</ns1:DatEquipmentId>
                                 <ns1:Description>Tagfahrlicht LED</ns1:Description>
                                 <ns1:EquipmentGroup>TFAL</ns1:EquipmentGroup>
                                 <ns1:EquipmentType>glass</ns1:EquipmentType>
                                 <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>19000</ns1:DatEquipmentId>
                                 <ns1:Description>Scheinwerfer-Reinigungsanlage (SRA)</ns1:Description>
                                 <ns1:EquipmentGroup>SWRA</ns1:EquipmentGroup>
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
                           <ns1:DatEquipmentId>18604</ns1:DatEquipmentId>
                           <ns1:Description>Automatische Fahrlichtschaltung</ns1:Description>
                           <ns1:EquipmentGroup>AUFL</ns1:EquipmentGroup>
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
                           <ns1:DatEquipmentId>19101</ns1:DatEquipmentId>
                           <ns1:Description>Scheibenwischer mit Regensensor</ns1:Description>
                           <ns1:EquipmentGroup>SWRE</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>19102</ns1:DatEquipmentId>
                           <ns1:Description>Scheibenwaschdüsen heizbar</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>19300</ns1:DatEquipmentId>
                           <ns1:Description>Heckscheibenwischer</ns1:Description>
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
                           <ns1:DatEquipmentId>24115</ns1:DatEquipmentId>
                           <ns1:Description>Audiosystem BMW Professional (Radio/CD-Player MP3-fähig)</ns1:Description>
                           <ns1:EquipmentGroup>CD</ns1:EquipmentGroup>
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
                           <ns1:DatEquipmentId>24999</ns1:DatEquipmentId>
                           <ns1:Description>AUX-IN-Anschluss (AUX-IN)</ns1:Description>
                           <ns1:EquipmentGroup>MP3A</ns1:EquipmentGroup>
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
                           <ns1:DatEquipmentId>25300</ns1:DatEquipmentId>
                           <ns1:Description>Drehzahlmesser</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25508</ns1:DatEquipmentId>
                           <ns1:Description>Bordcomputer</ns1:Description>
                           <ns1:EquipmentGroup>COMP</ns1:EquipmentGroup>
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
                           <ns1:DatEquipmentId>25702</ns1:DatEquipmentId>
                           <ns1:Description>Außentemperaturanzeige</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
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
                           <ns1:DatEquipmentId>25924</ns1:DatEquipmentId>
                           <ns1:Description>Control-Display mit Farbmonitor (6,5 Zoll)</ns1:Description>
                           <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26302</ns1:DatEquipmentId>
                           <ns1:Description>Innenausstattung: Interieurleisten, schwarz hochglänzend</ns1:Description>
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
                           <ns1:DatEquipmentId>26803</ns1:DatEquipmentId>
                           <ns1:Description>Airbag Fahrer-/Beifahrerseite</ns1:Description>
                           <ns1:EquipmentGroup>AIR1</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26804</ns1:DatEquipmentId>
                           <ns1:Description>Kopf-Airbag-System vorn</ns1:Description>
                           <ns1:EquipmentGroup>AIR4</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26805</ns1:DatEquipmentId>
                           <ns1:Description>Kopf-Airbag-System hinten</ns1:Description>
                           <ns1:EquipmentGroup>AIR4</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26903</ns1:DatEquipmentId>
                           <ns1:Description>Seitenairbag vorn</ns1:Description>
                           <ns1:EquipmentGroup>AIR3</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26909</ns1:DatEquipmentId>
                           <ns1:Description>Airbag Beifahrerseite abschaltbar</ns1:Description>
                           <ns1:EquipmentGroup>AIR2</ns1:EquipmentGroup>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27202</ns1:DatEquipmentId>
                           <ns1:Description>Mittelarmlehne vorn</ns1:Description>
                           <ns1:EquipmentGroup>MALV</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27300</ns1:DatEquipmentId>
                           <ns1:Description>Mittelarmlehne hinten</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27309</ns1:DatEquipmentId>
                           <ns1:Description>Multifunktionsarmlehne im Fond</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27400</ns1:DatEquipmentId>
                           <ns1:Description>Gepäckraumabdeckung / Rollo</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27605</ns1:DatEquipmentId>
                           <ns1:Description>Gepäckraum-Abtrennung (Netz)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>28402</ns1:DatEquipmentId>
                           <ns1:Description>Fußmatten Velours</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>29003</ns1:DatEquipmentId>
                           <ns1:Description>Klimaautomatik 2-Zonen</ns1:Description>
                           <ns1:EquipmentGroup>KLI2</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>30470</ns1:DatEquipmentId>
                           <ns1:Description>Sitzbezug / Polsterung: Stoff Diagonal</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>32811</ns1:DatEquipmentId>
                           <ns1:Description>Sitze vorn teilelektr. verstellbar</ns1:Description>
                           <ns1:EquipmentGroup>SITE</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>33508</ns1:DatEquipmentId>
                           <ns1:Description>Rücksitzlehne geteilt/klappbar</ns1:Description>
                           <ns1:EquipmentGroup>SITH</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>34704</ns1:DatEquipmentId>
                           <ns1:Description>Aktive Kopfstützen</ns1:Description>
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
                           <ns1:DatEquipmentId>35301</ns1:DatEquipmentId>
                           <ns1:Description>Zentralverriegelung mit Fernbedienung</ns1:Description>
                           <ns1:EquipmentGroup>ZV</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35408</ns1:DatEquipmentId>
                           <ns1:Description>Soft-Close-Automatik für Kofferraum / Heckklappe</ns1:Description>
                           <ns1:EquipmentGroup>HKEL</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35506</ns1:DatEquipmentId>
                           <ns1:Description>Heckklappenbetätigung automatisch</ns1:Description>
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
                           <ns1:DatEquipmentId>38105</ns1:DatEquipmentId>
                           <ns1:Description>Wegfahrsperre</ns1:Description>
                           <ns1:EquipmentGroup>WFS</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39016</ns1:DatEquipmentId>
                           <ns1:Description>Steckdose (12V-Anschluß) 3-fach</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39308</ns1:DatEquipmentId>
                           <ns1:Description>Isofix-Aufnahmen für Kindersitz an Rücksitz</ns1:Description>
                           <ns1:EquipmentGroup>KISI</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39402</ns1:DatEquipmentId>
                           <ns1:Description>Getränkehalter vorn und hinten</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40000</ns1:DatEquipmentId>
                           <ns1:Description>Anti-Blockier-System (ABS)</ns1:Description>
                           <ns1:EquipmentGroup>ABS</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40050</ns1:DatEquipmentId>
                           <ns1:Description>Bremsenergierückgewinnung (Rekuperationssystem)</ns1:Description>
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
                           <ns1:DatEquipmentId>40803</ns1:DatEquipmentId>
                           <ns1:Description>Parkbremse elektrisch</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>42805</ns1:DatEquipmentId>
                           <ns1:Description>Niveauregulierung</ns1:Description>
                           <ns1:EquipmentGroup>NIV</ns1:EquipmentGroup>
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
                           <ns1:DatEquipmentId>48535</ns1:DatEquipmentId>
                           <ns1:Description>LM-Felgen 8x17 (V-Speiche 236)</ns1:Description>
                           <ns1:EquipmentGroup>ALU</ns1:EquipmentGroup>
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
                           <ns1:DatEquipmentId>69811</ns1:DatEquipmentId>
                           <ns1:Description>Servolenkung Servotronic</ns1:Description>
                           <ns1:EquipmentGroup>SL</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>70100</ns1:DatEquipmentId>
                           <ns1:Description>Dynamische Stabilitäts-Control (DSC)</ns1:Description>
                           <ns1:EquipmentGroup>ESP</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>70518</ns1:DatEquipmentId>
                           <ns1:Description>Fahrassistenz-System: Fahrerlebnisschalter</ns1:Description>
                           <ns1:EquipmentGroup>FA22</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>73017</ns1:DatEquipmentId>
                           <ns1:Description>Vlies-Batterie 80 Ah (AGM)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>77015</ns1:DatEquipmentId>
                           <ns1:Description>NOx-Speicherkatalysator (BMW Blue Performance)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>77227</ns1:DatEquipmentId>
                           <ns1:Description>Schadstoffarm nach Abgasnorm Euro 6</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>77601</ns1:DatEquipmentId>
                           <ns1:Description>Start/Stop-Anlage (Funktion)</ns1:Description>
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
                           <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                           <ns1:Description>Karosserie: 5-türig</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
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
                           <ns1:DatEquipmentId>19000</ns1:DatEquipmentId>
                           <ns1:Description>Scheinwerfer-Reinigungsanlage (SRA)</ns1:Description>
                           <ns1:EquipmentGroup>SWRA</ns1:EquipmentGroup>
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
                           <ns1:DatEquipmentId>75205</ns1:DatEquipmentId>
                           <ns1:Description>Getriebe 6-Gang</ns1:Description>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25699</ns1:DatEquipmentId>
                           <ns1:Description>Schaltpunktanzeige</ns1:Description>
                        </ns1:EquipmentPosition>
                     </ns1:DeselectedSeriesEquipment>
                     <ns1:SpecialEquipment>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>75914</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Getriebe Automatik - mit Steptronic (8-Stufen)</ns1:Description>
                           <ns1:EquipmentGroup>AG2</ns1:EquipmentGroup>
                           <ns1:GearBoxType>automatic</ns1:GearBoxType>
                           <ns1:NrOfGears>8</ns1:NrOfGears>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                     </ns1:SpecialEquipment>
                  </ns1:Equipment>
                  <ns1:Tires>
                     <ns1:Axles/>
                  </ns1:Tires>
               </ns1:Vehicle>
               <ns1:VAT>
                  <ns1:VatAtCalculationTime>19</ns1:VatAtCalculationTime>
               </ns1:VAT>
               <ns1:TradingData>
                  <ns1:ClientContactAddresses>
                     <ns1:ClientContactAddress>
                        <ns1:Title>titleCompany</ns1:Title>
                        <ns1:CompanyName>DAT - Intern</ns1:CompanyName>
                        <ns1:NameLong>Schulung SST-Partner</ns1:NameLong>
                        <ns1:Country>DE</ns1:Country>
                        <ns1:CustomerNumber>9999999</ns1:CustomerNumber>
                        <ns1:CustomerType>9999999</ns1:CustomerType>
                        <ns1:Street>Hellmuth-Hirth-Str.</ns1:Street>
                        <ns1:StreetNumber>1</ns1:StreetNumber>
                        <ns1:StreetZipCode>73760</ns1:StreetZipCode>
                        <ns1:StreetCity>Ostfildern</ns1:StreetCity>
                        <ns1:EMail>kundendienst@dat.de</ns1:EMail>
                        <ns1:PhoneBusiness>+49 711/45000</ns1:PhoneBusiness>
                        <ns1:UsageFlag>9</ns1:UsageFlag>
                     </ns1:ClientContactAddress>
                  </ns1:ClientContactAddresses>
               </ns1:TradingData>
               <ns1:RepairCalculation>
                  <ns1:Vehicle>
                     <ns1:DatECode>011301110300002</ns1:DatECode>
                     <ns1:ConstructionTime>5297</ns1:ConstructionTime>
                     <ns1:VehicleTypeName origin="dat">Pkw, SUV, Kleintransporter</ns1:VehicleTypeName>
                     <ns1:VehicleTypeNameN origin="dat">Pkw, SUV, Kleintransporter</ns1:VehicleTypeNameN>
                     <ns1:ManufacturerName origin="dat">BMW</ns1:ManufacturerName>
                     <ns1:BaseModelName origin="dat">Baureihe 5 Touring (F11)(2010->)</ns1:BaseModelName>
                     <ns1:SubModelName origin="dat">520d</ns1:SubModelName>
                     <ns1:VehicleType>1</ns1:VehicleType>
                     <ns1:Manufacturer>130</ns1:Manufacturer>
                     <ns1:BaseModel>111</ns1:BaseModel>
                     <ns1:SubModel>30</ns1:SubModel>
                     <ns1:Country>DE</ns1:Country>
                     <ns1:SubModelVariant>2</ns1:SubModelVariant>
                     <ns1:RegistrationData/>
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
                        <ns1:ProductGroupName/>
                        <ns1:TechInfoWltp/>
                     </ns1:TechInfo>
                     <ns1:Equipment>
                        <ns1:SeriesEquipment>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>10715</ns1:DatEquipmentId>
                              <ns1:Description>Aktive Motorhaube</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>11406</ns1:DatEquipmentId>
                              <ns1:Description>Exterieurumfänge Wagenfarbe</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
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
                              <ns1:DatEquipmentId>18505</ns1:DatEquipmentId>
                              <ns1:Description>Bi-Xenon-Scheinwerfer</ns1:Description>
                              <ns1:EquipmentGroup>XELI</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>18913</ns1:DatEquipmentId>
                                    <ns1:Description>Tagfahrlicht LED</ns1:Description>
                                    <ns1:EquipmentGroup>TFAL</ns1:EquipmentGroup>
                                    <ns1:EquipmentType>glass</ns1:EquipmentType>
                                    <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>19000</ns1:DatEquipmentId>
                                    <ns1:Description>Scheinwerfer-Reinigungsanlage (SRA)</ns1:Description>
                                    <ns1:EquipmentGroup>SWRA</ns1:EquipmentGroup>
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
                              <ns1:DatEquipmentId>18604</ns1:DatEquipmentId>
                              <ns1:Description>Automatische Fahrlichtschaltung</ns1:Description>
                              <ns1:EquipmentGroup>AUFL</ns1:EquipmentGroup>
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
                              <ns1:DatEquipmentId>19101</ns1:DatEquipmentId>
                              <ns1:Description>Scheibenwischer mit Regensensor</ns1:Description>
                              <ns1:EquipmentGroup>SWRE</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>19102</ns1:DatEquipmentId>
                              <ns1:Description>Scheibenwaschdüsen heizbar</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>19300</ns1:DatEquipmentId>
                              <ns1:Description>Heckscheibenwischer</ns1:Description>
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
                              <ns1:DatEquipmentId>24115</ns1:DatEquipmentId>
                              <ns1:Description>Audiosystem BMW Professional (Radio/CD-Player MP3-fähig)</ns1:Description>
                              <ns1:EquipmentGroup>CD</ns1:EquipmentGroup>
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
                              <ns1:DatEquipmentId>24999</ns1:DatEquipmentId>
                              <ns1:Description>AUX-IN-Anschluss (AUX-IN)</ns1:Description>
                              <ns1:EquipmentGroup>MP3A</ns1:EquipmentGroup>
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
                              <ns1:DatEquipmentId>25300</ns1:DatEquipmentId>
                              <ns1:Description>Drehzahlmesser</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25508</ns1:DatEquipmentId>
                              <ns1:Description>Bordcomputer</ns1:Description>
                              <ns1:EquipmentGroup>COMP</ns1:EquipmentGroup>
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
                              <ns1:DatEquipmentId>25702</ns1:DatEquipmentId>
                              <ns1:Description>Außentemperaturanzeige</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
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
                              <ns1:DatEquipmentId>25924</ns1:DatEquipmentId>
                              <ns1:Description>Control-Display mit Farbmonitor (6,5 Zoll)</ns1:Description>
                              <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>26302</ns1:DatEquipmentId>
                              <ns1:Description>Innenausstattung: Interieurleisten, schwarz hochglänzend</ns1:Description>
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
                              <ns1:DatEquipmentId>26803</ns1:DatEquipmentId>
                              <ns1:Description>Airbag Fahrer-/Beifahrerseite</ns1:Description>
                              <ns1:EquipmentGroup>AIR1</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>26804</ns1:DatEquipmentId>
                              <ns1:Description>Kopf-Airbag-System vorn</ns1:Description>
                              <ns1:EquipmentGroup>AIR4</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>26805</ns1:DatEquipmentId>
                              <ns1:Description>Kopf-Airbag-System hinten</ns1:Description>
                              <ns1:EquipmentGroup>AIR4</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>26903</ns1:DatEquipmentId>
                              <ns1:Description>Seitenairbag vorn</ns1:Description>
                              <ns1:EquipmentGroup>AIR3</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>26909</ns1:DatEquipmentId>
                              <ns1:Description>Airbag Beifahrerseite abschaltbar</ns1:Description>
                              <ns1:EquipmentGroup>AIR2</ns1:EquipmentGroup>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27202</ns1:DatEquipmentId>
                              <ns1:Description>Mittelarmlehne vorn</ns1:Description>
                              <ns1:EquipmentGroup>MALV</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27300</ns1:DatEquipmentId>
                              <ns1:Description>Mittelarmlehne hinten</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27309</ns1:DatEquipmentId>
                              <ns1:Description>Multifunktionsarmlehne im Fond</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27400</ns1:DatEquipmentId>
                              <ns1:Description>Gepäckraumabdeckung / Rollo</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27605</ns1:DatEquipmentId>
                              <ns1:Description>Gepäckraum-Abtrennung (Netz)</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>28402</ns1:DatEquipmentId>
                              <ns1:Description>Fußmatten Velours</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>29003</ns1:DatEquipmentId>
                              <ns1:Description>Klimaautomatik 2-Zonen</ns1:Description>
                              <ns1:EquipmentGroup>KLI2</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>30470</ns1:DatEquipmentId>
                              <ns1:Description>Sitzbezug / Polsterung: Stoff Diagonal</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>32811</ns1:DatEquipmentId>
                              <ns1:Description>Sitze vorn teilelektr. verstellbar</ns1:Description>
                              <ns1:EquipmentGroup>SITE</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>33508</ns1:DatEquipmentId>
                              <ns1:Description>Rücksitzlehne geteilt/klappbar</ns1:Description>
                              <ns1:EquipmentGroup>SITH</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>34704</ns1:DatEquipmentId>
                              <ns1:Description>Aktive Kopfstützen</ns1:Description>
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
                              <ns1:DatEquipmentId>35301</ns1:DatEquipmentId>
                              <ns1:Description>Zentralverriegelung mit Fernbedienung</ns1:Description>
                              <ns1:EquipmentGroup>ZV</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>35408</ns1:DatEquipmentId>
                              <ns1:Description>Soft-Close-Automatik für Kofferraum / Heckklappe</ns1:Description>
                              <ns1:EquipmentGroup>HKEL</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>35506</ns1:DatEquipmentId>
                              <ns1:Description>Heckklappenbetätigung automatisch</ns1:Description>
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
                              <ns1:DatEquipmentId>38105</ns1:DatEquipmentId>
                              <ns1:Description>Wegfahrsperre</ns1:Description>
                              <ns1:EquipmentGroup>WFS</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>39016</ns1:DatEquipmentId>
                              <ns1:Description>Steckdose (12V-Anschluß) 3-fach</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>39308</ns1:DatEquipmentId>
                              <ns1:Description>Isofix-Aufnahmen für Kindersitz an Rücksitz</ns1:Description>
                              <ns1:EquipmentGroup>KISI</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>39402</ns1:DatEquipmentId>
                              <ns1:Description>Getränkehalter vorn und hinten</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>40000</ns1:DatEquipmentId>
                              <ns1:Description>Anti-Blockier-System (ABS)</ns1:Description>
                              <ns1:EquipmentGroup>ABS</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>40050</ns1:DatEquipmentId>
                              <ns1:Description>Bremsenergierückgewinnung (Rekuperationssystem)</ns1:Description>
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
                              <ns1:DatEquipmentId>40803</ns1:DatEquipmentId>
                              <ns1:Description>Parkbremse elektrisch</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>42805</ns1:DatEquipmentId>
                              <ns1:Description>Niveauregulierung</ns1:Description>
                              <ns1:EquipmentGroup>NIV</ns1:EquipmentGroup>
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
                              <ns1:DatEquipmentId>48535</ns1:DatEquipmentId>
                              <ns1:Description>LM-Felgen 8x17 (V-Speiche 236)</ns1:Description>
                              <ns1:EquipmentGroup>ALU</ns1:EquipmentGroup>
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
                              <ns1:DatEquipmentId>69811</ns1:DatEquipmentId>
                              <ns1:Description>Servolenkung Servotronic</ns1:Description>
                              <ns1:EquipmentGroup>SL</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>70100</ns1:DatEquipmentId>
                              <ns1:Description>Dynamische Stabilitäts-Control (DSC)</ns1:Description>
                              <ns1:EquipmentGroup>ESP</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>70518</ns1:DatEquipmentId>
                              <ns1:Description>Fahrassistenz-System: Fahrerlebnisschalter</ns1:Description>
                              <ns1:EquipmentGroup>FA22</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>73017</ns1:DatEquipmentId>
                              <ns1:Description>Vlies-Batterie 80 Ah (AGM)</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>77015</ns1:DatEquipmentId>
                              <ns1:Description>NOx-Speicherkatalysator (BMW Blue Performance)</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>77227</ns1:DatEquipmentId>
                              <ns1:Description>Schadstoffarm nach Abgasnorm Euro 6</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>77601</ns1:DatEquipmentId>
                              <ns1:Description>Start/Stop-Anlage (Funktion)</ns1:Description>
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
                              <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                              <ns1:Description>Karosserie: 5-türig</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
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
                              <ns1:DatEquipmentId>19000</ns1:DatEquipmentId>
                              <ns1:Description>Scheinwerfer-Reinigungsanlage (SRA)</ns1:Description>
                              <ns1:EquipmentGroup>SWRA</ns1:EquipmentGroup>
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
                              <ns1:DatEquipmentId>75205</ns1:DatEquipmentId>
                              <ns1:Description>Getriebe 6-Gang</ns1:Description>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25699</ns1:DatEquipmentId>
                              <ns1:Description>Schaltpunktanzeige</ns1:Description>
                           </ns1:EquipmentPosition>
                        </ns1:DeselectedSeriesEquipment>
                        <ns1:SpecialEquipment>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>75914</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Getriebe Automatik - mit Steptronic (8-Stufen)</ns1:Description>
                              <ns1:EquipmentGroup>AG2</ns1:EquipmentGroup>
                              <ns1:GearBoxType>automatic</ns1:GearBoxType>
                              <ns1:NrOfGears>8</ns1:NrOfGears>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                        </ns1:SpecialEquipment>
                     </ns1:Equipment>
                     <ns1:Tires>
                        <ns1:Axles/>
                     </ns1:Tires>
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
                     <ns1:ProcedureRelatedParameter attribute="selectedLacquerMethod" factor="CalculationFactor" type="LacquerMethod">EURO_LACQUER</ns1:ProcedureRelatedParameter>
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
                     <ns1:ProcedureRelatedParameter attribute="dentWage" factor="LabourCostFactor" mode="PER_HOUR" type="Price">100.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="mechanicWage1" factor="LabourCostFactor" mode="PER_HOUR" type="Price">100.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="electricWage1" factor="LabourCostFactor" mode="PER_HOUR" type="Price">100.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnit" factor="LabourCostFactor" type="TimeUnitSystem">HOUR</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="LabourCostFactor" type="Integer">1</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="bodyWage1" factor="LabourCostFactor" mode="PER_HOUR" type="Price">100.0</ns1:ProcedureRelatedParameter>
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
                     <ns1:ProcedureRelatedParameter attribute="materialMode" factor="ManufacturerLacquerFactor" type="LacquerMaterialMode">LACQUER_METHOD</ns1:ProcedureRelatedParameter>
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
                  <ns1:CalculationSummary>
                     <ns1:SparePartsCosts/>
                     <ns1:AuxiliaryCosts/>
                     <ns1:LabourCosts>
                        <ns1:AllSum>0</ns1:AllSum>
                        <ns1:Bodywork>
                           <ns1:Type>CAR BODY</ns1:Type>
                           <ns1:Units>0</ns1:Units>
                           <ns1:Price>0</ns1:Price>
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
                        <ns1:TotalSum>0</ns1:TotalSum>
                        <ns1:Wages/>
                        <ns1:Works/>
                     </ns1:LabourCosts>
                     <ns1:LacquerCosts>
                        <ns1:Material/>
                     </ns1:LacquerCosts>
                     <ns1:MetaPositions>
                        <ns1:MetaPosition key="TIME_UNIT_SYSTEM" value="STD"/>
                        <ns1:MetaPosition key="LACQUER_TIME_UNIT_SYSTEM" value="STD"/>
                        <ns1:MetaPosition key="DAT_EUROLACQUER_IN_HOURS" value="false"/>
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
                  <ns1:InvoiceDate>2023-12-22T14:03:05.618+01:00</ns1:InvoiceDate>
               </ns1:RepairOrder>
               <ns1:MaintenanceIntervals>
                  <ns1:MaintenanceInterval>
                     <ns1:Description>BEDARFSORIENTIERTER SERVICE STANDARDUMFANG</ns1:Description>
                     <ns1:DATProcessId>94802</ns1:DATProcessId>
                     <ns1:MaintenancePositions>
                        <ns1:MaintenancePosition>
                           <ns1:Description>HINWEIS: Unter bestimmten örtlichen Bedingungen kann es erforderlich sein, bestimmte Servicearbeiten früher auszuführen.</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Service Standardumfang: Check-Control-Meldungen und Kontroll- und Warnleuchten kontrollieren, ggf. Schiebedachführungsschienen auf Verschmutzung prüfen, Feststellbremse prüfen ohne Prüfstand</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Service-Intervallanzeige nach Werksvorschrift zurückstellen und Wartungsumfänge in elektronische Servicehistorie eintragen</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>ZUSATZARBEITEN</ns1:Description>
                           <ns1:PositionType>G</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>98020</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Service Motoröl: Motoröl und Ölfilter wechseln (Motorölfreigabelisten beachten)</ns1:Description>
                           <ns1:FootNote>- alle 30.000 Km oder alle 24 Monate
- Serviceanzeige nach Werksvorschrift zurücksetzen und Wartungsumfang in elektronische Servicehistorie eintragen</ns1:FootNote>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>81200</ns1:DATProcessId>
                                 <ns1:Description>OELFILTER EINSATZ</ns1:Description>
                              </ns1:MaterialPosition>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>99031</ns1:DATProcessId>
                                 <ns1:Description>MOTOROEL</ns1:Description>
                                 <ns1:ManualPriceRequired>true</ns1:ManualPriceRequired>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>64230</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Service Bremse v: Bremsbeläge und Bremsbelagfühler v. wechseln, Bremsschächte reinigen. Bremsscheiben: Oberfläche und Dicke kontrollieren</ns1:Description>
                           <ns1:FootNote>- Serviceanzeige nach Werksvorschrift zurücksetzen und Wartungsumfang in elektronische Servicehistorie eintragen</ns1:FootNote>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>64230</ns1:DATProcessId>
                                 <ns1:Description>REP.-SATZ BREMSBELAEGE V.</ns1:Description>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>75630</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Service Bremse h: Bremsbeläge und Bremsbelagfühler h. wechseln, Bremsschächte reinigen. Bremsscheiben: Oberfläche und Dicke kontrollieren. Feststellbremse Funktionsprüfung auf Rollenprüfstand</ns1:Description>
                           <ns1:FootNote>- Serviceanzeige nach Werksvorschrift zurücksetzen und Wartungsumfang in elektronische Servicehistorie eintragen</ns1:FootNote>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>75630</ns1:DATProcessId>
                                 <ns1:Description>REP.-SATZ BREMSBELAEGE H.</ns1:Description>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>75980</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Service Bremsflüssigkeit: Bremsflüssigkeit wechseln, Aktives Fußgängerschutzsystem, Haltbarkeitsdatum der Gasdruckfedern Motorhaube prüfen. Haltbarkeit muß nächsten Service erreichen.</ns1:Description>
                           <ns1:FootNote>- alle 24 Monate
- Aktives Fußgängerschutzsystem: Ohne Aufdruck Haltbarkeitsdatum. Ausgehend vom Produktionsdatum Kfz. Gasdruckfedern Frontklappe alle 5 Jahre ersetzen. Serviceanzeige zurücksetzen und Wartungsumfang in elektronische Servicehistorie eintragen</ns1:FootNote>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>99035</ns1:DATProcessId>
                                 <ns1:Description>BREMSFLUESSIGKEIT</ns1:Description>
                                 <ns1:ManualPriceRequired>true</ns1:ManualPriceRequired>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>42847</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Aktives Fußgängerschutzsystem: Gasdruckfeder der Motorhaube wechseln links</ns1:Description>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>42847</ns1:DATProcessId>
                                 <ns1:Description>GASDRUCKFEDER AKTIV FRONTKLAPPE L.</ns1:Description>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>42848</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Aktives Fußgängerschutzsystem: Gasdruckfeder der Motorhaube wechseln rechts</ns1:Description>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>42848</ns1:DATProcessId>
                                 <ns1:Description>GASDRUCKFEDER AKTIV FRONTKLAPPE R.</ns1:Description>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>10040</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Service Mikrofilter: Zusatzarbeiten bei jedem  Motorölwechsel (Mikro- / Aktivkohlefilter wechseln).Bei größerem Staubanfall Wechselintervall verkürzen</ns1:Description>
                           <ns1:FootNote>- alle 30.000 Km oder alle 24 Monate
- Serviceanzeige nach Werksvorschrift zurücksetzen und Wartungsumfang in elektronische Servicehistorie eintragen</ns1:FootNote>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>10040</ns1:DATProcessId>
                                 <ns1:Description>SATZ MIKROFILTER / AKTIVKOHLEFILTER</ns1:Description>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>83112</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Service Luftfiltereinsatz: Zusatzarbeiten bei jedem 2. Motorölwechsel (Luftfiltereinsatz ersetzen).Bei größerem Staubanfall Wechselintervall verkürzen</ns1:Description>
                           <ns1:FootNote>- alle 60.000 Km oder alle 48 Monate
- Serviceanzeige nach Werksvorschrift zurücksetzen und Wartungsumfang in elektronische Servicehistorie eintragen</ns1:FootNote>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>83112</ns1:DATProcessId>
                                 <ns1:Description>LUFTFILTEREINSATZ</ns1:Description>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>83350</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Service Kraftstofffilter: Zusatzarbeiten bei jedem 2. Motorölwechsel (Kraftstoffhauptfilter ersetzen).Bei schlechter Kraftstoffqualität Wechselintervall verkürzen</ns1:Description>
                           <ns1:FootNote>- alle 60.000 Km oder alle 48 Monate
- Serviceanzeige nach Werksvorschrift zurücksetzen und Wartungsumfang in elektronische Servicehistorie eintragen</ns1:FootNote>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>83350</ns1:DATProcessId>
                                 <ns1:Description>KRAFTST.-FILTER</ns1:Description>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Optionale Erweiterung: Wechseln der Wischerblätter mit Kundenabsprache</ns1:Description>
                           <ns1:PositionType>Z</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>45210</ns1:DATProcessId>
                                 <ns1:Description>SATZ WISCHERBLAETTER</ns1:Description>
                              </ns1:MaterialPosition>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>55211</ns1:DATProcessId>
                                 <ns1:Description>WISCHERBLATT HECKSCHEIBE</ns1:Description>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>94901</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Hauptuntersuchung (HU)</ns1:Description>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>94901</ns1:DATProcessId>
                                 <ns1:Description>HAUPTUNTERSUCHUNG (HU)</ns1:Description>
                                 <ns1:ManualPriceRequired>true</ns1:ManualPriceRequired>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>94922</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Abgasuntersuchung (AU) mit OBD-Daten (ON-BOARD-DIAGNOSE) und Endrohrmessung</ns1:Description>
                           <ns1:PositionType>R</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>94903</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Hauptuntersuchung (HU) mit Abgasuntersuchung (AU)</ns1:Description>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>94903</ns1:DATProcessId>
                                 <ns1:Description>HAUPTUNTERSUCHUNG (HU) MIT ABGASUNTERSUCHUNG (AU)</ns1:Description>
                                 <ns1:ManualPriceRequired>true</ns1:ManualPriceRequired>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>KLEINMATERIAL</ns1:Description>
                           <ns1:PositionType>G</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>99100</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Ggf. zusätzlich benötigte Kleinmaterialien</ns1:Description>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>99012</ns1:DATProcessId>
                                 <ns1:Description>GLUEHLAMPEN NORMAL</ns1:Description>
                                 <ns1:ManualPriceRequired>true</ns1:ManualPriceRequired>
                              </ns1:MaterialPosition>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>99013</ns1:DATProcessId>
                                 <ns1:Description>GLUEHLAMPEN HALOGEN</ns1:Description>
                                 <ns1:ManualPriceRequired>true</ns1:ManualPriceRequired>
                              </ns1:MaterialPosition>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>99030</ns1:DATProcessId>
                                 <ns1:Description>FROSTSCHUTZMITTEL</ns1:Description>
                                 <ns1:ManualPriceRequired>true</ns1:ManualPriceRequired>
                              </ns1:MaterialPosition>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>99032</ns1:DATProcessId>
                                 <ns1:Description>GETRIEBEOEL</ns1:Description>
                                 <ns1:ManualPriceRequired>true</ns1:ManualPriceRequired>
                              </ns1:MaterialPosition>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>99033</ns1:DATProcessId>
                                 <ns1:Description>HYDRAULIKOEL</ns1:Description>
                                 <ns1:ManualPriceRequired>true</ns1:ManualPriceRequired>
                              </ns1:MaterialPosition>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>99034</ns1:DATProcessId>
                                 <ns1:Description>SCHEIBENREINIGER</ns1:Description>
                                 <ns1:ManualPriceRequired>true</ns1:ManualPriceRequired>
                              </ns1:MaterialPosition>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>99039</ns1:DATProcessId>
                                 <ns1:Description>REINIGER</ns1:Description>
                                 <ns1:ManualPriceRequired>true</ns1:ManualPriceRequired>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                     </ns1:MaintenancePositions>
                  </ns1:MaintenanceInterval>
                  <ns1:MaintenanceInterval>
                     <ns1:Description>BEDARFSORIENTIERTER SERVICE MIT FAHRZEUG - CHECK</ns1:Description>
                     <ns1:DATProcessId>94800</ns1:DATProcessId>
                     <ns1:Hint>- Flexibel bis max. 60.000 km / 4 Jahre</ns1:Hint>
                     <ns1:MaintenancePositions>
                        <ns1:MaintenancePosition>
                           <ns1:Description>- Flexibel bis max. 60.000 km / 4 Jahre</ns1:Description>
                           <ns1:PositionType>F</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>FAHRZEUG - CHECK</ns1:Description>
                           <ns1:PositionType>G</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Service-Intervallanzeige nach Werksvorschrift zurückstellen und Wartungsumfänge in elektronische Servicehistorie eintragen</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Lichtanlage prüfen, Funktion der Frontbeleuchtung, Heckbeleuchtung und Kennzeichenbeleuchtung prüfen ggf.Scheinwerfer einstellen</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Instrumenten- und Schriftfeldbeleuchtung prüfen, Innenraumbeleuchtung, Kofferraumbeleuchtung und Handschuhfachbeleuchtung prüfen</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Signalhorn, Lichthupe und Warnblinkanlage prüfen</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Sicherheitsgurte: Zustand des Gurtbandes Gurtclip und ggf. Spange, Funktion von Aufrollmechanismus, Gurtsperre, Gurtschloß prüfen</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Batterie: Säurestand, Ladezustand prüfen (Magic Eye). Falls erforderlich, Batterie nachladen</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Kühlmittelstand und -konzentration prüfen ggf. ergänzen, ggf. bei nicht korrekten Füllstand nach Kundenabsprache Fehlersuche durchführen</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Lenkungsölbehälter: Ölstand prüfen, ggf. bei nicht korrekten Füllstand nach Kundenabsprache Fehlersuche durchführen</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Scheibenwisch- / Waschanlage und falls vorhanden Scheinwerferreinigungsanlage Funktion und Einstellung prüfen</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Scheibenwaschanlage und Intensivreiniger: Flüssigkeitsstand prüfen, ggf. ergänzen</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                           <ns1:MaterialPositions/>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Lenkungskomponenten: Prüfen auf Spielfreiheit, Dichtheit, Schäden und Verschleiß</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Kabelbaum und Anschlüsse auf Beschädigung, Befestigung und richtige Lage prüfen</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Unterboden incl. aller sichtbaren Teile: auf Schäden, Dichtheit, Korrosion inkl. Stoßdämpfer und Montage Federn ausgefedert prüfen</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Bremsleitungen und -anschlüsse: Sichtkontrolle auf Dichtheit, Beschädigung und richtige Lage.</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Reifen: Profiltiefe, Laufbild, äußeren Zustand und Fülldruck prüfen / korrigieren. Profiltiefe VL... mm VR... mm HL... mm HR... mm Ersatzrad... mm, Luftdruck VL... VR... HL... HR... Ersatzrad... bar</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>M-Mobility System: Haltbarkeitsdatum auf der Dichtmittelflasche prüfen</ns1:Description>
                           <ns1:FootNote>- Falls vorhanden</ns1:FootNote>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Reifen Pannen Anzeige initialisieren</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Warndreieck,Warnweste und Erste-Hilfe Set auf Vorhandensein prüfen.Haltbarkeitsdatum prüfen ggf.Ländervorschriften beachten</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Prüfen auf Verkehrssicherheit (Probefahrt) :</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Bremsen</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Lenkung</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Automatgetriebe</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Stoßdämpfer</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>ZUSATZARBEITEN</ns1:Description>
                           <ns1:PositionType>G</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>98118</ns1:DATProcessId>
                           <ns1:RepairType>P</ns1:RepairType>
                           <ns1:Description>Service Standardumfang: Check-Control-Meldungen und Kontroll- und Warnleuchten kontrollieren, ggf. Schiebedachführungsschienen auf Verschmutzung prüfen, Feststellbremse prüfen ohne Prüfstand</ns1:Description>
                           <ns1:PositionType>R</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>98020</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Service Motoröl: Motoröl und Ölfilter wechseln (Motorölfreigabelisten beachten)</ns1:Description>
                           <ns1:FootNote>- alle 30.000 Km oder alle 24 Monate
- Serviceanzeige nach Werksvorschrift zurücksetzen und Wartungsumfang in elektronische Servicehistorie eintragen</ns1:FootNote>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>81200</ns1:DATProcessId>
                                 <ns1:Description>OELFILTER EINSATZ</ns1:Description>
                              </ns1:MaterialPosition>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>99031</ns1:DATProcessId>
                                 <ns1:Description>MOTOROEL</ns1:Description>
                                 <ns1:ManualPriceRequired>true</ns1:ManualPriceRequired>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>64230</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Service Bremse v: Bremsbeläge und Bremsbelagfühler v. wechseln, Bremsschächte reinigen. Bremsscheiben: Oberfläche und Dicke kontrollieren</ns1:Description>
                           <ns1:FootNote>- Serviceanzeige nach Werksvorschrift zurücksetzen und Wartungsumfang in elektronische Servicehistorie eintragen</ns1:FootNote>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>64230</ns1:DATProcessId>
                                 <ns1:Description>REP.-SATZ BREMSBELAEGE V.</ns1:Description>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>75630</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Service Bremse h: Bremsbeläge und Bremsbelagfühler h. wechseln, Bremsschächte reinigen. Bremsscheiben: Oberfläche und Dicke kontrollieren. Feststellbremse Funktionsprüfung auf Rollenprüfstand</ns1:Description>
                           <ns1:FootNote>- Serviceanzeige nach Werksvorschrift zurücksetzen und Wartungsumfang in elektronische Servicehistorie eintragen</ns1:FootNote>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>75630</ns1:DATProcessId>
                                 <ns1:Description>REP.-SATZ BREMSBELAEGE H.</ns1:Description>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Dichtmittelflasche M-Mobility System wechseln</ns1:Description>
                           <ns1:FootNote>- Falls vorhanden</ns1:FootNote>
                           <ns1:PositionType>Z</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>57982</ns1:DATProcessId>
                                 <ns1:Description>DICHTMITTEL REIFEN-REPARATURSET</ns1:Description>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>75980</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Service Bremsflüssigkeit: Bremsflüssigkeit wechseln, Aktives Fußgängerschutzsystem, Haltbarkeitsdatum der Gasdruckfedern Motorhaube prüfen. Haltbarkeit muß nächsten Service erreichen.</ns1:Description>
                           <ns1:FootNote>- alle 24 Monate
- Aktives Fußgängerschutzsystem: Ohne Aufdruck Haltbarkeitsdatum. Ausgehend vom Produktionsdatum Kfz. Gasdruckfedern Frontklappe alle 5 Jahre ersetzen. Serviceanzeige zurücksetzen und Wartungsumfang in elektronische Servicehistorie eintragen</ns1:FootNote>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>99035</ns1:DATProcessId>
                                 <ns1:Description>BREMSFLUESSIGKEIT</ns1:Description>
                                 <ns1:ManualPriceRequired>true</ns1:ManualPriceRequired>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>42847</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Aktives Fußgängerschutzsystem: Gasdruckfeder der Motorhaube wechseln links</ns1:Description>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>42847</ns1:DATProcessId>
                                 <ns1:Description>GASDRUCKFEDER AKTIV FRONTKLAPPE L.</ns1:Description>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>42848</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Aktives Fußgängerschutzsystem: Gasdruckfeder der Motorhaube wechseln rechts</ns1:Description>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>42848</ns1:DATProcessId>
                                 <ns1:Description>GASDRUCKFEDER AKTIV FRONTKLAPPE R.</ns1:Description>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>10040</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Service Mikrofilter: Zusatzarbeiten bei jedem  Motorölwechsel (Mikro- / Aktivkohlefilter wechseln).Bei größerem Staubanfall Wechselintervall verkürzen</ns1:Description>
                           <ns1:FootNote>- alle 30.000 Km oder alle 24 Monate
- Serviceanzeige nach Werksvorschrift zurücksetzen und Wartungsumfang in elektronische Servicehistorie eintragen</ns1:FootNote>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>10040</ns1:DATProcessId>
                                 <ns1:Description>SATZ MIKROFILTER / AKTIVKOHLEFILTER</ns1:Description>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>83112</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Service Luftfiltereinsatz: Zusatzarbeiten bei jedem 2. Motorölwechsel (Luftfiltereinsatz ersetzen).Bei größerem Staubanfall Wechselintervall verkürzen</ns1:Description>
                           <ns1:FootNote>- alle 60.000 Km oder alle 48 Monate
- Serviceanzeige nach Werksvorschrift zurücksetzen und Wartungsumfang in elektronische Servicehistorie eintragen</ns1:FootNote>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>83112</ns1:DATProcessId>
                                 <ns1:Description>LUFTFILTEREINSATZ</ns1:Description>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>83350</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Service Kraftstofffilter: Zusatzarbeiten bei jedem 2. Motorölwechsel (Kraftstoffhauptfilter ersetzen).Bei schlechter Kraftstoffqualität Wechselintervall verkürzen</ns1:Description>
                           <ns1:FootNote>- alle 60.000 Km oder alle 48 Monate
- Serviceanzeige nach Werksvorschrift zurücksetzen und Wartungsumfang in elektronische Servicehistorie eintragen</ns1:FootNote>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>83350</ns1:DATProcessId>
                                 <ns1:Description>KRAFTST.-FILTER</ns1:Description>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Optionale Erweiterung: Wechseln der Wischerblätter mit Kundenabsprache</ns1:Description>
                           <ns1:PositionType>Z</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>45210</ns1:DATProcessId>
                                 <ns1:Description>SATZ WISCHERBLAETTER</ns1:Description>
                              </ns1:MaterialPosition>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>55211</ns1:DATProcessId>
                                 <ns1:Description>WISCHERBLATT HECKSCHEIBE</ns1:Description>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>94901</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Hauptuntersuchung (HU)</ns1:Description>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>94901</ns1:DATProcessId>
                                 <ns1:Description>HAUPTUNTERSUCHUNG (HU)</ns1:Description>
                                 <ns1:ManualPriceRequired>true</ns1:ManualPriceRequired>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>94922</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Abgasuntersuchung (AU) mit OBD-Daten (ON-BOARD-DIAGNOSE) und Endrohrmessung</ns1:Description>
                           <ns1:PositionType>R</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>94903</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Hauptuntersuchung (HU) mit Abgasuntersuchung (AU)</ns1:Description>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>94903</ns1:DATProcessId>
                                 <ns1:Description>HAUPTUNTERSUCHUNG (HU) MIT ABGASUNTERSUCHUNG (AU)</ns1:Description>
                                 <ns1:ManualPriceRequired>true</ns1:ManualPriceRequired>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>WARTUNGSINFORMATION</ns1:Description>
                           <ns1:PositionType>G</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>HINWEIS: Unter bestimmten örtlichen Bedingungen kann es erforderlich sein, bestimmte Servicearbeiten früher auszuführen.</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>KLEINMATERIAL</ns1:Description>
                           <ns1:PositionType>G</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>99100</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Ggf. zusätzlich benötigte Kleinmaterialien</ns1:Description>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>99012</ns1:DATProcessId>
                                 <ns1:Description>GLUEHLAMPEN NORMAL</ns1:Description>
                                 <ns1:ManualPriceRequired>true</ns1:ManualPriceRequired>
                              </ns1:MaterialPosition>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>99013</ns1:DATProcessId>
                                 <ns1:Description>GLUEHLAMPEN HALOGEN</ns1:Description>
                                 <ns1:ManualPriceRequired>true</ns1:ManualPriceRequired>
                              </ns1:MaterialPosition>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>99030</ns1:DATProcessId>
                                 <ns1:Description>FROSTSCHUTZMITTEL</ns1:Description>
                                 <ns1:ManualPriceRequired>true</ns1:ManualPriceRequired>
                              </ns1:MaterialPosition>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>99032</ns1:DATProcessId>
                                 <ns1:Description>GETRIEBEOEL</ns1:Description>
                                 <ns1:ManualPriceRequired>true</ns1:ManualPriceRequired>
                              </ns1:MaterialPosition>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>99033</ns1:DATProcessId>
                                 <ns1:Description>HYDRAULIKOEL</ns1:Description>
                                 <ns1:ManualPriceRequired>true</ns1:ManualPriceRequired>
                              </ns1:MaterialPosition>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>99034</ns1:DATProcessId>
                                 <ns1:Description>SCHEIBENREINIGER</ns1:Description>
                                 <ns1:ManualPriceRequired>true</ns1:ManualPriceRequired>
                              </ns1:MaterialPosition>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>99039</ns1:DATProcessId>
                                 <ns1:Description>REINIGER</ns1:Description>
                                 <ns1:ManualPriceRequired>true</ns1:ManualPriceRequired>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                     </ns1:MaintenancePositions>
                  </ns1:MaintenanceInterval>
                  <ns1:MaintenanceInterval>
                     <ns1:Description>ABGASUNTERSUCHUNG (AU) mit OBD - Daten und Endrohrmessung</ns1:Description>
                     <ns1:DATProcessId>94922</ns1:DATProcessId>
                     <ns1:Hint>- DIESEL</ns1:Hint>
                     <ns1:MaintenancePositions>
                        <ns1:MaintenancePosition>
                           <ns1:Description>- DIESEL</ns1:Description>
                           <ns1:PositionType>F</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Abgasuntersuchung (AU) mit OBD-Daten (ON-BOARD-DIAGNOSE) und Endrohrmessung gemäß gesetzlicher Anforderung durchführen</ns1:Description>
                           <ns1:PositionType>X</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>ZUSATZARBEITEN</ns1:Description>
                           <ns1:PositionType>G</ns1:PositionType>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:Description>Motoröl: nachfüllen</ns1:Description>
                           <ns1:PositionType>Z</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>99031</ns1:DATProcessId>
                                 <ns1:Description>MOTOROEL</ns1:Description>
                                 <ns1:ManualPriceRequired>true</ns1:ManualPriceRequired>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                        <ns1:MaintenancePosition>
                           <ns1:DATProcessId>94901</ns1:DATProcessId>
                           <ns1:RepairType>E</ns1:RepairType>
                           <ns1:Description>Hauptuntersuchung (HU)</ns1:Description>
                           <ns1:PositionType>R</ns1:PositionType>
                           <ns1:MaterialPositions>
                              <ns1:MaterialPosition>
                                 <ns1:DATProcessId>94901</ns1:DATProcessId>
                                 <ns1:Description>HAUPTUNTERSUCHUNG (HU)</ns1:Description>
                                 <ns1:ManualPriceRequired>true</ns1:ManualPriceRequired>
                              </ns1:MaterialPosition>
                           </ns1:MaterialPositions>
                        </ns1:MaintenancePosition>
                     </ns1:MaintenancePositions>
                  </ns1:MaintenanceInterval>
               </ns1:MaintenanceIntervals>
               <ns1:ProcessManagement/>
            </ns1:Dossier>
         </maintenance>
      </ns3:getMaintenanceIntervalsResponse>
   </S:Body>
</S:Envelope>
