---
title: "Response calculateContract"
topic_id: "18908"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > (Nach-) Kalkulieren eines bestehenden Vorgangs > Response calculateContract"
---

# Response calculateContract

<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns10:calculateContractResponse xmlns:ns10="http://www.dat.eu/myClaim/soap/v2/VehicleRepairService">
         <calculationResult source="FI_ONLINE" type="SILVERDATFIONLINE">
            <ns1:Dossier xmlns:ns1="http://www.dat.de/vxs">
               <ns1:Name>DAT-TEST_14:20:56,591</ns1:Name>
               <ns1:Description>DAT-TEST_14:20:56,591</ns1:Description>
               <ns1:DossierId>9999999</ns1:DossierId>
               <ns1:IdSD3Network>9999999</ns1:IdSD3Network>
               <ns1:Country>DE</ns1:Country>
               <ns1:Language>de_DE</ns1:Language>
               <ns1:Currency>EUR</ns1:Currency>
               <ns1:DatCustomerId>1111111</ns1:DatCustomerId>
               <ns1:DossierType>SD3ProCalc</ns1:DossierType>
               <ns1:DossierOrigin>soap</ns1:DossierOrigin>
               <ns1:CreateDate>2023-12-22T14:20:57.468+01:00</ns1:CreateDate>
               <ns1:CreateUser>Anwender</ns1:CreateUser>
               <ns1:ChangeDate>2023-12-22T14:21:00.597+01:00</ns1:ChangeDate>
               <ns1:DatCustomerAddress>
                  <ns1:Title>titleCompany</ns1:Title>
                  <ns1:CompanyName>DAT - Intern</ns1:CompanyName>
                  <ns1:NameLong>Schulung SST-Partner</ns1:NameLong>
                  <ns1:Country>DE</ns1:Country>
                  <ns1:CustomerNumber>1111111</ns1:CustomerNumber>
                  <ns1:CustomerType>1111111</ns1:CustomerType>
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
                  <ns1:ManufacturerName origin="dat">BMW</ns1:ManufacturerName>
                  <ns1:BaseModelName origin="dat">Baureihe 5 Touring (F11)(2010->)</ns1:BaseModelName>
                  <ns1:SubModelName origin="dat">520d</ns1:SubModelName>
                  <ns1:VehicleType>1</ns1:VehicleType>
                  <ns1:Manufacturer>130</ns1:Manufacturer>
                  <ns1:BaseModel>111</ns1:BaseModel>
                  <ns1:SubModel>30</ns1:SubModel>
                  <ns1:Country>DE</ns1:Country>
                  <ns1:isDisengaged>false</ns1:isDisengaged>
                  <ns1:VinActive>false</ns1:VinActive>
                  <ns1:ReleaseIndicator>REPAIR</ns1:ReleaseIndicator>
                  <ns1:SubModelVariant>2</ns1:SubModelVariant>
                  <ns1:RegistrationData>
                     <ns1:KbaCode>0005/AYT</ns1:KbaCode>
                     <ns1:LicenseNumber>ES SM1122</ns1:LicenseNumber>
                  </ns1:RegistrationData>
                  <ns1:Engine/>
                  <ns1:TechInfo>
                     <ns1:InsuranceTypeClassLiability>20</ns1:InsuranceTypeClassLiability>
                     <ns1:InsuranceTypeClassCascoPartial>25</ns1:InsuranceTypeClassCascoPartial>
                     <ns1:InsuranceTypeClassCascoComplete>23</ns1:InsuranceTypeClassCascoComplete>
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
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>15200</ns1:DatEquipmentId>
                           <ns1:Description>Außenspiegel elektr. verstell- und heizbar</ns1:Description>
                           <ns1:EquipmentGroup>AUSP</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18505</ns1:DatEquipmentId>
                           <ns1:Description>Bi-Xenon-Scheinwerfer</ns1:Description>
                           <ns1:EquipmentGroup>XELI</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>19000</ns1:DatEquipmentId>
                                 <ns1:Description>Scheinwerfer-Reinigungsanlage (SRA)</ns1:Description>
                                 <ns1:EquipmentGroup>SWRA</ns1:EquipmentGroup>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>18913</ns1:DatEquipmentId>
                                 <ns1:Description>Tagfahrlicht LED</ns1:Description>
                                 <ns1:EquipmentGroup>TFAL</ns1:EquipmentGroup>
                                 <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>18940</ns1:DatEquipmentId>
                                 <ns1:Description>Blinkleuchten LED</ns1:Description>
                                 <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18604</ns1:DatEquipmentId>
                           <ns1:Description>Automatische Fahrlichtschaltung</ns1:Description>
                           <ns1:EquipmentGroup>AUFL</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18898</ns1:DatEquipmentId>
                           <ns1:Description>Dynamische Bremsleuchte</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>19101</ns1:DatEquipmentId>
                           <ns1:Description>Scheibenwischer mit Regensensor</ns1:Description>
                           <ns1:EquipmentGroup>SWRE</ns1:EquipmentGroup>
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
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25300</ns1:DatEquipmentId>
                           <ns1:Description>Drehzahlmesser</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25508</ns1:DatEquipmentId>
                           <ns1:Description>Bordcomputer</ns1:Description>
                           <ns1:EquipmentGroup>COMP</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25606</ns1:DatEquipmentId>
                           <ns1:Description>Check-Control-System</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25702</ns1:DatEquipmentId>
                           <ns1:Description>Außentemperaturanzeige</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25906</ns1:DatEquipmentId>
                           <ns1:Description>Reifenpannen-Anzeige</ns1:Description>
                           <ns1:EquipmentGroup>RDK</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26710</ns1:DatEquipmentId>
                           <ns1:Description>Geschwindigkeits-Regelanlage mit Bremsfunktion</ns1:Description>
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
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>96508</ns1:DatEquipmentId>
                                 <ns1:Description>Motor 2,0 Ltr. - 135 kW Turbodiesel</ns1:Description>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                           <ns1:Description>Karosserie: 5-türig</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>96508</ns1:DatEquipmentId>
                           <ns1:Description>Motor 2,0 Ltr. - 135 kW Turbodiesel</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>19000</ns1:DatEquipmentId>
                           <ns1:Description>Scheinwerfer-Reinigungsanlage (SRA)</ns1:Description>
                           <ns1:EquipmentGroup>SWRA</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18913</ns1:DatEquipmentId>
                           <ns1:Description>Tagfahrlicht LED</ns1:Description>
                           <ns1:EquipmentGroup>TFAL</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18940</ns1:DatEquipmentId>
                           <ns1:Description>Blinkleuchten LED</ns1:Description>
                           <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                     </ns1:SeriesEquipment>
                     <ns1:SpecialEquipment>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>75914</ns1:DatEquipmentId>
                           <ns1:Description>Getriebe Automatik - mit Steptronic (8-Stufen)</ns1:Description>
                           <ns1:EquipmentGroup>AG2</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>18313</ns1:DatEquipmentId>
                           <ns1:Description>Nebelscheinwerfer LED</ns1:Description>
                           <ns1:EquipmentGroup>BEL</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>37901</ns1:DatEquipmentId>
                           <ns1:Description>Innenspiegel mit Abblendautomatik</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>24607</ns1:DatEquipmentId>
                           <ns1:Description>HiFi-Lautsprechersystem</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27810</ns1:DatEquipmentId>
                           <ns1:Description>Dachhimmel Anthrazit (BMW Individual)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>16302</ns1:DatEquipmentId>
                           <ns1:Description>Panoramadach (Glas)</ns1:Description>
                           <ns1:EquipmentGroup>SD2</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>31408</ns1:DatEquipmentId>
                           <ns1:Description>Innenausstattung: Interieurleisten Aluminium Längsschliff fein</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>28982</ns1:DatEquipmentId>
                           <ns1:Description>Klimaautomatik 2-Zonen mit autom. Umluft-Control, erweiterter Umfang</ns1:Description>
                           <ns1:EquipmentGroup>KLI2</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>77240</ns1:DatEquipmentId>
                           <ns1:Description>Modellvariante CO2-Umfang (Code 1CB)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>29500</ns1:DatEquipmentId>
                           <ns1:Description>Sitzheizung vorn</ns1:Description>
                           <ns1:EquipmentGroup>SITB</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25413</ns1:DatEquipmentId>
                           <ns1:Description>Instrumentenkombination (erweiterter Umfang)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>25930</ns1:DatEquipmentId>
                                 <ns1:Description>Control-Display mit Farbmonitor (9,2 Zoll)</ns1:Description>
                                 <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>16198</ns1:DatEquipmentId>
                           <ns1:Description>Dachreling Hochglanz Shadow-Line</ns1:Description>
                           <ns1:EquipmentGroup>DARE</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25930</ns1:DatEquipmentId>
                           <ns1:Description>Control-Display mit Farbmonitor (9,2 Zoll)</ns1:Description>
                           <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25802</ns1:DatEquipmentId>
                           <ns1:Description>Park-Distance-Control (PDC)</ns1:Description>
                           <ns1:EquipmentGroup>PDC1</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25804</ns1:DatEquipmentId>
                           <ns1:Description>Audio-Navigationssystem Professional</ns1:Description>
                           <ns1:EquipmentGroup>GPS</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>24709</ns1:DatEquipmentId>
                                 <ns1:Description>Sprachbediensystem</ns1:Description>
                                 <ns1:EquipmentGroup>TEL4</ns1:EquipmentGroup>
                                 <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>22102</ns1:DatEquipmentId>
                           <ns1:Description>Sonnenschutzverglasung (hinten abgedunkelt, BMW Individual)</ns1:Description>
                           <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>30301</ns1:DatEquipmentId>
                           <ns1:Description>Sitzbezug / Polsterung: Leder Dakota</ns1:Description>
                           <ns1:EquipmentGroup>LEDE</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>37603</ns1:DatEquipmentId>
                           <ns1:Description>Ambiente-Beleuchtung</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25704</ns1:DatEquipmentId>
                           <ns1:Description>Fahrassistenz-System: Speed-Limit-Anzeige</ns1:Description>
                           <ns1:EquipmentGroup>FA28</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>22505</ns1:DatEquipmentId>
                           <ns1:Description>Frontscheibe (Ausführung: Klimakomfort)</ns1:Description>
                           <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>25204</ns1:DatEquipmentId>
                           <ns1:Description>Head-up-Display</ns1:Description>
                           <ns1:EquipmentGroup>HUD</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>25413</ns1:DatEquipmentId>
                                 <ns1:Description>Instrumentenkombination (erweiterter Umfang)</ns1:Description>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>25930</ns1:DatEquipmentId>
                                 <ns1:Description>Control-Display mit Farbmonitor (9,2 Zoll)</ns1:Description>
                                 <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                                 <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>33403</ns1:DatEquipmentId>
                           <ns1:Description>Lendenwirbelstütze Sitz vorn links und rechts, elektr. verstellbar</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>8702</ns1:DatEquipmentId>
                           <ns1:Description>Außenausstattung: Shadow-Line Hochglanz</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>24709</ns1:DatEquipmentId>
                           <ns1:Description>Sprachbediensystem</ns1:Description>
                           <ns1:EquipmentGroup>TEL4</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                     </ns1:SpecialEquipment>
                  </ns1:Equipment>
                  <ns1:Tires>
                     <ns1:Axles/>
                  </ns1:Tires>
               </ns1:Vehicle>
               <ns1:VAT>
                  <ns1:VatType>Regular</ns1:VatType>
                  <ns1:VatAtValuationTime origin="dat">19.0</ns1:VatAtValuationTime>
                  <ns1:VatAtCalculationTime>19.0</ns1:VatAtCalculationTime>
               </ns1:VAT>
               <ns1:TradingData>
                  <ns1:Owner>
                     <ns1:LastName>Test</ns1:LastName>
                     <ns1:FirstName>Heiner</ns1:FirstName>
                     <ns1:Country>DE</ns1:Country>
                     <ns1:VatEntitled>false</ns1:VatEntitled>
                     <ns1:UsageFlag>2</ns1:UsageFlag>
                  </ns1:Owner>
                  <ns1:Dealership>
                     <ns1:Title>titleCompany</ns1:Title>
                     <ns1:CompanyName>DAT - Intern</ns1:CompanyName>
                     <ns1:NameLong>Schulung SST-Partner</ns1:NameLong>
                     <ns1:Country>DE</ns1:Country>
                     <ns1:CustomerNumber>1111111</ns1:CustomerNumber>
                     <ns1:CustomerType>REPAIRER</ns1:CustomerType>
                     <ns1:CustomerTypeShort>94144</ns1:CustomerTypeShort>
                     <ns1:Street>Hellmuth-Hirth-Str.</ns1:Street>
                     <ns1:StreetNumber>1</ns1:StreetNumber>
                     <ns1:StreetZipCode>73760</ns1:StreetZipCode>
                     <ns1:StreetCity>Ostfildern</ns1:StreetCity>
                     <ns1:EMail>kundendienst@dat.de</ns1:EMail>
                     <ns1:PhoneBusiness>+49 711/45000</ns1:PhoneBusiness>
                     <ns1:UsageFlag>9</ns1:UsageFlag>
                  </ns1:Dealership>
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
                     <ns1:ManufacturerName origin="dat">BMW</ns1:ManufacturerName>
                     <ns1:BaseModelName origin="dat">Baureihe 5 Touring (F11)(2010->)</ns1:BaseModelName>
                     <ns1:SubModelName origin="dat">520d</ns1:SubModelName>
                     <ns1:VehicleType>1</ns1:VehicleType>
                     <ns1:Manufacturer>130</ns1:Manufacturer>
                     <ns1:BaseModel>111</ns1:BaseModel>
                     <ns1:SubModel>30</ns1:SubModel>
                     <ns1:Country>DE</ns1:Country>
                     <ns1:isDisengaged>false</ns1:isDisengaged>
                     <ns1:VinActive>false</ns1:VinActive>
                     <ns1:ReleaseIndicator>REPAIR</ns1:ReleaseIndicator>
                     <ns1:SubModelVariant>2</ns1:SubModelVariant>
                     <ns1:RegistrationData>
                        <ns1:KbaCode>0005/AYT</ns1:KbaCode>
                        <ns1:LicenseNumber>ES SM1122</ns1:LicenseNumber>
                     </ns1:RegistrationData>
                     <ns1:Engine/>
                     <ns1:TechInfo>
                        <ns1:InsuranceTypeClassLiability>20</ns1:InsuranceTypeClassLiability>
                        <ns1:InsuranceTypeClassCascoPartial>25</ns1:InsuranceTypeClassCascoPartial>
                        <ns1:InsuranceTypeClassCascoComplete>23</ns1:InsuranceTypeClassCascoComplete>
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
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>15200</ns1:DatEquipmentId>
                              <ns1:Description>Außenspiegel elektr. verstell- und heizbar</ns1:Description>
                              <ns1:EquipmentGroup>AUSP</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>18505</ns1:DatEquipmentId>
                              <ns1:Description>Bi-Xenon-Scheinwerfer</ns1:Description>
                              <ns1:EquipmentGroup>XELI</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>19000</ns1:DatEquipmentId>
                                    <ns1:Description>Scheinwerfer-Reinigungsanlage (SRA)</ns1:Description>
                                    <ns1:EquipmentGroup>SWRA</ns1:EquipmentGroup>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>18913</ns1:DatEquipmentId>
                                    <ns1:Description>Tagfahrlicht LED</ns1:Description>
                                    <ns1:EquipmentGroup>TFAL</ns1:EquipmentGroup>
                                    <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>18940</ns1:DatEquipmentId>
                                    <ns1:Description>Blinkleuchten LED</ns1:Description>
                                    <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>18604</ns1:DatEquipmentId>
                              <ns1:Description>Automatische Fahrlichtschaltung</ns1:Description>
                              <ns1:EquipmentGroup>AUFL</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>18898</ns1:DatEquipmentId>
                              <ns1:Description>Dynamische Bremsleuchte</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>19101</ns1:DatEquipmentId>
                              <ns1:Description>Scheibenwischer mit Regensensor</ns1:Description>
                              <ns1:EquipmentGroup>SWRE</ns1:EquipmentGroup>
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
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25300</ns1:DatEquipmentId>
                              <ns1:Description>Drehzahlmesser</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25508</ns1:DatEquipmentId>
                              <ns1:Description>Bordcomputer</ns1:Description>
                              <ns1:EquipmentGroup>COMP</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25606</ns1:DatEquipmentId>
                              <ns1:Description>Check-Control-System</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25702</ns1:DatEquipmentId>
                              <ns1:Description>Außentemperaturanzeige</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25906</ns1:DatEquipmentId>
                              <ns1:Description>Reifenpannen-Anzeige</ns1:Description>
                              <ns1:EquipmentGroup>RDK</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>26710</ns1:DatEquipmentId>
                              <ns1:Description>Geschwindigkeits-Regelanlage mit Bremsfunktion</ns1:Description>
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
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>96508</ns1:DatEquipmentId>
                                    <ns1:Description>Motor 2,0 Ltr. - 135 kW Turbodiesel</ns1:Description>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                              <ns1:Description>Karosserie: 5-türig</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>96508</ns1:DatEquipmentId>
                              <ns1:Description>Motor 2,0 Ltr. - 135 kW Turbodiesel</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>19000</ns1:DatEquipmentId>
                              <ns1:Description>Scheinwerfer-Reinigungsanlage (SRA)</ns1:Description>
                              <ns1:EquipmentGroup>SWRA</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>18913</ns1:DatEquipmentId>
                              <ns1:Description>Tagfahrlicht LED</ns1:Description>
                              <ns1:EquipmentGroup>TFAL</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>18940</ns1:DatEquipmentId>
                              <ns1:Description>Blinkleuchten LED</ns1:Description>
                              <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                        </ns1:SeriesEquipment>
                        <ns1:SpecialEquipment>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>75914</ns1:DatEquipmentId>
                              <ns1:Description>Getriebe Automatik - mit Steptronic (8-Stufen)</ns1:Description>
                              <ns1:EquipmentGroup>AG2</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>18313</ns1:DatEquipmentId>
                              <ns1:Description>Nebelscheinwerfer LED</ns1:Description>
                              <ns1:EquipmentGroup>BEL</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>37901</ns1:DatEquipmentId>
                              <ns1:Description>Innenspiegel mit Abblendautomatik</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>24607</ns1:DatEquipmentId>
                              <ns1:Description>HiFi-Lautsprechersystem</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27810</ns1:DatEquipmentId>
                              <ns1:Description>Dachhimmel Anthrazit (BMW Individual)</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>16302</ns1:DatEquipmentId>
                              <ns1:Description>Panoramadach (Glas)</ns1:Description>
                              <ns1:EquipmentGroup>SD2</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>31408</ns1:DatEquipmentId>
                              <ns1:Description>Innenausstattung: Interieurleisten Aluminium Längsschliff fein</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>28982</ns1:DatEquipmentId>
                              <ns1:Description>Klimaautomatik 2-Zonen mit autom. Umluft-Control, erweiterter Umfang</ns1:Description>
                              <ns1:EquipmentGroup>KLI2</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>77240</ns1:DatEquipmentId>
                              <ns1:Description>Modellvariante CO2-Umfang (Code 1CB)</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>29500</ns1:DatEquipmentId>
                              <ns1:Description>Sitzheizung vorn</ns1:Description>
                              <ns1:EquipmentGroup>SITB</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25413</ns1:DatEquipmentId>
                              <ns1:Description>Instrumentenkombination (erweiterter Umfang)</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>25930</ns1:DatEquipmentId>
                                    <ns1:Description>Control-Display mit Farbmonitor (9,2 Zoll)</ns1:Description>
                                    <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>16198</ns1:DatEquipmentId>
                              <ns1:Description>Dachreling Hochglanz Shadow-Line</ns1:Description>
                              <ns1:EquipmentGroup>DARE</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25930</ns1:DatEquipmentId>
                              <ns1:Description>Control-Display mit Farbmonitor (9,2 Zoll)</ns1:Description>
                              <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25802</ns1:DatEquipmentId>
                              <ns1:Description>Park-Distance-Control (PDC)</ns1:Description>
                              <ns1:EquipmentGroup>PDC1</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25804</ns1:DatEquipmentId>
                              <ns1:Description>Audio-Navigationssystem Professional</ns1:Description>
                              <ns1:EquipmentGroup>GPS</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>24709</ns1:DatEquipmentId>
                                    <ns1:Description>Sprachbediensystem</ns1:Description>
                                    <ns1:EquipmentGroup>TEL4</ns1:EquipmentGroup>
                                    <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>22102</ns1:DatEquipmentId>
                              <ns1:Description>Sonnenschutzverglasung (hinten abgedunkelt, BMW Individual)</ns1:Description>
                              <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>30301</ns1:DatEquipmentId>
                              <ns1:Description>Sitzbezug / Polsterung: Leder Dakota</ns1:Description>
                              <ns1:EquipmentGroup>LEDE</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>37603</ns1:DatEquipmentId>
                              <ns1:Description>Ambiente-Beleuchtung</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25704</ns1:DatEquipmentId>
                              <ns1:Description>Fahrassistenz-System: Speed-Limit-Anzeige</ns1:Description>
                              <ns1:EquipmentGroup>FA28</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>22505</ns1:DatEquipmentId>
                              <ns1:Description>Frontscheibe (Ausführung: Klimakomfort)</ns1:Description>
                              <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>25204</ns1:DatEquipmentId>
                              <ns1:Description>Head-up-Display</ns1:Description>
                              <ns1:EquipmentGroup>HUD</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>25413</ns1:DatEquipmentId>
                                    <ns1:Description>Instrumentenkombination (erweiterter Umfang)</ns1:Description>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>25930</ns1:DatEquipmentId>
                                    <ns1:Description>Control-Display mit Farbmonitor (9,2 Zoll)</ns1:Description>
                                    <ns1:EquipmentGroup>MONM</ns1:EquipmentGroup>
                                    <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>33403</ns1:DatEquipmentId>
                              <ns1:Description>Lendenwirbelstütze Sitz vorn links und rechts, elektr. verstellbar</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>8702</ns1:DatEquipmentId>
                              <ns1:Description>Außenausstattung: Shadow-Line Hochglanz</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>24709</ns1:DatEquipmentId>
                              <ns1:Description>Sprachbediensystem</ns1:Description>
                              <ns1:EquipmentGroup>TEL4</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                        </ns1:SpecialEquipment>
                     </ns1:Equipment>
                     <ns1:Tires>
                        <ns1:Axles/>
                     </ns1:Tires>
                  </ns1:Vehicle>
                  <ns1:RepairParameters>
                     <ns1:PhantomCalculation>false</ns1:PhantomCalculation>
                     <ns1:LacquerTypeId>12</ns1:LacquerTypeId>
                     <ns1:LacquerType>Metallic (2-Schicht)</ns1:LacquerType>
                     <ns1:LacquerTypeLayers>2</ns1:LacquerTypeLayers>
                     <ns1:TimeUnitsOfManufacturer>false</ns1:TimeUnitsOfManufacturer>
                     <ns1:DMSCalculation>false</ns1:DMSCalculation>
                  </ns1:RepairParameters>
                  <ns1:ProcedureRelatedParameters>
                     <ns1:ProcedureRelatedParameter attribute="referenceSetName" factor="CalculationFactor" type="String">DAT TEST</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="biwOptimizationMode" factor="CalculationFactor" type="BiwOptimizationMode">AUTOMATIC</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="selectedLacquerMethod" factor="CalculationFactor" type="LacquerMethod">MANUFACTURER_SPECIFIC</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="crossSeries" factor="CalculationFactor" type="CrossSeriesState">NO</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="withoutValuesOfAdditionallyRequiredPositions" factor="CalculationFactor" type="Boolean">false</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnit" factor="CalculationFactor" type="TimeUnitSystem">HOUR</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="CalculationFactor" type="Integer">1</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="dataCurrency" factor="CalculationFactor" type="String">EUR</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="surchargeInProtocolOly" factor="SparePartFactor" type="Boolean">true</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="smallSparePartCalculationModel" factor="SparePartFactor" type="SmallPartsCalculationModel">PERCENT_OF_PARTS</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="priceDate" factor="SparePartFactor" type="Date">2023-12-01</ns1:ProcedureRelatedParameter>
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
                     <ns1:ProcedureRelatedParameter attribute="timeUnit" factor="AztLacquerFactor" type="TimeUnitSystem">HOUR</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="threeLayerLacquerMode" factor="AztLacquerFactor" type="AztLacquerMode">WET_IN_WET</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="AztLacquerFactor" type="Integer">1</ns1:ProcedureRelatedParameter>
                  </ns1:ProcedureRelatedParameters>
                  <ns1:RepairPositions>
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>20111</ns1:DATProcessId>
                        <ns1:RepairType>replace</ns1:RepairType>
                        <ns1:Description>Tür</ns1:Description>
                        <ns1:DescriptionId>77066</ns1:DescriptionId>
                        <ns1:IsManualDescription>false</ns1:IsManualDescription>
                        <ns1:ConstructionGroupId>11</ns1:ConstructionGroupId>
                        <ns1:ConstructionGroup>ARMATURENBRETT</ns1:ConstructionGroup>
                        <ns1:ConstructionGroupPolygon>13</ns1:ConstructionGroupPolygon>
                        <ns1:PositionEntryType>graphical</ns1:PositionEntryType>
                        <ns1:IsRepairExtension>false</ns1:IsRepairExtension>
                        <ns1:DentsWithFinishing>false</ns1:DentsWithFinishing>
                        <ns1:DentsWithSetupTime>false</ns1:DentsWithSetupTime>
                        <ns1:IsAdditionalLM>false</ns1:IsAdditionalLM>
                        <ns1:PreDamage>false</ns1:PreDamage>
                        <ns1:AlloyLM>false</ns1:AlloyLM>
                     </ns1:RepairPosition>
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>44210</ns1:DATProcessId>
                        <ns1:RepairType>lacquer</ns1:RepairType>
                        <ns1:Description>Frontklappe</ns1:Description>
                        <ns1:DescriptionId>141168</ns1:DescriptionId>
                        <ns1:IsManualDescription>false</ns1:IsManualDescription>
                        <ns1:ConstructionGroupId>1</ns1:ConstructionGroupId>
                        <ns1:ConstructionGroup>VORDERWAGEN AUSSEN</ns1:ConstructionGroup>
                        <ns1:ConstructionGroupPolygon>20</ns1:ConstructionGroupPolygon>
                        <ns1:PositionEntryType>dents</ns1:PositionEntryType>
                        <ns1:IsRepairExtension>false</ns1:IsRepairExtension>
                        <ns1:LacquerLevel>none</ns1:LacquerLevel>
                        <ns1:LacquerLevelId>0</ns1:LacquerLevelId>
                        <ns1:DentsCalculationMethod>bvat</ns1:DentsCalculationMethod>
                        <ns1:DentsWithFinishing>true</ns1:DentsWithFinishing>
                        <ns1:DentsWithSetupTime>true</ns1:DentsWithSetupTime>
                        <ns1:DentsOutOfReach>false</ns1:DentsOutOfReach>
                        <ns1:IsAdditionalLM>false</ns1:IsAdditionalLM>
                        <ns1:PreDamage>false</ns1:PreDamage>
                        <ns1:AlloyLM>false</ns1:AlloyLM>
                        <ns1:AdhesiveMethod>false</ns1:AdhesiveMethod>
                     </ns1:RepairPosition>
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>44210</ns1:DATProcessId>
                        <ns1:RepairType>overhaul</ns1:RepairType>
                        <ns1:Description>Frontklappe</ns1:Description>
                        <ns1:DescriptionId>141168</ns1:DescriptionId>
                        <ns1:IsManualDescription>false</ns1:IsManualDescription>
                        <ns1:ConstructionGroupId>1</ns1:ConstructionGroupId>
                        <ns1:ConstructionGroup>VORDERWAGEN AUSSEN</ns1:ConstructionGroup>
                        <ns1:ConstructionGroupPolygon>20</ns1:ConstructionGroupPolygon>
                        <ns1:PositionEntryType>dents</ns1:PositionEntryType>
                        <ns1:IsRepairExtension>false</ns1:IsRepairExtension>
                        <ns1:DentsCount>20</ns1:DentsCount>
                        <ns1:DentsOver20mmCount>20</ns1:DentsOver20mmCount>
                        <ns1:DentsSize>20</ns1:DentsSize>
                        <ns1:DentsPartOrientation>vertical</ns1:DentsPartOrientation>
                        <ns1:DentsCalculationMethod>bvat</ns1:DentsCalculationMethod>
                        <ns1:DentsWithFinishing>true</ns1:DentsWithFinishing>
                        <ns1:DentsWithSetupTime>true</ns1:DentsWithSetupTime>
                        <ns1:DentsOutOfReach>false</ns1:DentsOutOfReach>
                        <ns1:IsAdditionalLM>false</ns1:IsAdditionalLM>
                        <ns1:PreDamage>false</ns1:PreDamage>
                        <ns1:AlloyLM>false</ns1:AlloyLM>
                        <ns1:AdhesiveMethod>false</ns1:AdhesiveMethod>
                     </ns1:RepairPosition>
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>43711</ns1:DATProcessId>
                        <ns1:RepairType>replace</ns1:RepairType>
                        <ns1:Description>Seitenwand grundiert</ns1:Description>
                        <ns1:DescriptionId>36419456</ns1:DescriptionId>
                        <ns1:IsManualDescription>false</ns1:IsManualDescription>
                        <ns1:ConstructionGroupId>1</ns1:ConstructionGroupId>
                        <ns1:ConstructionGroup>VORDERWAGEN AUSSEN</ns1:ConstructionGroup>
                        <ns1:ConstructionGroupPolygon>63</ns1:ConstructionGroupPolygon>
                        <ns1:PositionEntryType>graphical</ns1:PositionEntryType>
                        <ns1:IsRepairExtension>false</ns1:IsRepairExtension>
                        <ns1:DentsWithFinishing>false</ns1:DentsWithFinishing>
                        <ns1:DentsWithSetupTime>false</ns1:DentsWithSetupTime>
                        <ns1:IsAdditionalLM>false</ns1:IsAdditionalLM>
                        <ns1:PreDamage>false</ns1:PreDamage>
                        <ns1:AlloyLM>false</ns1:AlloyLM>
                     </ns1:RepairPosition>
                  </ns1:RepairPositions>
                  <ns1:CalcResultToUse>common</ns1:CalcResultToUse>
                  <ns1:CalcEngine>DAT</ns1:CalcEngine>
                  <ns1:CalcSource>vxs</ns1:CalcSource>
                  <ns1:CalcResultCommon>
                     <ns1:MaterialPositions>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>20111</ns1:DATProcessId>
                           <ns1:PartNumber>41007206107</ns1:PartNumber>
                           <ns1:DATPartNumber>41007206107</ns1:DATPartNumber>
                           <ns1:Description>TUER V.L.</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>794.27</ns1:ValuePerUnit>
                           <ns1:ValueTotal>794.27</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>794.27</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>20351</ns1:DATProcessId>
                           <ns1:PartNumber>51767182269</ns1:PartNumber>
                           <ns1:DATPartNumber>51767182269</ns1:DATPartNumber>
                           <ns1:Description>TUERDICHTUNG V.L.</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>86.03</ns1:ValuePerUnit>
                           <ns1:ValueTotal>86.03</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>86.03</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:RequiredByProcessId>20111</ns1:RequiredByProcessId>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>43711</ns1:DATProcessId>
                           <ns1:PartNumber>41355A03261</ns1:PartNumber>
                           <ns1:DATPartNumber>41355A03261</ns1:DATPartNumber>
                           <ns1:Description>SEITENWAND V.L.</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>371.22</ns1:ValuePerUnit>
                           <ns1:ValueTotal>371.22</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>371.22</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                     </ns1:MaterialPositions>
                     <ns1:LabourPositions>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>20111</ns1:DATProcessId>
                           <ns1:LabourPositionKind>1</ns1:LabourPositionKind>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:LabourPosId>41 51 500</ns1:LabourPosId>
                           <ns1:Description>VORDERTUER L. ERS.
