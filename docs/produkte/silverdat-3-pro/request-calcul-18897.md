---
title: "Request calculateN"
topic_id: "18897"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > Reparaturkostenkalkulation ohne Speicherung > Request calculateN"
---

# Request calculateN

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://www.dat.eu/myClaim/soap/v2/VehicleRepairService" xmlns:vxs="http://www.dat.de/vxs">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:calculateN>
         <request>
            <dossiers>
               <vxs:Dossier>
                  <vxs:Description>TestCalculationInMemory</vxs:Description>
                  <vxs:Country>DE</vxs:Country>
                  <vxs:Language>de_DE</vxs:Language>
                  <vxs:DataVersion>1</vxs:DataVersion>
                  <vxs:Currency>EUR</vxs:Currency>
                  <vxs:DatCustomerAddress>
                     <vxs:Title>titleCompany</vxs:Title>
                     <vxs:CompanyName>DAT - Intern</vxs:CompanyName>
                     <vxs:NameLong>Wiederkehrende Testfälle</vxs:NameLong>
                     <vxs:Country>DE</vxs:Country>
                     <vxs:TaxNumber>32132465465</vxs:TaxNumber>
                     <vxs:CustomerNumber>11111111</vxs:CustomerNumber>
                     <vxs:CustomerType>11111111</vxs:CustomerType>
                     <vxs:Street>Hellmuth-Hirth-Str.</vxs:Street>
                     <vxs:StreetNumber>1</vxs:StreetNumber>
                     <vxs:StreetZipCode>73760</vxs:StreetZipCode>
                     <vxs:StreetCity>Ostfildern</vxs:StreetCity>
                     <vxs:PhoneBusiness>+49 711/4503-401</vxs:PhoneBusiness>
                     <vxs:Fax>+49 711/4503-203</vxs:Fax>
                     <vxs:Bank>Landesbank BW</vxs:Bank>
                     <vxs:BIC>251345u1349</vxs:BIC>
                     <vxs:BLZ>9000000000</vxs:BLZ>
                     <vxs:AccountNo>9876543211</vxs:AccountNo>
                     <vxs:IBAN>45897457913</vxs:IBAN>
                     <vxs:UsageFlag>9</vxs:UsageFlag>
                  </vxs:DatCustomerAddress>
                  <vxs:VAT>
                     <vxs:VatAtCalculationTime>19</vxs:VatAtCalculationTime>
                  </vxs:VAT>
                  <vxs:TradingData>
                     <vxs:ClientContactAddresses>
                        <vxs:ClientContactAddress>
                           <vxs:Title>titleCompany</vxs:Title>
                           <vxs:CompanyName>Reese, Sven</vxs:CompanyName>
                           <vxs:NameLong>DAT Werkstatt Deutschland</vxs:NameLong>
                           <vxs:Country>DE</vxs:Country>
                           <vxs:TaxNumber>32132465465</vxs:TaxNumber>
                           <vxs:CustomerNumber>11111111</vxs:CustomerNumber>
                           <vxs:CustomerType>11111111</vxs:CustomerType>
                           <vxs:Street>Hastedtstr</vxs:Street>
                           <vxs:StreetNumber>9</vxs:StreetNumber>
                           <vxs:StreetZipCode>21614</vxs:StreetZipCode>
                           <vxs:StreetCity>Buxtehude</vxs:StreetCity>
                           <vxs:EMail>myDAT@dat.de</vxs:EMail>
                           <vxs:PhoneBusiness>01983645754</vxs:PhoneBusiness>
                           <vxs:Bank>Landesbank BW</vxs:Bank>
                           <vxs:BIC>251345u1349</vxs:BIC>
                           <vxs:BLZ>9000000000</vxs:BLZ>
                           <vxs:AccountNo>9876543211</vxs:AccountNo>
                           <vxs:IBAN>45897457913</vxs:IBAN>
                           <vxs:UsageFlag>9</vxs:UsageFlag>
                        </vxs:ClientContactAddress>
                     </vxs:ClientContactAddresses>
                  </vxs:TradingData>
                  <vxs:RepairCalculation>
                     <vxs:Vehicle>
                        <vxs:VehicleIdentNumber>WBADEXTESTSTUB001</vxs:VehicleIdentNumber>
                        <vxs:DatECode>011301110300002</vxs:DatECode>
                        <vxs:Container>DE006</vxs:Container>
                        <vxs:ConstructionTime>5297</vxs:ConstructionTime>
                        <vxs:ConstructionTimeFrom>5230</vxs:ConstructionTimeFrom>
                        <vxs:ConstructionTimeTo>5350</vxs:ConstructionTimeTo>
                        <vxs:ConstructionTimePriceList>5230</vxs:ConstructionTimePriceList>
                        <vxs:SalesDescription>5er - 520 d DPF Touring</vxs:SalesDescription>
                        <vxs:VehicleTypeName>Pkw, SUV, Kleintransporter</vxs:VehicleTypeName>
                        <vxs:VehicleTypeNameN origin="dat">Pkw, SUV, Kleintransporter</vxs:VehicleTypeNameN>
                        <vxs:ManufacturerName origin="dat">BMW</vxs:ManufacturerName>
                        <vxs:BaseModelName origin="dat">Baureihe 5 Touring (F11)(2010->)</vxs:BaseModelName>
                        <vxs:SubModelName origin="dat">520d</vxs:SubModelName>
                        <vxs:MainTypeGroupName>5</vxs:MainTypeGroupName>
                        <vxs:VehicleType>1</vxs:VehicleType>
                        <vxs:Manufacturer>130</vxs:Manufacturer>
                        <vxs:BaseModel>111</vxs:BaseModel>
                        <vxs:SubModel>30</vxs:SubModel>
                        <vxs:MainTypeGroup>5</vxs:MainTypeGroup>
                        <vxs:IdentificationSource>IDENTIFICATIONSOURCE_VIN</vxs:IdentificationSource>
                        <vxs:VinAccuracy>0</vxs:VinAccuracy>
                        <vxs:ReleaseIndicator>ALL</vxs:ReleaseIndicator>
                        <vxs:KbaNumbersN>
                           <vxs:KbaNumber>0005/AYT</vxs:KbaNumber>
                        </vxs:KbaNumbersN>
                        <vxs:PaintTypes>
                           <vxs:PaintType>05</vxs:PaintType>
                           <vxs:PaintType>09</vxs:PaintType>
                        </vxs:PaintTypes>
                        <vxs:Equipment>
                           <vxs:SeriesEquipment>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>26909</vxs:DatEquipmentId>
                                 <vxs:Description>Airbag Beifahrerseite abschaltbar</vxs:Description>
                                 <vxs:EquipmentGroup>AIR2</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>26803</vxs:DatEquipmentId>
                                 <vxs:Description>Airbag Fahrer-/Beifahrerseite</vxs:Description>
                                 <vxs:EquipmentGroup>AIR1</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>34704</vxs:DatEquipmentId>
                                 <vxs:Description>Aktive Kopfstützen</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>10715</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>8TF</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>AKTIVER FUSSGAENGERSCHUTZ.</vxs:ManufacturerDescription>
                                 <vxs:Description>Aktive Motorhaube</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>40000</vxs:DatEquipmentId>
                                 <vxs:Description>Anti-Blockier-System (ABS)</vxs:Description>
                                 <vxs:EquipmentGroup>ABS</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>18604</vxs:DatEquipmentId>
                                 <vxs:Description>Automatische Fahrlichtschaltung</vxs:Description>
                                 <vxs:EquipmentGroup>AUFL</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>24999</vxs:DatEquipmentId>
                                 <vxs:Description>AUX-IN-Anschluss (AUX-IN)</vxs:Description>
                                 <vxs:EquipmentGroup>MP3A</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>15200</vxs:DatEquipmentId>
                                 <vxs:Description>Außenspiegel elektr. verstell- und heizbar</vxs:Description>
                                 <vxs:EquipmentGroup>AUSP</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>25702</vxs:DatEquipmentId>
                                 <vxs:Description>Außentemperaturanzeige</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>18505</vxs:DatEquipmentId>
                                 <vxs:Description>Bi-Xenon-Scheinwerfer</vxs:Description>
                                 <vxs:EquipmentGroup>XELI</vxs:EquipmentGroup>
                                 <vxs:ContainedEquipmentPositions>
                                    <vxs:EquipmentPosition>
                                       <vxs:DatEquipmentId>18913</vxs:DatEquipmentId>
                                       <vxs:Description>Tagfahrlicht LED</vxs:Description>
                                       <vxs:EquipmentGroup>TFAL</vxs:EquipmentGroup>
                                    </vxs:EquipmentPosition>
                                    <vxs:EquipmentPosition>
                                       <vxs:DatEquipmentId>18940</vxs:DatEquipmentId>
                                       <vxs:Description>Blinkleuchten LED</vxs:Description>
                                    </vxs:EquipmentPosition>
                                    <vxs:EquipmentPosition>
                                       <vxs:DatEquipmentId>19000</vxs:DatEquipmentId>
                                       <vxs:Description>Scheinwerfer-Reinigungsanlage (SRA)</vxs:Description>
                                       <vxs:EquipmentGroup>SWRA</vxs:EquipmentGroup>
                                    </vxs:EquipmentPosition>
                                 </vxs:ContainedEquipmentPositions>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>25508</vxs:DatEquipmentId>
                                 <vxs:Description>Bordcomputer</vxs:Description>
                                 <vxs:EquipmentGroup>COMP</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>40801</vxs:DatEquipmentId>
                                 <vxs:Description>Bremsassistent</vxs:Description>
                                 <vxs:EquipmentGroup>FA01</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>40050</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>1CD</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>BRAKE ENERGY REGENERATION</vxs:ManufacturerDescription>
                                 <vxs:Description>Bremsenergierückgewinnung (Rekuperationssystem)</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>25606</vxs:DatEquipmentId>
                                 <vxs:Description>Check-Control-System</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>25300</vxs:DatEquipmentId>
                                 <vxs:Description>Drehzahlmesser</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>18898</vxs:DatEquipmentId>
                                 <vxs:Description>Dynamische Bremsleuchte</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>70100</vxs:DatEquipmentId>
                                 <vxs:Description>Dynamische Stabilitäts-Control (DSC)</vxs:Description>
                                 <vxs:EquipmentGroup>ESP</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>11406</vxs:DatEquipmentId>
                                 <vxs:Description>Exterieurumfänge Wagenfarbe</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>70518</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>4U2</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>FAHRERLEBNISSCHALTER INKL. ECO PRO</vxs:ManufacturerDescription>
                                 <vxs:Description>Fahrassistenz-System: Fahrerlebnisschalter</vxs:Description>
                                 <vxs:EquipmentGroup>FA22</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>35003</vxs:DatEquipmentId>
                                 <vxs:Description>Fensterheber elektrisch vorn + hinten</vxs:Description>
                                 <vxs:EquipmentGroup>FH4</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>24833</vxs:DatEquipmentId>
                                 <vxs:Description>Freisprecheinrichtung mit USB-Schnittstelle</vxs:Description>
                                 <vxs:EquipmentGroup>TEL3</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>28402</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>423</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>FUSSMATTEN IN VELOURS</vxs:ManufacturerDescription>
                                 <vxs:Description>Fußmatten Velours</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>27605</vxs:DatEquipmentId>
                                 <vxs:Description>Gepäckraum-Abtrennung (Netz)</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>27400</vxs:DatEquipmentId>
                                 <vxs:Description>Gepäckraumabdeckung / Rollo</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>26710</vxs:DatEquipmentId>
                                 <vxs:Description>Geschwindigkeits-Regelanlage mit Bremsfunktion</vxs:Description>
                                 <vxs:EquipmentGroup>TEMP</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>39402</vxs:DatEquipmentId>
                                 <vxs:Description>Getränkehalter vorn und hinten</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>35506</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>316</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>AUTOMATISCHE HECKKLAPPENBETAETIGUNG</vxs:ManufacturerDescription>
                                 <vxs:Description>Heckklappenbetätigung automatisch</vxs:Description>
                                 <vxs:EquipmentGroup>HKEL</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>19300</vxs:DatEquipmentId>
                                 <vxs:Description>Heckscheibenwischer</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>39308</vxs:DatEquipmentId>
                                 <vxs:Description>Isofix-Aufnahmen für Kindersitz an Rücksitz</vxs:Description>
                                 <vxs:EquipmentGroup>KISI</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>10005</vxs:DatEquipmentId>
                                 <vxs:Description>Karosserie: 5-türig</vxs:Description>
                                 <vxs:EquipmentClass>2</vxs:EquipmentClass>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>26805</vxs:DatEquipmentId>
                                 <vxs:Description>Kopf-Airbag-System hinten</vxs:Description>
                                 <vxs:EquipmentGroup>AIR4</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>26804</vxs:DatEquipmentId>
                                 <vxs:Description>Kopf-Airbag-System vorn</vxs:Description>
                                 <vxs:EquipmentGroup>AIR4</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>69007</vxs:DatEquipmentId>
                                 <vxs:Description>Lenkrad (Leder) mit Multifunktion</vxs:Description>
                                 <vxs:EquipmentGroup>LEN2</vxs:EquipmentGroup>
                                 <vxs:ContainedEquipmentPositions>
                                    <vxs:EquipmentPosition>
                                       <vxs:DatEquipmentId>69505</vxs:DatEquipmentId>
                                       <vxs:Description>Lenksäule (Lenkrad) mechan. verstellbar</vxs:Description>
                                    </vxs:EquipmentPosition>
                                 </vxs:ContainedEquipmentPositions>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>69505</vxs:DatEquipmentId>
                                 <vxs:Description>Lenksäule (Lenkrad) mechan. verstellbar</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>48535</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>2K1</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>LM RAEDER V-SPEICHE 236</vxs:ManufacturerDescription>
                                 <vxs:Description>LM-Felgen 8x17 (V-Speiche 236)</vxs:Description>
                                 <vxs:EquipmentGroup>ALU</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>42905</vxs:DatEquipmentId>
                                 <vxs:Description>Luftfederung Hinterachse</vxs:Description>
                                 <vxs:EquipmentGroup>LUFT</vxs:EquipmentGroup>
                                 <vxs:ContainedEquipmentPositions>
                                    <vxs:EquipmentPosition>
                                       <vxs:DatEquipmentId>42805</vxs:DatEquipmentId>
                                       <vxs:Description>Niveauregulierung</vxs:Description>
                                       <vxs:EquipmentGroup>NIV</vxs:EquipmentGroup>
                                    </vxs:EquipmentPosition>
                                 </vxs:ContainedEquipmentPositions>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>27300</vxs:DatEquipmentId>
                                 <vxs:Description>Mittelarmlehne hinten</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>27202</vxs:DatEquipmentId>
                                 <vxs:Description>Mittelarmlehne vorn</vxs:Description>
                                 <vxs:EquipmentGroup>MALV</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>87410</vxs:DatEquipmentId>
                                 <vxs:Description>Motor 2,0 Ltr. - 135 kW Turbodiesel KAT (N 47 T)</vxs:Description>
                                 <vxs:EquipmentClass>1</vxs:EquipmentClass>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>27309</vxs:DatEquipmentId>
                                 <vxs:Description>Multifunktionsarmlehne im Fond</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>42805</vxs:DatEquipmentId>
                                 <vxs:Description>Niveauregulierung</vxs:Description>
                                 <vxs:EquipmentGroup>NIV</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>77015</vxs:DatEquipmentId>
                                 <vxs:Description>NOx-Speicherkatalysator (BMW Blue Performance)</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>40803</vxs:DatEquipmentId>
                                 <vxs:Description>Parkbremse elektrisch</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>62004</vxs:DatEquipmentId>
                                 <vxs:Description>Reifen 225/55 R17 ..Z</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>68802</vxs:DatEquipmentId>
                                 <vxs:Description>Reifen-Reparaturset (Mobility-Pack)</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>25906</vxs:DatEquipmentId>
                                 <vxs:Description>Reifenpannen-Anzeige</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>77602</vxs:DatEquipmentId>
                                 <vxs:Description>Rußpartikelfilter</vxs:Description>
                                 <vxs:EquipmentGroup>DPF</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>33508</vxs:DatEquipmentId>
                                 <vxs:Description>Rücksitzlehne geteilt/klappbar</vxs:Description>
                                 <vxs:EquipmentGroup>SITH</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>77227</vxs:DatEquipmentId>
                                 <vxs:Description>Schadstoffarm nach Abgasnorm Euro 6</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>19102</vxs:DatEquipmentId>
                                 <vxs:Description>Scheibenwaschdüsen heizbar</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>19101</vxs:DatEquipmentId>
                                 <vxs:Description>Scheibenwischer mit Regensensor</vxs:Description>
                                 <vxs:EquipmentGroup>SWRE</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>19000</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>502</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>SCHEINWERFER-WASCHANLAGE</vxs:ManufacturerDescription>
                                 <vxs:Description>Scheinwerfer-Reinigungsanlage (SRA)</vxs:Description>
                                 <vxs:EquipmentGroup>SWRA</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>26903</vxs:DatEquipmentId>
                                 <vxs:Description>Seitenairbag vorn</vxs:Description>
                                 <vxs:EquipmentGroup>AIR3</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>25151</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>6AE</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>TELESERVICES</vxs:ManufacturerDescription>
                                 <vxs:Description>Service-System: Intelligenter Notruf inkl. TeleServices</vxs:Description>
                                 <vxs:EquipmentGroup>FA10</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>69811</vxs:DatEquipmentId>
                                 <vxs:Description>Servolenkung Servotronic</vxs:Description>
                                 <vxs:EquipmentGroup>SL</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>32811</vxs:DatEquipmentId>
                                 <vxs:Description>Sitze vorn teilelektr. verstellbar</vxs:Description>
                                 <vxs:EquipmentGroup>SITE</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>35408</vxs:DatEquipmentId>
                                 <vxs:Description>Soft-Close-Automatik für Kofferraum / Heckklappe</vxs:Description>
                                 <vxs:EquipmentGroup>HKEL</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>35513</vxs:DatEquipmentId>
                                 <vxs:Description>Start-Stop-Knopf</vxs:Description>
                                 <vxs:EquipmentGroup>MSSA</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>77601</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>1CC</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>AUTO START STOP FUNKTION</vxs:ManufacturerDescription>
                                 <vxs:Description>Start/Stop-Anlage (Funktion)</vxs:Description>
                                 <vxs:EquipmentGroup>MSSA</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>39016</vxs:DatEquipmentId>
                                 <vxs:Description>Steckdose (12V-Anschluß) 3-fach</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>73017</vxs:DatEquipmentId>
                                 <vxs:Description>Vlies-Batterie 80 Ah (AGM)</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>38105</vxs:DatEquipmentId>
                                 <vxs:Description>Wegfahrsperre</vxs:Description>
                                 <vxs:EquipmentGroup>WFS</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>22218</vxs:DatEquipmentId>
                                 <vxs:Description>Wärme-/Sonnenschutzverglasung kombiniert (hinten abgedunkelt)</vxs:Description>
                                 <vxs:EquipmentGroup>WDG</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>35301</vxs:DatEquipmentId>
                                 <vxs:Description>Zentralverriegelung mit Fernbedienung</vxs:Description>
                                 <vxs:EquipmentGroup>ZV</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                           </vxs:SeriesEquipment>
                           <vxs:SpecialEquipment>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>37603</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>4UR</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>AMBIENTES LICHT</vxs:ManufacturerDescription>
                                 <vxs:Description>Ambiente-Beleuchtung</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>25804</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>609</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>NAVIGATIONSSYSTEM PROFESSIONAL</vxs:ManufacturerDescription>
                                 <vxs:Description>Audio-Navigationssystem Professional</vxs:Description>
                                 <vxs:EquipmentGroup>GPS</vxs:EquipmentGroup>
                                 <vxs:ContainedEquipmentPositions>
                                    <vxs:EquipmentPosition>
                                       <vxs:DatEquipmentId>24116</vxs:DatEquipmentId>
                                       <vxs:Description>Audiosystem BMW Professional (Radio / DVD-Laufwerk MP3-fähig)</vxs:Description>
                                       <vxs:EquipmentGroup>CD</vxs:EquipmentGroup>
                                    </vxs:EquipmentPosition>
                                    <vxs:EquipmentPosition>
                                       <vxs:DatEquipmentId>24709</vxs:DatEquipmentId>
                                       <vxs:Description>Sprachbediensystem</vxs:Description>
                                       <vxs:EquipmentGroup>TEL4</vxs:EquipmentGroup>
                                    </vxs:EquipmentPosition>
                                 </vxs:ContainedEquipmentPositions>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>8702</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>760</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>INDIVIDUAL HOCHGLANZ SHADOW LINE</vxs:ManufacturerDescription>
                                 <vxs:Description>Außenausstattung: Shadow-Line Hochglanz</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>25930</vxs:DatEquipmentId>
                                 <vxs:Description>Control-Display mit Farbmonitor (9,2 Zoll)</vxs:Description>
                                 <vxs:EquipmentGroup>MONM</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>27810</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>775</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>INDIVIDUAL DACHHIMMEL ANTHRAZIT</vxs:ManufacturerDescription>
                                 <vxs:Description>Dachhimmel Anthrazit (BMW Individual)</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>16198</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>3MC</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>INDIV.DACHRELING HOCHGL.SHADOW LINE</vxs:ManufacturerDescription>
                                 <vxs:Description>Dachreling Hochglanz Shadow-Line</vxs:Description>
                                 <vxs:EquipmentGroup>DARE</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>25704</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>8TH</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>SPEED LIMIT INFO</vxs:ManufacturerDescription>
                                 <vxs:Description>Fahrassistenz-System: Speed-Limit-Anzeige</vxs:Description>
                                 <vxs:EquipmentGroup>FA28</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>22505</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>358</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>KLIMAKOMFORT-FRONTSCHEIBE</vxs:ManufacturerDescription>
                                 <vxs:Description>Frontscheibe (Ausführung: Klimakomfort)</vxs:Description>
                                 <vxs:EquipmentGroup>WDG</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>75914</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>205</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>AUTOMATIC GETRIEBE</vxs:ManufacturerDescription>
                                 <vxs:Description>Getriebe Automatik - mit Steptronic (8-Stufen)</vxs:Description>
                                 <vxs:EquipmentGroup>AG2</vxs:EquipmentGroup>
                                 <vxs:EquipmentClass>11</vxs:EquipmentClass>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>25204</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>610</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>HEAD-UP DISPLAY</vxs:ManufacturerDescription>
                                 <vxs:Description>Head-up-Display</vxs:Description>
                                 <vxs:EquipmentGroup>HUD</vxs:EquipmentGroup>
                                 <vxs:ContainedEquipmentPositions>
                                    <vxs:EquipmentPosition>
                                       <vxs:DatEquipmentId>25413</vxs:DatEquipmentId>
                                       <vxs:Description>Instrumentenkombination (erweiterter Umfang)</vxs:Description>
                                    </vxs:EquipmentPosition>
                                    <vxs:EquipmentPosition>
                                       <vxs:DatEquipmentId>25930</vxs:DatEquipmentId>
                                       <vxs:Description>Control-Display mit Farbmonitor (9,2 Zoll)</vxs:Description>
                                       <vxs:EquipmentGroup>MONM</vxs:EquipmentGroup>
                                    </vxs:EquipmentPosition>
                                 </vxs:ContainedEquipmentPositions>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>24607</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>676</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>HIFI LAUTSPRECHERSYSTEM</vxs:ManufacturerDescription>
                                 <vxs:Description>HiFi-Lautsprechersystem</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>31408</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>4B9</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>INT.LEISTE ALUMINIUM FEINSCHLIFF</vxs:ManufacturerDescription>
                                 <vxs:Description>Innenausstattung: Interieurleisten Aluminium Längsschliff fein</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>37901</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>431</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>INNENSPIEGEL,AUTOMATISCH ABBLENDEND</vxs:ManufacturerDescription>
                                 <vxs:Description>Innenspiegel mit Abblendautomatik</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>25413</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>6WA</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>INSTRUMENTENKOMBI. M. ERW. UMF.</vxs:ManufacturerDescription>
                                 <vxs:Description>Instrumentenkombination (erweiterter Umfang)</vxs:Description>
                                 <vxs:ContainedEquipmentPositions>
                                    <vxs:EquipmentPosition>
                                       <vxs:DatEquipmentId>25930</vxs:DatEquipmentId>
                                       <vxs:Description>Control-Display mit Farbmonitor (9,2 Zoll)</vxs:Description>
                                       <vxs:EquipmentGroup>MONM</vxs:EquipmentGroup>
                                    </vxs:EquipmentPosition>
                                 </vxs:ContainedEquipmentPositions>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>28982</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>534</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>KLIMAAUTOMATIK</vxs:ManufacturerDescription>
                                 <vxs:Description>Klimaautomatik 2-Zonen mit autom. Umluft-Control, erweiterter Umfang</vxs:Description>
                                 <vxs:EquipmentGroup>KLI2</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>33403</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>488</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>LORDOSENSTUETZE FAHRER/BEIFAHRER</vxs:ManufacturerDescription>
                                 <vxs:Description>Lendenwirbelstütze Sitz vorn links und rechts, elektr. verstellbar</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>77240</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>1CB</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>CO2 UMFANG</vxs:ManufacturerDescription>
                                 <vxs:Description>Modellvariante CO2-Umfang (Code 1CB)</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>18313</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>5A1</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>LED-NEBELSCHEINWERFER</vxs:ManufacturerDescription>
                                 <vxs:Description>Nebelscheinwerfer LED</vxs:Description>
                                 <vxs:EquipmentGroup>BEL</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>16302</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>402</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>PANORAMA GLASDACH</vxs:ManufacturerDescription>
                                 <vxs:Description>Panoramadach (Glas)</vxs:Description>
                                 <vxs:EquipmentGroup>SD2</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>25802</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>508</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>PARK DISTANCE CONTROL (PDC)</vxs:ManufacturerDescription>
                                 <vxs:Description>Park-Distance-Control (PDC)</vxs:Description>
                                 <vxs:EquipmentGroup>PDC1</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>30301</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>LCSW</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>LEDER DAKOTA/SCHWARZ</vxs:ManufacturerDescription>
                                 <vxs:Description>Sitzbezug / Polsterung: Leder Dakota</vxs:Description>
                                 <vxs:EquipmentGroup>LEDE</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>29500</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>494</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>SITZHEIZUNG FUER FAHRER/BEIFAHRER</vxs:ManufacturerDescription>
                                 <vxs:Description>Sitzheizung vorn</vxs:Description>
                                 <vxs:EquipmentGroup>SITB</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>22102</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>761</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>INDIVIDUAL SONNENSCHUTZVERGLASUNG</vxs:ManufacturerDescription>
                                 <vxs:Description>Sonnenschutzverglasung (hinten abgedunkelt, BMW Individual)</vxs:Description>
                                 <vxs:EquipmentGroup>WDG</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                           </vxs:SpecialEquipment>
                        </vxs:Equipment>
                        <vxs:DATECodeEquipment>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>96508</vxs:DatEquipmentId>
                              <vxs:Description>Motor 2,0 Ltr. - 135 kW Turbodiesel</vxs:Description>
                              <vxs:EquipmentClass>1</vxs:EquipmentClass>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>10005</vxs:DatEquipmentId>
                              <vxs:Description>Karosserie: 5-türig</vxs:Description>
                              <vxs:EquipmentClass>2</vxs:EquipmentClass>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>75914</vxs:DatEquipmentId>
                              <vxs:Description>Getriebe Automatik - mit Steptronic (8-Stufen)</vxs:Description>
                              <vxs:EquipmentClass>11</vxs:EquipmentClass>
                           </vxs:EquipmentPosition>
                        </vxs:DATECodeEquipment>
                        <vxs:VINResult>
                           <vxs:VinInterfaceVersion>2.5</vxs:VinInterfaceVersion>
                           <vxs:VINECodes>
                              <vxs:VINECode>
                                 <vxs:Sign>0</vxs:Sign>
                                 <vxs:Country>DE</vxs:Country>
                                 <vxs:VehicleTypeKey>1</vxs:VehicleTypeKey>
                                 <vxs:ManufacturerKey>130</vxs:ManufacturerKey>
                                 <vxs:VehicleMainTypeKey>111</vxs:VehicleMainTypeKey>
                                 <vxs:VehicleSubTypeKey>30</vxs:VehicleSubTypeKey>
                                 <vxs:VehicleSubTypeVariantKey>2</vxs:VehicleSubTypeVariantKey>
                                 <vxs:ConstructionTimeMin>5250</vxs:ConstructionTimeMin>
                                 <vxs:ConstructionTime>5297</vxs:ConstructionTime>
                                 <vxs:ConstructionTimeEdge>4830</vxs:ConstructionTimeEdge>
                                 <vxs:ConstructionTimeProd>5297</vxs:ConstructionTimeProd>
                                 <vxs:ConstructionTimePriceList>5230</vxs:ConstructionTimePriceList>
                                 <vxs:VINContainers>
                                    <vxs:VINContainer>
                                       <vxs:Container>006</vxs:Container>
                                       <vxs:VehicleTypeKey>5</vxs:VehicleTypeKey>
                                       <vxs:ManufacturerKey>130</vxs:ManufacturerKey>
                                       <vxs:VehicleMainTypeKey>3260</vxs:VehicleMainTypeKey>
                                       <vxs:VehicleSubTypeKey>121</vxs:VehicleSubTypeKey>
                                       <vxs:VehicleConstructionTime>5297</vxs:VehicleConstructionTime>
                                    </vxs:VINContainer>
                                 </vxs:VINContainers>
                              </vxs:VINECode>
                           </vxs:VINECodes>
                           <vxs:VINEquipments>
                              <vxs:VINEquipment>
                                 <vxs:ShortName>Model: 520D (F11)</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>1CA</vxs:ManufacturerCode>
                                 <vxs:ShortName>SELEKTION COP RELEVANTER FAHRZEUGE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>548</vxs:ManufacturerCode>
                                 <vxs:ShortName>KILOMETERTACHO</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>668U</vxs:ManufacturerCode>
                                 <vxs:ShortName>SCHWARZ 2</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>698</vxs:ManufacturerCode>
                                 <vxs:ShortName>AREA-CODE 2</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>851</vxs:ManufacturerCode>
                                 <vxs:ShortName>SPRACHVERSION DEUTSCH</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>8KA</vxs:ManufacturerCode>
                                 <vxs:ShortName>OELWARTUNGSINT. 30.000KM/24MONATE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>8V1</vxs:ManufacturerCode>
                                 <vxs:ShortName>HINWEISSCHILD NCAP</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>9AA</vxs:ManufacturerCode>
                                 <vxs:ShortName>AUSSENHAUTSCHUTZ</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>Country:DE</vxs:ManufacturerCode>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>N47T/2.00/135</vxs:ManufacturerCode>
                                 <vxs:ShortName>2.00L / 135kW</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>U</vxs:ManufacturerCode>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>VIN10:0</vxs:ManufacturerCode>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>VIN11:D</vxs:ManufacturerCode>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>WHC:WBA</vxs:ManufacturerCode>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>81</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>230</vxs:ManufacturerCode>
                                 <vxs:ShortName>EU SPEZIFISCHE ZUSATZUMFAENGE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>789</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>320</vxs:ManufacturerCode>
                                 <vxs:ShortName>MODELLSCHRIFTZUG ENTFALL</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>2707</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>9BD</vxs:ManufacturerCode>
                                 <vxs:ShortName>BUSINESS PAKET DE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>8701</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>760</vxs:ManufacturerCode>
                                 <vxs:ShortName>INDIVIDUAL HOCHGLANZ SHADOW LINE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>8702</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>760</vxs:ManufacturerCode>
                                 <vxs:ShortName>INDIVIDUAL HOCHGLANZ SHADOW LINE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>10715</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>8TF</vxs:ManufacturerCode>
                                 <vxs:ShortName>AKTIVER FUSSGAENGERSCHUTZ.</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>16198</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>3MC</vxs:ManufacturerCode>
                                 <vxs:ShortName>INDIV.DACHRELING HOCHGL.SHADOW LINE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>16302</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>402</vxs:ManufacturerCode>
                                 <vxs:ShortName>PANORAMA GLASDACH</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>18313</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>5A1</vxs:ManufacturerCode>
                                 <vxs:ShortName>LED-NEBELSCHEINWERFER</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>19000</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>502</vxs:ManufacturerCode>
                                 <vxs:ShortName>SCHEINWERFER-WASCHANLAGE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>19001</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>502</vxs:ManufacturerCode>
                                 <vxs:ShortName>SCHEINWERFER-WASCHANLAGE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>19002</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>502</vxs:ManufacturerCode>
                                 <vxs:ShortName>SCHEINWERFER-WASCHANLAGE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>19004</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>502</vxs:ManufacturerCode>
                                 <vxs:ShortName>SCHEINWERFER-WASCHANLAGE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>22102</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>761</vxs:ManufacturerCode>
                                 <vxs:ShortName>INDIVIDUAL SONNENSCHUTZVERGLASUNG</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>22505</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>358</vxs:ManufacturerCode>
                                 <vxs:ShortName>KLIMAKOMFORT-FRONTSCHEIBE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>22507</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>358</vxs:ManufacturerCode>
                                 <vxs:ShortName>KLIMAKOMFORT-FRONTSCHEIBE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>24607</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>676</vxs:ManufacturerCode>
                                 <vxs:ShortName>HIFI LAUTSPRECHERSYSTEM</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>24826</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>6NH</vxs:ManufacturerCode>
                                 <vxs:ShortName>FREISPRECHEIN. M. USB-SCHNITTSTELLE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>25051</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>6NR</vxs:ManufacturerCode>
                                 <vxs:ShortName>APPS</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>25150</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>6AK</vxs:ManufacturerCode>
                                 <vxs:ShortName>CONNECTEDDRIVE SERVICES</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>25151</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>6AC</vxs:ManufacturerCode>
                                 <vxs:ShortName>INTELLIGENTER NOTRUF</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>25151</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>6AE</vxs:ManufacturerCode>
                                 <vxs:ShortName>TELESERVICES</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>25204</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>610</vxs:ManufacturerCode>
                                 <vxs:ShortName>HEAD-UP DISPLAY</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>25413</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>6WA</vxs:ManufacturerCode>
                                 <vxs:ShortName>INSTRUMENTENKOMBI. M. ERW. UMF.</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>25704</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>8TH</vxs:ManufacturerCode>
                                 <vxs:ShortName>SPEED LIMIT INFO</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>25802</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>508</vxs:ManufacturerCode>
                                 <vxs:ShortName>PARK DISTANCE CONTROL (PDC)</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>25804</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>609</vxs:ManufacturerCode>
                                 <vxs:ShortName>NAVIGATIONSSYSTEM PROFESSIONAL</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>25881</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>6AM</vxs:ManufacturerCode>
                                 <vxs:ShortName>REAL TIME TRAFFIC INFORMATION</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>27804</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>775</vxs:ManufacturerCode>
                                 <vxs:ShortName>INDIVIDUAL DACHHIMMEL ANTHRAZIT</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>27810</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>775</vxs:ManufacturerCode>
                                 <vxs:ShortName>INDIVIDUAL DACHHIMMEL ANTHRAZIT</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>28402</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>423</vxs:ManufacturerCode>
                                 <vxs:ShortName>FUSSMATTEN IN VELOURS</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>28807</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>534</vxs:ManufacturerCode>
                                 <vxs:ShortName>KLIMAAUTOMATIK</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>28901</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>534</vxs:ManufacturerCode>
                                 <vxs:ShortName>KLIMAAUTOMATIK</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>28903</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>534</vxs:ManufacturerCode>
                                 <vxs:ShortName>KLIMAAUTOMATIK</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>28980</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>534</vxs:ManufacturerCode>
                                 <vxs:ShortName>KLIMAAUTOMATIK</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>28982</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>534</vxs:ManufacturerCode>
                                 <vxs:ShortName>KLIMAAUTOMATIK</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>28983</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>534</vxs:ManufacturerCode>
                                 <vxs:ShortName>KLIMAAUTOMATIK</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>29500</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>494</vxs:ManufacturerCode>
                                 <vxs:ShortName>SITZHEIZUNG FUER FAHRER/BEIFAHRER</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>29505</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>494</vxs:ManufacturerCode>
                                 <vxs:ShortName>SITZHEIZUNG FUER FAHRER/BEIFAHRER</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>30301</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>LCSW</vxs:ManufacturerCode>
                                 <vxs:ShortName>LEDER DAKOTA/SCHWARZ</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>31408</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>4B9</vxs:ManufacturerCode>
                                 <vxs:ShortName>INT.LEISTE ALUMINIUM FEINSCHLIFF</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>33303</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>488</vxs:ManufacturerCode>
                                 <vxs:ShortName>LORDOSENSTUETZE FAHRER/BEIFAHRER</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>33304</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>488</vxs:ManufacturerCode>
                                 <vxs:ShortName>LORDOSENSTUETZE FAHRER/BEIFAHRER</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>33305</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>488</vxs:ManufacturerCode>
                                 <vxs:ShortName>LORDOSENSTUETZE FAHRER/BEIFAHRER</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>33306</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>488</vxs:ManufacturerCode>
                                 <vxs:ShortName>LORDOSENSTUETZE FAHRER/BEIFAHRER</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>33307</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>488</vxs:ManufacturerCode>
                                 <vxs:ShortName>LORDOSENSTUETZE FAHRER/BEIFAHRER</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>33403</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>488</vxs:ManufacturerCode>
                                 <vxs:ShortName>LORDOSENSTUETZE FAHRER/BEIFAHRER</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>35506</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>316</vxs:ManufacturerCode>
                                 <vxs:ShortName>AUTOMATISCHE HECKKLAPPENBETAETIGUNG</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>37603</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>4UR</vxs:ManufacturerCode>
                                 <vxs:ShortName>AMBIENTES LICHT</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>37901</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>431</vxs:ManufacturerCode>
                                 <vxs:ShortName>INNENSPIEGEL,AUTOMATISCH ABBLENDEND</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>38999</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>428</vxs:ManufacturerCode>
                                 <vxs:ShortName>WARNDREIECK</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>39011</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>575</vxs:ManufacturerCode>
                                 <vxs:ShortName>ZUSAETZLICHE 12-V-STECKDOSE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>40050</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>1CD</vxs:ManufacturerCode>
                                 <vxs:ShortName>BRAKE ENERGY REGENERATION</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>48535</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>2K1</vxs:ManufacturerCode>
                                 <vxs:ShortName>LM RAEDER V-SPEICHE 236</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>70518</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>4U2</vxs:ManufacturerCode>
                                 <vxs:ShortName>FAHRERLEBNISSCHALTER INKL. ECO PRO</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>75500</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>205</vxs:ManufacturerCode>
                                 <vxs:ShortName>AUTOMATIC GETRIEBE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>75503</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>205</vxs:ManufacturerCode>
                                 <vxs:ShortName>AUTOMATIC GETRIEBE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>75505</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>205</vxs:ManufacturerCode>
                                 <vxs:ShortName>AUTOMATIC GETRIEBE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>75605</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>205</vxs:ManufacturerCode>
                                 <vxs:ShortName>AUTOMATIC GETRIEBE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>75608</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>205</vxs:ManufacturerCode>
                                 <vxs:ShortName>AUTOMATIC GETRIEBE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>75609</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>205</vxs:ManufacturerCode>
                                 <vxs:ShortName>AUTOMATIC GETRIEBE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>75904</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>205</vxs:ManufacturerCode>
                                 <vxs:ShortName>AUTOMATIC GETRIEBE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>75906</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>205</vxs:ManufacturerCode>
                                 <vxs:ShortName>AUTOMATIC GETRIEBE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>75913</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>205</vxs:ManufacturerCode>
                                 <vxs:ShortName>AUTOMATIC GETRIEBE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>75914</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>205</vxs:ManufacturerCode>
                                 <vxs:ShortName>AUTOMATIC GETRIEBE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>77240</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>1CB</vxs:ManufacturerCode>
                                 <vxs:ShortName>CO2 UMFANG</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>77601</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>1CC</vxs:ManufacturerCode>
                                 <vxs:ShortName>AUTO START STOP FUNKTION</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>99954</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>801</vxs:ManufacturerCode>
                                 <vxs:ShortName>DEUTSCHLAND-AUSFUEHRUNG</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>99954</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>879</vxs:ManufacturerCode>
                                 <vxs:ShortName>DEUTSCH / BORDLITERATUR</vxs:ShortName>
                              </vxs:VINEquipment>
                           </vxs:VINEquipments>
                           <vxs:VINColors>
                              <vxs:VINColor>
                                 <vxs:ColorID>A1</vxs:ColorID>
                                 <vxs:Code>668</vxs:Code>
                                 <vxs:Description>SCHWARZ 2</vxs:Description>
                                 <vxs:StandardColor>9</vxs:StandardColor>
                                 <vxs:PaintType>05|09</vxs:PaintType>
                              </vxs:VINColor>
                              <vxs:VINColor>
                                 <vxs:ColorID>I1</vxs:ColorID>
                                 <vxs:Code>LCSW</vxs:Code>
                                 <vxs:Description>LEDER DAKOTA/SCHWARZ</vxs:Description>
                              </vxs:VINColor>
                              <vxs:VINColor>
                                 <vxs:ColorID>PM</vxs:ColorID>
                                 <vxs:Code/>
                                 <vxs:Description>LEDER DAKOTA</vxs:Description>
                              </vxs:VINColor>
                              <vxs:VINColor>
                                 <vxs:ColorID>PF</vxs:ColorID>
                                 <vxs:Code/>
                                 <vxs:Description>SCHWARZ</vxs:Description>
                              </vxs:VINColor>
                           </vxs:VINColors>
                           <vxs:VINVehicle>
                              <vxs:VINumber>
                                 <vxs:VinCode>WBADEXTESTSTUB001</vxs:VinCode>
                              </vxs:VINumber>
                              <vxs:ManufacturerCarCode>5J41</vxs:ManufacturerCarCode>
                           </vxs:VINVehicle>
                        </vxs:VINResult>
                        <vxs:TokenOfVinResult>eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJkYXQiLCJ0aW1lc3RhbXAiOjE2NjU2NzY1NDgyODIsImN1c3RvbWVyIjoiMTM0MDc4OSIsImludGVyZmFjZVBhcnRuZXIiOiIxMzQwNzg5IiwidmluUmVzdWx0SGFzaCI6Imhhc2gwMV8tMTI1Mjc0OTYwMSJ9.sD5gJVJYE7pQSNNY152tBVmeR4g1gCFFyoRQaKq-nvM</vxs:TokenOfVinResult>
                     </vxs:Vehicle>
                     <vxs:ProcedureRelatedParameters>
                        <vxs:ProcedureRelatedParameter factor="CalculationFactor" attribute="vatRate" type="Double">19.0</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="CalculationFactor" attribute="referenceSetName" type="String">DAT-Default-CalcPro</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="CalculationFactor" attribute="biwOptimizationMode" type="BiwOptimizationMode">AUTOMATIC</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="CalculationFactor" attribute="showLongWorkStrings" type="Boolean">true</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="CalculationFactor" attribute="selectedLacquerMethod" type="LacquerMethod">EURO_LACQUER</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="CalculationFactor" attribute="crossSeries" type="CrossSeriesState">NO</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="CalculationFactor" attribute="timeUnit" type="TimeUnitSystem">AW</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="CalculationFactor" attribute="timeUnitsPerHour" type="Integer">12</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="CalculationFactor" attribute="dataCurrency" type="String">EUR</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="SparePartFactor" attribute="smallSparePartCalculationModel" type="SmallPartsCalculationModel">FLAT</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="SparePartFactor" attribute="priceDate" type="Date">2022-09-01</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="SparePartFactor" attribute="priceSource" type="PriceSource">DAT</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="LabourCostFactor" attribute="mechanicWage1" type="Price" mode="PER_TIME_SYSTEM">0.0833</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="LabourCostFactor" attribute="electricWage1" type="Price" mode="PER_TIME_SYSTEM">0.0833</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="LabourCostFactor" attribute="timeUnit" type="TimeUnitSystem">AW</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="LabourCostFactor" attribute="timeUnitsPerHour" type="Integer">12</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="LabourCostFactor" attribute="bodyWage1" type="Price" mode="PER_TIME_SYSTEM">0.0833</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="EuroLacquerFactor" attribute="preparationTimePercent" type="Double">100.0</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="EuroLacquerFactor" attribute="preparationTimePlasticPercent" type="Double">100.0</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="EuroLacquerFactor" attribute="materialMode" type="LacquerMaterialMode">LACQUER_METHOD</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="EuroLacquerFactor" attribute="type" type="String" description="Metallic (2-layer)">12</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="EuroLacquerFactor" attribute="wage" type="Price" mode="PER_TIME_SYSTEM">0.0833</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="EuroLacquerFactor" attribute="materialIndex" type="Double">100.0</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="EuroLacquerFactor" attribute="wageMode" type="LacquerWageMode">PER_TIME</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="EuroLacquerFactor" attribute="wageInclMaterialMode" type="LacquerWageMode">PER_TIME</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="EuroLacquerFactor" attribute="calculationType" type="LacquerCalculationMode">WAGE_MATERIAL_SEPARATELY</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="EuroLacquerFactor" attribute="disposalCostPercent" type="Double">0.0</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="EuroLacquerFactor" attribute="timeUnit" type="TimeUnitSystem">AW</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="EuroLacquerFactor" attribute="timeUnitsPerHour" type="Integer">12</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="ManufacturerLacquerFactor" attribute="preparationTimePercent" type="Double">100.0</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="ManufacturerLacquerFactor" attribute="materialMode" type="LacquerMaterialMode">LACQUER_METHOD</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="ManufacturerLacquerFactor" attribute="typeSaved" type="Boolean">true</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="ManufacturerLacquerFactor" attribute="wageMode" type="LacquerWageMode">PER_TIME</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="ManufacturerLacquerFactor" attribute="wageInclMaterialMode" type="LacquerWageMode">PER_TIME</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="ManufacturerLacquerFactor" attribute="calculationType" type="LacquerCalculationMode">WAGE_MATERIAL_SEPARATELY</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="ManufacturerLacquerFactor" attribute="timeUnit" type="TimeUnitSystem">AW</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="ManufacturerLacquerFactor" attribute="timeUnitsPerHour" type="Integer">12</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="AztLacquerFactor" attribute="preparationTimePercent" type="Double">100.0</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="AztLacquerFactor" attribute="fourLayerLacquerMode" type="AztLacquerMode">WET_IN_WET</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="AztLacquerFactor" attribute="preparationTimePlasticPercent" type="Double">100.0</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="AztLacquerFactor" attribute="materialMode" type="LacquerMaterialMode">LACQUER_METHOD</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="AztLacquerFactor" attribute="materialIndex" type="Double">100.0</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="AztLacquerFactor" attribute="aztDataset" type="Integer">1</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="AztLacquerFactor" attribute="wageMode" type="LacquerWageMode">PER_TIME</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="AztLacquerFactor" attribute="wageInclMaterialMode" type="LacquerWageMode">PER_TIME</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="AztLacquerFactor" attribute="calculationType" type="LacquerCalculationMode">WAGE_MATERIAL_SEPARATELY</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="AztLacquerFactor" attribute="disposalCostPercent" type="Double">0.0</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="AztLacquerFactor" attribute="timeUnit" type="TimeUnitSystem">HOUR</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="AztLacquerFactor" attribute="threeLayerLacquerMode" type="AztLacquerMode">WET_IN_WET</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="AztLacquerFactor" attribute="timeUnitsPerHour" type="Integer">1</vxs:ProcedureRelatedParameter>
                     </vxs:ProcedureRelatedParameters>
                     <vxs:RepairPositions>
                        <!--windshield replacement-->
                        <vxs:RepairPosition>
                           <vxs:DATProcessId>44910</vxs:DATProcessId>
                           <vxs:RepairType>replace</vxs:RepairType>
                           <vxs:Description>windshield</vxs:Description>
                           <vxs:ConstructionGroupId>1</vxs:ConstructionGroupId>
                           <vxs:ConstructionGroup>FRONT END MODULE OUTSIDE</vxs:ConstructionGroup>
                           <vxs:ConstructionGroupPolygon>65</vxs:ConstructionGroupPolygon>
                           <vxs:PositionEntryType>graphical</vxs:PositionEntryType>
                        </vxs:RepairPosition>
                     </vxs:RepairPositions>
                  </vxs:RepairCalculation>
               </vxs:Dossier>
            </dossiers>
            <locale country="DE" datCountryIndicator="DE" language="en"/>
         </request>
      </veh:calculateN>
   </soapenv:Body>
</soapenv:Envelope>
```