UMFASST: TUER A+E</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>4</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>420.00</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>420.00</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>41 51 500</ns1:WorkNumber>
                           <ns1:SparePartNumber>41007206107</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>20111</ns1:DATProcessId>
                           <ns1:LabourPositionKind>4</ns1:LabourPositionKind>
                           <ns1:RepairType>body cavity protection</ns1:RepairType>
                           <ns1:LabourPosId>97 51 501</ns1:LabourPosId>
                           <ns1:Description>HOHLRAUMKONSERVIERUNG VORDERTUER L.
(VERBUNDARBEIT)</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>0.17</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>17.85</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>17.85</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>true</ns1:hasRequiredByPosition>
                           <ns1:RequiredByPosition>
                              <ns1:DATProcessId>20111</ns1:DATProcessId>
                              <ns1:RepairType>replace</ns1:RepairType>
                           </ns1:RequiredByPosition>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>97 51 501</ns1:WorkNumber>
                           <ns1:SparePartNumber>41007206107</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>43711</ns1:DATProcessId>
                           <ns1:LabourPositionKind>1</ns1:LabourPositionKind>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:LabourPosId>41 35 550</ns1:LabourPosId>
                           <ns1:Description>SEITENWAND V.L. ERS.</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>1.58</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>165.90</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>165.90</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>41 35 550</ns1:WorkNumber>
                           <ns1:SparePartNumber>41355A03261</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>43711</ns1:DATProcessId>
                           <ns1:LabourPositionKind>4</ns1:LabourPositionKind>
                           <ns1:RepairType>body cavity protection</ns1:RepairType>
                           <ns1:LabourPosId>97 35 511</ns1:LabourPosId>
                           <ns1:Description>HOHLRAUMKONSERVIERUNG SEITENWAND V.L.</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>0.42</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>44.10</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>44.10</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>true</ns1:hasRequiredByPosition>
                           <ns1:RequiredByPosition>
                              <ns1:DATProcessId>43711</ns1:DATProcessId>
                              <ns1:RepairType>replace</ns1:RepairType>
                           </ns1:RequiredByPosition>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>97 35 511</ns1:WorkNumber>
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
                           <ns1:DATProcessId>44210</ns1:DATProcessId>
                           <ns1:RepairType>overhaul</ns1:RepairType>
                           <ns1:Description>FRONTKLAPPE
(GROESSE: 20 MM)</ns1:Description>
                           <ns1:WageType>dents</ns1:WageType>
                           <ns1:Duration>2.70</ns1:Duration>
                           <ns1:ValueTotal>210.60</ns1:ValueTotal>
                           <ns1:ValueTotalCorrected>210.60</ns1:ValueTotalCorrected>
                           <ns1:Amount>20</ns1:Amount>
                           <ns1:size>20</ns1:size>
                           <ns1:DentsCalculationMethod>press</ns1:DentsCalculationMethod>
                           <ns1:SparePartNumber>41617207194</ns1:SparePartNumber>
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
                           <ns1:LabourPosId>99 51 011</ns1:LabourPosId>
                           <ns1:Description>VORDERTUER L. UMFASST: VORBEREITUNGSARBEITEN</ns1:Description>
                           <ns1:Level>4</ns1:Level>
                           <ns1:LevelDescription>new</ns1:LevelDescription>
                           <ns1:LevelManufacturer>ST.2</ns1:LevelManufacturer>
                           <ns1:Duration>3.5</ns1:Duration>
                           <ns1:ManualDuration>false</ns1:ManualDuration>
                           <ns1:Material>105</ns1:Material>
                           <ns1:ValueTotal>525.00</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>525.00</ns1:ValueTotalCorrected>
                           <ns1:WageLevel1>420</ns1:WageLevel1>
                           <ns1:WorkNumber>99 51 011</ns1:WorkNumber>
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
                           <ns1:LabourPosId>99 35 519</ns1:LabourPosId>
                           <ns1:Description>SEITENWAND V.L.</ns1:Description>
                           <ns1:Level>4</ns1:Level>
                           <ns1:LevelDescription>new</ns1:LevelDescription>
                           <ns1:LevelManufacturer>ST.2</ns1:LevelManufacturer>
                           <ns1:Duration>0.67</ns1:Duration>
                           <ns1:ManualDuration>false</ns1:ManualDuration>
                           <ns1:Material>20.1</ns1:Material>
                           <ns1:ValueTotal>100.50</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>100.50</ns1:ValueTotalCorrected>
                           <ns1:WageLevel1>80.4</ns1:WageLevel1>
                           <ns1:WorkNumber>99 35 519</ns1:WorkNumber>
                           <ns1:LacquerPositionTimeState/>
                           <ns1:LacquerPositionMaterialState/>
                           <ns1:LacquerPositionPriceState/>
                           <ns1:MaterialType>2</ns1:MaterialType>
                           <ns1:SparePartNumber>41355A03261</ns1:SparePartNumber>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                        </ns1:LacquerPosition>
                     </ns1:LacquerPositions>
                     <ns1:PriceDate>2023-12-01+01:00</ns1:PriceDate>
                     <ns1:RepairCalculationSummary>
                        <ns1:SparePartsCosts>
                           <ns1:AllSum>1251.52</ns1:AllSum>
                           <ns1:ConsumablesSurcharge>25.03</ns1:ConsumablesSurcharge>
                           <ns1:ConsumablesSurchargePercentage>2.00</ns1:ConsumablesSurchargePercentage>
                           <ns1:TotalSum>1276.55</ns1:TotalSum>
                        </ns1:SparePartsCosts>
                        <ns1:AuxiliaryCosts/>
                        <ns1:LabourCosts>
                           <ns1:AllSum>942.60</ns1:AllSum>
                           <ns1:Bodywork>
                              <ns1:Type>CAR BODY</ns1:Type>
                              <ns1:Units>6.34</ns1:Units>
                              <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                              <ns1:Price>665.70</ns1:Price>
                           </ns1:Bodywork>
                           <ns1:Electric>
                              <ns1:Type>ELECTRIC</ns1:Type>
                              <ns1:Units>0</ns1:Units>
                              <ns1:Price>0</ns1:Price>
                           </ns1:Electric>
                           <ns1:Mechanic>
                              <ns1:Type>MECHANIC</ns1:Type>
                              <ns1:Units>0</ns1:Units>
                              <ns1:Price>0</ns1:Price>
                           </ns1:Mechanic>
                           <ns1:DentsPress>
                              <ns1:Type>DENTS PRESS</ns1:Type>
                              <ns1:Units>2.70</ns1:Units>
                              <ns1:PricePerUnit>78.00</ns1:PricePerUnit>
                              <ns1:Price>210.60</ns1:Price>
                           </ns1:DentsPress>
                           <ns1:DentsGlobal>
                              <ns1:Type>DENTS GLOBAL</ns1:Type>
                              <ns1:Units>0.85</ns1:Units>
                              <ns1:PricePerUnit>78.00</ns1:PricePerUnit>
                              <ns1:Price>66.30</ns1:Price>
                           </ns1:DentsGlobal>
                           <ns1:TotalSum>942.60</ns1:TotalSum>
                           <ns1:Wages/>
                           <ns1:Works>
                              <ns1:Work>
                                 <ns1:Type>CAR BODY</ns1:Type>
                                 <ns1:WageLevel>1</ns1:WageLevel>
                                 <ns1:Units>6.34</ns1:Units>
                                 <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                                 <ns1:Price>665.70</ns1:Price>
                              </ns1:Work>
                              <ns1:Work>
                                 <ns1:Type>HAIL DAMAGE PRESS</ns1:Type>
                                 <ns1:Units>2.70</ns1:Units>
                                 <ns1:PricePerUnit>78.00</ns1:PricePerUnit>
                                 <ns1:Price>210.60</ns1:Price>
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
                              <ns1:Units>4.17</ns1:Units>
                              <ns1:PricePerUnit>120.00</ns1:PricePerUnit>
                              <ns1:Price>500.40</ns1:Price>
                           </ns1:Wage>
                           <ns1:TotalWages>500.40</ns1:TotalWages>
                           <ns1:Material>
                              <ns1:FlatPercentage>25.0</ns1:FlatPercentage>
                              <ns1:FlatAmount>125.10</ns1:FlatAmount>
                              <ns1:MaterialGroups/>
                              <ns1:TotalSum>125.10</ns1:TotalSum>
                              <ns1:SumMaterialCorrected>125.10</ns1:SumMaterialCorrected>
                           </ns1:Material>
                           <ns1:TotalSum>625.50</ns1:TotalSum>
                        </ns1:LacquerCosts>
                        <ns1:TotalNetCosts>2844.65</ns1:TotalNetCosts>
                        <ns1:TotalVAT>540.48</ns1:TotalVAT>
                        <ns1:TotalGrossCosts>3385.13</ns1:TotalGrossCosts>
                        <ns1:TotalNetCorrected>2844.65</ns1:TotalNetCorrected>
                        <ns1:TotalVATCorrected>540.48</ns1:TotalVATCorrected>
                        <ns1:TotalGrossCorrected>3385.13</ns1:TotalGrossCorrected>
                        <ns1:AmountCustomer>0</ns1:AmountCustomer>
                        <ns1:AmountInsurance>3385.13</ns1:AmountInsurance>
                        <ns1:SumNet>2844.65</ns1:SumNet>
                        <ns1:SumGross>3385.13</ns1:SumGross>
                        <ns1:SumSparePartCosts>1251.52</ns1:SumSparePartCosts>
                        <ns1:SumSmallSparePartCosts>25.03</ns1:SumSmallSparePartCosts>
                        <ns1:SumLabourCosts>942.60</ns1:SumLabourCosts>
                        <ns1:MetaPositions>
                           <ns1:MetaPosition key="TIME_UNIT_SYSTEM" value="STD"/>
                           <ns1:MetaPosition key="LACQUER_TIME_UNIT_SYSTEM" value="STD"/>
                           <ns1:MetaPosition key="DAT_EUROLACQUER_IN_HOURS" value="false"/>
                           <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EQUIPMENT" value="false"/>
                           <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EXTENSION" value="false"/>
                           <ns1:MetaPosition key="FLAT_PERCENTAGE_BASE" value="500.40"/>
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
                              <ns1:DATProcessId>44210</ns1:DATProcessId>
                              <ns1:Description>Frontklappe</ns1:Description>
                              <ns1:CalculationMethod>bvat</ns1:CalculationMethod>
                              <ns1:CalculationMethodDescription>Bundesverband Ausbeultechnik (BVAT), Drücken</ns1:CalculationMethodDescription>
                              <ns1:DentsCount>20</ns1:DentsCount>
                              <ns1:DentsSize>20</ns1:DentsSize>
                           </ns1:DentPositionsProtocolEntry>
                        </ns1:DentPositionsProtocol>
                        <ns1:ProtocolData>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wkdWRpjw4gCMMOHxIoQRJjxehDDChJfCYERt37MythLFhpWtFOri04HQNm2Sj/jf1/r8np9HjR4P6b4s5eSQ80jOh+fJME5Zj6z5Oj9nmfKr/gJXcyzeCmVuZHN0cmVhbQplbmRvYmoKMyAwIG9iago8PC9TdWJ0eXBlL1R5cGUwL1R5cGUvRm9udC9CYXNlRm9udC9UU0NZQUcrRGVqYVZ1U2Fuc0NvbmRlbnNlZC1Cb2xkL0VuY29kaW5nL0lkZW50aXR5LUgvRGVzY2VuZGFudEZvbnRzWzEzIDAgUl0vVG9Vbmljb2RlIDE0IDAgUj4+CmVuZG9iago1IDAgb2JqCjw8L0tpZHNbMSAwIFJdL1R5cGUvUGFnZXMvQ291bnQgMS9JVFhUKDQuMi4wKT4+CmVuZG9iagoxNSAwIG9iago8PC9OYW1lc1soSlJfUEFHRV9BTkNIT1JfMF8xKSA2IDAgUl0+PgplbmRvYmoKMTYgMCBvYmoKPDwvRGVzdHMgMTUgMCBSPj4KZW5kb2JqCjE3IDAgb2JqCjw8L05hbWVzIDE2IDAgUi9UeXBlL0NhdGFsb2cvUGFnZXMgNSAwIFIvVmlld2VyUHJlZmVyZW5jZXM8PC9QcmludFNjYWxpbmcvQXBwRGVmYXVsdD4+Pj4KZW5kb2JqCjE4IDAgb2JqCjw8L01vZERhdGUoRDoyMDIzMTIyMjE0MjEwMCswMScwMCcpL0NyZWF0b3IoSmFzcGVyUmVwb3J0cyBcKENhbGN1bGF0aW9uUHJvdG9jb2xSZXBvcnRcKSkvQ3JlYXRpb25EYXRlKEQ6MjAyMzEyMjIxNDIxMDArMDEnMDAnKS9Qcm9kdWNlcihpVGV4dCA0LjIuMCBieSAxVDNYVCk+PgplbmRvYmoKeHJlZgowIDE5CjAwMDAwMDAwMDAgNjU1MzUgZiAKMDAwMDAwMTkxMyAwMDAwMCBuIAowMDAwMDE3NzkxIDAwMDAwIG4gCjAwMDAwMzM0MDUgMDAwMDAgbiAKMDAwMDAwMDAxNSAwMDAwMCBuIAowMDAwMDMzNTUxIDAwMDAwIG4gCjAwMDAwMDIxNTYgMDAwMDAgbiAKMDAwMDAwMjE5MSAwMDAwMCBuIAowMDAwMDE2NDg1IDAwMDAwIG4gCjAwMDAwMTY2NzcgMDAwMDAgbiAKMDAwMDAxNzE3OCAwMDAwMCBuIAowMDAwMDE3OTMxIDAwMDAwIG4gCjAwMDAwMzIxODUgMDAwMDAgbiAKMDAwMDAzMjM4OCAwMDAwMCBuIAowMDAwMDMyODQ5IDAwMDAwIG4gCjAwMDAwMzM2MTQgMDAwMDAgbiAKMDAwMDAzMzY2OSAwMDAwMCBuIAowMDAwMDMzNzAzIDAwMDAwIG4gCjAwMDAwMzM4MDggMDAwMDAgbiAKdHJhaWxlcgo8PC9JbmZvIDE4IDAgUi9JRCBbPGRhMmY5NTE5MGVlN2NmNmIwNzZmZWY1YzNiMzg4Zjk4PjwwY2VhNmI5NDZhN2QyMTFlMDQwMDRmMjI3NDlmNTEyMz5dL1Jvb3QgMTcgMCBSL1NpemUgMTk+PgpzdGFydHhyZWYKMzM5ODQKJSVFT0YK</ns1:ProtocolData>
                     </ns1:CalcProtocol>
                     <ns1:CalcType>VRO_API</ns1:CalcType>
                  </ns1:CalcResultCommon>
                  <ns1:CalculationSummary>
                     <ns1:SparePartsCosts>
                        <ns1:AllSum>1251.52</ns1:AllSum>
                        <ns1:ConsumablesSurcharge>25.03</ns1:ConsumablesSurcharge>
                        <ns1:TotalSum>1276.55</ns1:TotalSum>
                     </ns1:SparePartsCosts>
                     <ns1:LabourCosts>
                        <ns1:Bodywork>
                           <ns1:Type>CAR BODY</ns1:Type>
                           <ns1:Units>6.34</ns1:Units>
                           <ns1:PricePerUnit>105.0</ns1:PricePerUnit>
                           <ns1:PricePerUnitState/>
                           <ns1:Price>665.7</ns1:Price>
                        </ns1:Bodywork>
                        <ns1:Electric>
                           <ns1:Type>ELECTRIC</ns1:Type>
                           <ns1:Units>0.0</ns1:Units>
                           <ns1:PricePerUnitState/>
                           <ns1:Price>0.0</ns1:Price>
                        </ns1:Electric>
                        <ns1:Mechanic>
                           <ns1:Type>MECHANIC</ns1:Type>
                           <ns1:Units>0.0</ns1:Units>
                           <ns1:PricePerUnitState/>
                           <ns1:Price>0.0</ns1:Price>
                        </ns1:Mechanic>
                        <ns1:DentsPress>
                           <ns1:Type>DENTS PRESS</ns1:Type>
                           <ns1:Units>2.7</ns1:Units>
                           <ns1:PricePerUnit>78.0</ns1:PricePerUnit>
                           <ns1:PricePerUnitState/>
                           <ns1:Price>210.6</ns1:Price>
                        </ns1:DentsPress>
                        <ns1:DentsGlobal>
                           <ns1:Type>DENTS GLOBAL</ns1:Type>
                           <ns1:Units>0.85</ns1:Units>
                           <ns1:PricePerUnit>78.0</ns1:PricePerUnit>
                           <ns1:PricePerUnitState/>
                           <ns1:Price>66.3</ns1:Price>
                        </ns1:DentsGlobal>
                        <ns1:TotalSum>942.6</ns1:TotalSum>
                        <ns1:Works>
                           <ns1:Work>
                              <ns1:Type>CAR BODY</ns1:Type>
                              <ns1:WageLevel>1</ns1:WageLevel>
                              <ns1:Units>6.34</ns1:Units>
                              <ns1:PricePerUnit>105.00</ns1:PricePerUnit>
                              <ns1:Price>665.70</ns1:Price>
                           </ns1:Work>
                           <ns1:Work>
                              <ns1:Type>HAIL DAMAGE PRESS</ns1:Type>
                              <ns1:Units>2.70</ns1:Units>
                              <ns1:PricePerUnit>78.00</ns1:PricePerUnit>
                              <ns1:Price>210.60</ns1:Price>
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
                           <ns1:Units>4.17</ns1:Units>
                           <ns1:PricePerUnit>120.0</ns1:PricePerUnit>
                           <ns1:Price>500.4</ns1:Price>
                        </ns1:Wage>
                        <ns1:TotalWages>500.4</ns1:TotalWages>
                        <ns1:Material>
                           <ns1:FlatPercentage>25.0</ns1:FlatPercentage>
                           <ns1:FlatAmount>125.1</ns1:FlatAmount>
                           <ns1:TotalSum>125.1</ns1:TotalSum>
                           <ns1:SumMaterialCorrected>125.10</ns1:SumMaterialCorrected>
                        </ns1:Material>
                        <ns1:TotalSum>625.5</ns1:TotalSum>
                     </ns1:LacquerCosts>
                     <ns1:TotalNetCosts>2844.65</ns1:TotalNetCosts>
                     <ns1:TotalVAT>540.48</ns1:TotalVAT>
                     <ns1:TotalGrossCosts>3385.13</ns1:TotalGrossCosts>
                     <ns1:TotalNetCorrected>2844.65</ns1:TotalNetCorrected>
                     <ns1:TotalVATCorrected>540.48</ns1:TotalVATCorrected>
                     <ns1:TotalGrossCorrected>3385.13</ns1:TotalGrossCorrected>
                     <ns1:SumNet>2844.65</ns1:SumNet>
                     <ns1:SumGross>3385.13</ns1:SumGross>
                     <ns1:SumSparePartCosts>1276.55</ns1:SumSparePartCosts>
                     <ns1:SumSmallSparePartCosts>25.03</ns1:SumSmallSparePartCosts>
                     <ns1:SumLabourCosts>942.60</ns1:SumLabourCosts>
                     <ns1:MetaPositions>
                        <ns1:MetaPosition key="TIME_UNIT_SYSTEM" value="STD"/>
                        <ns1:MetaPosition key="LACQUER_TIME_UNIT_SYSTEM" value="STD"/>
                     </ns1:MetaPositions>
                  </ns1:CalculationSummary>
                  <ns1:SurchargeSettings/>
                  <ns1:SettingsParameters>
                     <ns1:SettingsParameter key="SHOW_FORD_FINIS_NUMBER" level="company" name="SparePartSettings" value="false"/>
                     <ns1:SettingsParameter key="MANUAL_TIME_IN_HOURS" level="company" name="LabourSettings" value="false"/>
                  </ns1:SettingsParameters>
               </ns1:RepairCalculation>
               <ns1:RepairOrder>
                  <ns1:RepairCoverage/>
                  <ns1:OrderNumber>DAT-TEST_14:20231222142057468</ns1:OrderNumber>
                  <ns1:JobNumber>DAT-TEST_14:20:56,59</ns1:JobNumber>
                  <ns1:Retention>false</ns1:Retention>
                  <ns1:DeclarationOfAssignment>false</ns1:DeclarationOfAssignment>
                  <ns1:CreationDateTime>2023-12-22T14:21:05.824+01:00</ns1:CreationDateTime>
                  <ns1:TypeOfInsurance>1</ns1:TypeOfInsurance>
                  <ns1:InvoiceDate>2023-12-22T14:21:00.086+01:00</ns1:InvoiceDate>
               </ns1:RepairOrder>
               <ns1:InsuranceClaim>false</ns1:InsuranceClaim>
               <ns1:ProcessManagement>
                  <ns1:CustomDataList source="vro_calculation">
                     <ns1:CustomData name="date_registration">2013-11-23T00:00:00+01:00</ns1:CustomData>
                     <ns1:CustomData name="inv_work_total_total">942.6</ns1:CustomData>
                     <ns1:CustomData name="referenceNumber">DAT-TEST_14:20:56,591</ns1:CustomData>
                     <ns1:CustomData name="vehicle_vin">WBADEXTESTSTUB001</ns1:CustomData>
                     <ns1:CustomData name="inv_spareParts_total_total">1276.55</ns1:CustomData>
                     <ns1:CustomData name="date_invoice">2023-12-22T14:21:00+01:00</ns1:CustomData>
                     <ns1:CustomData name="inv_painting_total_total">625.5</ns1:CustomData>
                     <ns1:CustomData name="inv_spareParts_total_parts">1251.52</ns1:CustomData>
                     <ns1:CustomData name="inv_totalPrice">2844.65</ns1:CustomData>
                     <ns1:CustomData name="cpku_kz_ust">0</ns1:CustomData>
                     <ns1:CustomData name="calculationsettings_country">DE</ns1:CustomData>
                     <ns1:CustomData name="inv_totalPrice_vatIncluded">3385.13</ns1:CustomData>
                     <ns1:CustomData name="inv_spareParts_total_smallParts">25.03</ns1:CustomData>
                     <ns1:CustomData name="fhdVersicherungsfall">0</ns1:CustomData>
                     <ns1:CustomData name="inv_painting_total_material">125.1</ns1:CustomData>
                     <ns1:CustomData name="calculationsettings_crossCalculation">0</ns1:CustomData>
                     <ns1:CustomData name="vehicle_registration">ES SM1122</ns1:CustomData>
                     <ns1:CustomData name="address_surname">Test</ns1:CustomData>
                     <ns1:CustomData name="vehicle_mileage">654321</ns1:CustomData>
                     <ns1:CustomData name="inv_painting_total_work">500.4</ns1:CustomData>
                     <ns1:CustomData name="inv_work_total_body">665.7</ns1:CustomData>
                     <ns1:CustomData name="address_country">DE</ns1:CustomData>
                     <ns1:CustomData name="address_firstName">Heiner</ns1:CustomData>
                     <ns1:CustomData name="inv_totalPrice_vat">540.48</ns1:CustomData>
                  </ns1:CustomDataList>
                  <ns1:DamageManagement>
                     <ns1:DamageProcess/>
                  </ns1:DamageManagement>
                  <ns1:AdditionalInsuranceData>
                     <ns1:Email/>
                  </ns1:AdditionalInsuranceData>
               </ns1:ProcessManagement>
            </ns1:Dossier>
         </calculationResult>
      </ns10:calculateContractResponse>
   </S:Body>
</S:Envelope>
