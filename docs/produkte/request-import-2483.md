---
title: "Request importDossier"
topic_id: "2483"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Erstellen, Aktualisiern und Überschreiben eines Vorgangs > Request importDossier"
---

# Request importDossier

<?xml version="1.0" encoding="UTF-8"?>
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:veh="http://sphinx.dat.de/services/VehicleRepairService" xmlns:vxs="http://www.dat.de/vxs">
   <soapenv:Header/>
   <soapenv:Body>
      <veh:importDossier>
         <request>
            <crud>CREATE</crud>
            <dossiers>
               <vxs:Dossier>
                  <vxs:Description>Test_importDossier</vxs:Description>
                  <vxs:DossierType>repair</vxs:DossierType>
                  <vxs:Country>DE</vxs:Country>
                  <vxs:Language>de_DE</vxs:Language>
                  <vxs:Currency>EUR</vxs:Currency>
                  <vxs:Vehicle>
                     <vxs:VehicleIdentNumber>WBAPY71050CU14918</vxs:VehicleIdentNumber>
                     <vxs:DatECode>011300660340006</vxs:DatECode>
                     <vxs:Container>DE002</vxs:Container>
                     <vxs:ConstructionTime>4518</vxs:ConstructionTime>
                     <vxs:ConstructionTimeFrom>4470</vxs:ConstructionTimeFrom>
                     <vxs:ConstructionTimeTo>5049</vxs:ConstructionTimeTo>
                     <vxs:ConstructionTimePriceList>4470</vxs:ConstructionTimePriceList>
                     <vxs:VehicleTypeName>Pkw, SUV, Kleintransporter</vxs:VehicleTypeName>
                     <vxs:VehicleTypeNameN origin="dat">Pkw, SUV, Kleintransporter</vxs:VehicleTypeNameN>
                     <vxs:ManufacturerName origin="dat">BMW</vxs:ManufacturerName>
                     <vxs:BaseModelName origin="dat">Baureihe 5 Touring (E61)(2004->)</vxs:BaseModelName>
                     <vxs:SubModelName origin="dat">530d xDrive</vxs:SubModelName>
                     <vxs:MainTypeGroupName>5</vxs:MainTypeGroupName>
                     <vxs:VehicleType>1</vxs:VehicleType>
                     <vxs:Manufacturer>130</vxs:Manufacturer>
                     <vxs:BaseModel>66</vxs:BaseModel>
                     <vxs:SubModel>34</vxs:SubModel>
                     <vxs:MainTypeGroup>5</vxs:MainTypeGroup>
                     <vxs:IdentificationSource>IDENTIFICATIONSOURCE_VIN</vxs:IdentificationSource>
                     <vxs:VinAccuracy>0</vxs:VinAccuracy>
                     <vxs:VinActive>true</vxs:VinActive>
                     <vxs:ReleaseIndicator>ALL</vxs:ReleaseIndicator>
                     <vxs:KbaNumbersN>
                        <vxs:KbaNumber>0005/AIT</vxs:KbaNumber>
                     </vxs:KbaNumbersN>
                     <vxs:PaintTypes>
                        <vxs:PaintType>31</vxs:PaintType>
                     </vxs:PaintTypes>
                     <vxs:Equipment>
                        <vxs:SeriesEquipment>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>26803</vxs:DatEquipmentId>
                              <vxs:Description>Airbag Fahrer-/Beifahrerseite</vxs:Description>
                              <vxs:EquipmentGroup>AIR1</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>40000</vxs:DatEquipmentId>
                              <vxs:Description>Anti-Blockier-System (ABS)</vxs:Description>
                              <vxs:EquipmentGroup>ABS</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>70410</vxs:DatEquipmentId>
                              <vxs:ManufacturerEquipmentId>203</vxs:ManufacturerEquipmentId>
                              <vxs:ManufacturerDescription>ALLRADSYSTEM</vxs:ManufacturerDescription>
                              <vxs:Description>Antriebsart: xDrive (Allrad)</vxs:Description>
                              <vxs:EquipmentGroup>4WD</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>18604</vxs:DatEquipmentId>
                              <vxs:Description>Automatische Fahrlichtschaltung</vxs:Description>
                              <vxs:EquipmentGroup>AUFL</vxs:EquipmentGroup>
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
                              <vxs:DatEquipmentId>72901</vxs:DatEquipmentId>
                              <vxs:Description>Batterie 90 Ah</vxs:Description>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>18504</vxs:DatEquipmentId>
                              <vxs:Description>Blinkleuchten Weiß</vxs:Description>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>25508</vxs:DatEquipmentId>
                              <vxs:Description>Bordcomputer</vxs:Description>
                              <vxs:EquipmentGroup>COMP</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>25506</vxs:DatEquipmentId>
                              <vxs:Description>Bordmonitor mit Farbbildschirm</vxs:Description>
                              <vxs:EquipmentGroup>COMP</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>25606</vxs:DatEquipmentId>
                              <vxs:Description>Check-Control-System</vxs:Description>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>25300</vxs:DatEquipmentId>
                              <vxs:Description>Drehzahlmesser</vxs:Description>
                              <vxs:ContainedEquipmentPositions>
                                 <vxs:EquipmentPosition>
                                    <vxs:DatEquipmentId>25607</vxs:DatEquipmentId>
                                    <vxs:Description>Energie-Control (EC)</vxs:Description>
                                 </vxs:EquipmentPosition>
                              </vxs:ContainedEquipmentPositions>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>70100</vxs:DatEquipmentId>
                              <vxs:Description>Dynamische Stabilitäts-Control (DSC)</vxs:Description>
                              <vxs:EquipmentGroup>ESP</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>25607</vxs:DatEquipmentId>
                              <vxs:Description>Energie-Control (EC)</vxs:Description>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>35000</vxs:DatEquipmentId>
                              <vxs:Description>Fensterheber elektrisch</vxs:Description>
                              <vxs:EquipmentGroup>FH2</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>35405</vxs:DatEquipmentId>
                              <vxs:Description>Fernbedienung für Zentralverriegelung</vxs:Description>
                              <vxs:EquipmentGroup>ZV</vxs:EquipmentGroup>
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
                              <vxs:DatEquipmentId>26708</vxs:DatEquipmentId>
                              <vxs:Description>Geschwindigkeits-Regelanlage (Tempomat)</vxs:Description>
                              <vxs:EquipmentGroup>TEMP</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>18802</vxs:DatEquipmentId>
                              <vxs:Description>Heckleuchten LED</vxs:Description>
                              <vxs:EquipmentGroup>LEDH</vxs:EquipmentGroup>
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
                              <vxs:DatEquipmentId>34805</vxs:DatEquipmentId>
                              <vxs:Description>Kopfstützen hinten</vxs:Description>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>34904</vxs:DatEquipmentId>
                              <vxs:Description>Kopfstützen hinten mechan. verstellbar (3 Stück)</vxs:Description>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>69505</vxs:DatEquipmentId>
                              <vxs:Description>Lenksäule (Lenkrad) mechan. verstellbar</vxs:Description>
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
                              <vxs:DatEquipmentId>92930</vxs:DatEquipmentId>
                              <vxs:Description>Motor 3,0 Ltr. - 173 kW Turbodiesel KAT</vxs:Description>
                              <vxs:EquipmentClass>1</vxs:EquipmentClass>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>18300</vxs:DatEquipmentId>
                              <vxs:Description>Nebelscheinwerfer</vxs:Description>
                              <vxs:EquipmentGroup>BEL</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>42805</vxs:DatEquipmentId>
                              <vxs:Description>Niveauregulierung</vxs:Description>
                              <vxs:EquipmentGroup>NIV</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>25903</vxs:DatEquipmentId>
                              <vxs:Description>Reifendruck-Kontrollsystem</vxs:Description>
                              <vxs:EquipmentGroup>RDK</vxs:EquipmentGroup>
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
                              <vxs:DatEquipmentId>33600</vxs:DatEquipmentId>
                              <vxs:Description>Rücksitzbank klappbar</vxs:Description>
                              <vxs:EquipmentGroup>SITH</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>77224</vxs:DatEquipmentId>
                              <vxs:Description>Schadstoffarm nach Abgasnorm Euro 4</vxs:Description>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>39205</vxs:DatEquipmentId>
                              <vxs:Description>Schalt-/Wählhebelgriff Leder</vxs:Description>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>23603</vxs:DatEquipmentId>
                              <vxs:Description>Scheibenkleber für Warmverklebung</vxs:Description>
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
                              <vxs:DatEquipmentId>26903</vxs:DatEquipmentId>
                              <vxs:Description>Seitenairbag vorn</vxs:Description>
                              <vxs:EquipmentGroup>AIR3</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>69811</vxs:DatEquipmentId>
                              <vxs:Description>Servolenkung Servotronic</vxs:Description>
                              <vxs:EquipmentGroup>SL</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>32607</vxs:DatEquipmentId>
                              <vxs:Description>Sitze vorn elektr. verstellbar</vxs:Description>
                              <vxs:EquipmentGroup>SITE</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>21300</vxs:DatEquipmentId>
                              <vxs:Description>Stoßfänger Wagenfarbe</vxs:Description>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>22005</vxs:DatEquipmentId>
                              <vxs:Description>Verglasung grün getönt</vxs:Description>
                              <vxs:EquipmentGroup>WDG</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>22302</vxs:DatEquipmentId>
                              <vxs:Description>Wärmeschutzverglasung getönt</vxs:Description>
                              <vxs:EquipmentGroup>WDG</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>35307</vxs:DatEquipmentId>
                              <vxs:Description>Zentralverriegelung mit Diebstahlsicherung und Crashsensor</vxs:Description>
                              <vxs:EquipmentGroup>ZV</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                        </vxs:SeriesEquipment>
                        <vxs:SpecialEquipment>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>4905</vxs:DatEquipmentId>
                              <vxs:ManufacturerEquipmentId>7RP</vxs:ManufacturerEquipmentId>
                              <vxs:ManufacturerDescription>ADVANTAGE PAKET</vxs:ManufacturerDescription>
                              <vxs:Description>Advantage-Paket</vxs:Description>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>2701</vxs:DatEquipmentId>
                              <vxs:ManufacturerEquipmentId>715</vxs:ManufacturerEquipmentId>
                              <vxs:ManufacturerDescription>M AERODYNAMIKPAKET</vxs:ManufacturerDescription>
                              <vxs:Description>Aerodynamik-Paket M-Technic</vxs:Description>
                              <vxs:EquipmentGroup>SPOI</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>25805</vxs:DatEquipmentId>
                              <vxs:ManufacturerEquipmentId>633</vxs:ManufacturerEquipmentId>
                              <vxs:ManufacturerDescription>HANDY VORB. BUSINESS/BLUETOOTH-SCH.</vxs:ManufacturerDescription>
                              <vxs:Description>Audio-Navigationssystem Professional mit integrierter Handyvorrüstung</vxs:Description>
                              <vxs:EquipmentGroup>GPS</vxs:EquipmentGroup>
                              <vxs:ContainedEquipmentPositions>
                                 <vxs:EquipmentPosition>
                                    <vxs:DatEquipmentId>24106</vxs:DatEquipmentId>
                                    <vxs:Description>Audiosystem BMW Professional (Radio/CD-Player)</vxs:Description>
                                    <vxs:EquipmentGroup>CD</vxs:EquipmentGroup>
                                 </vxs:EquipmentPosition>
                                 <vxs:EquipmentPosition>
                                    <vxs:DatEquipmentId>24707</vxs:DatEquipmentId>
                                    <vxs:Description>Vorrüstung Mobiltelefon/Handy</vxs:Description>
                                    <vxs:EquipmentGroup>TEL1</vxs:EquipmentGroup>
                                 </vxs:EquipmentPosition>
                                 <vxs:EquipmentPosition>
                                    <vxs:DatEquipmentId>24811</vxs:DatEquipmentId>
                                    <vxs:Description>Vorrüstung Mobiltelefon/Handy Business mit Bluetooth Schnittstelle</vxs:Description>
                                    <vxs:EquipmentGroup>TEL1</vxs:EquipmentGroup>
                                 </vxs:EquipmentPosition>
                              </vxs:ContainedEquipmentPositions>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>8702</vxs:DatEquipmentId>
                              <vxs:ManufacturerEquipmentId>760</vxs:ManufacturerEquipmentId>
                              <vxs:ManufacturerDescription>M HOCHGLANZ SHADOW LINE</vxs:ManufacturerDescription>
                              <vxs:Description>Außenausstattung: Shadow-Line Hochglanz</vxs:Description>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>27804</vxs:DatEquipmentId>
                              <vxs:ManufacturerEquipmentId>775</vxs:ManufacturerEquipmentId>
                              <vxs:ManufacturerDescription>M DACHHIMMEL ANTHRAZIT</vxs:ManufacturerDescription>
                              <vxs:Description>Dachhimmel Anthrazit</vxs:Description>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>16000</vxs:DatEquipmentId>
                              <vxs:ManufacturerEquipmentId>386</vxs:ManufacturerEquipmentId>
                              <vxs:ManufacturerDescription>DACHRELING</vxs:ManufacturerDescription>
                              <vxs:Description>Dachreling</vxs:Description>
                              <vxs:EquipmentGroup>DARE</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>75904</vxs:DatEquipmentId>
                              <vxs:ManufacturerEquipmentId>205</vxs:ManufacturerEquipmentId>
                              <vxs:ManufacturerDescription>AUTOMATIC GETRIEBE</vxs:ManufacturerDescription>
                              <vxs:Description>Getriebe Automatik - mit Steptronic (6-Stufen)</vxs:Description>
                              <vxs:EquipmentGroup>AG2</vxs:EquipmentGroup>
                              <vxs:EquipmentClass>11</vxs:EquipmentClass>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>38908</vxs:DatEquipmentId>
                              <vxs:ManufacturerEquipmentId>442</vxs:ManufacturerEquipmentId>
                              <vxs:ManufacturerDescription>GETRAENKEHALTER</vxs:ManufacturerDescription>
                              <vxs:Description>Getränkehalter</vxs:Description>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>24607</vxs:DatEquipmentId>
                              <vxs:ManufacturerEquipmentId>676</vxs:ManufacturerEquipmentId>
                              <vxs:ManufacturerDescription>HIFI LAUTSPRECHERSYSTEM</vxs:ManufacturerDescription>
                              <vxs:Description>HiFi-Lautsprechersystem</vxs:Description>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>31704</vxs:DatEquipmentId>
                              <vxs:ManufacturerEquipmentId>438</vxs:ManufacturerEquipmentId>
                              <vxs:ManufacturerDescription>EDELHOLZAUSFUEHRUNG</vxs:ManufacturerDescription>
                              <vxs:Description>Innenausstattung: Edelholz</vxs:Description>
                              <vxs:ContainedEquipmentPositions>
                                 <vxs:EquipmentPosition>
                                    <vxs:DatEquipmentId>26217</vxs:DatEquipmentId>
                                    <vxs:Description>Innenausstattung: Interieurleisten Edelholz</vxs:Description>
                                 </vxs:EquipmentPosition>
                              </vxs:ContainedEquipmentPositions>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>26217</vxs:DatEquipmentId>
                              <vxs:Description>Innenausstattung: Interieurleisten Edelholz</vxs:Description>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>28807</vxs:DatEquipmentId>
                              <vxs:ManufacturerEquipmentId>534</vxs:ManufacturerEquipmentId>
                              <vxs:ManufacturerDescription>KLIMAAUTOMATIK</vxs:ManufacturerDescription>
                              <vxs:Description>Klimaautomatik erweiterter Umfang</vxs:Description>
                              <vxs:EquipmentGroup>KLI2</vxs:EquipmentGroup>
                              <vxs:ContainedEquipmentPositions>
                                 <vxs:EquipmentPosition>
                                    <vxs:DatEquipmentId>27206</vxs:DatEquipmentId>
                                    <vxs:Description>Mittelarmlehne vorn verstellbar</vxs:Description>
                                    <vxs:EquipmentGroup>MALV</vxs:EquipmentGroup>
                                 </vxs:EquipmentPosition>
                              </vxs:ContainedEquipmentPositions>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>69204</vxs:DatEquipmentId>
                              <vxs:ManufacturerEquipmentId>710</vxs:ManufacturerEquipmentId>
                              <vxs:ManufacturerDescription>M LEDERLENKRAD</vxs:ManufacturerDescription>
                              <vxs:Description>Lenkrad (Sport M-Technic)</vxs:Description>
                              <vxs:EquipmentGroup>LEN6</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>49405</vxs:DatEquipmentId>
                              <vxs:ManufacturerEquipmentId>2NP</vxs:ManufacturerEquipmentId>
                              <vxs:ManufacturerDescription>M LM R. DOPPELSPEICHE 135 M NOTLAUF</vxs:ManufacturerDescription>
                              <vxs:Description>LM-Felgen 8x18 (M Doppelspeichen 135)</vxs:Description>
                              <vxs:EquipmentGroup>ALU</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>11000</vxs:DatEquipmentId>
                              <vxs:ManufacturerEquipmentId>M</vxs:ManufacturerEquipmentId>
                              <vxs:Description>Metallic-Lackierung</vxs:Description>
                              <vxs:EquipmentGroup>SONL</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>27206</vxs:DatEquipmentId>
                              <vxs:Description>Mittelarmlehne vorn verstellbar</vxs:Description>
                              <vxs:EquipmentGroup>MALV</vxs:EquipmentGroup>
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
                              <vxs:DatEquipmentId>19000</vxs:DatEquipmentId>
                              <vxs:ManufacturerEquipmentId>502</vxs:ManufacturerEquipmentId>
                              <vxs:ManufacturerDescription>SCHEINWERFER-WASCHANLAGE</vxs:ManufacturerDescription>
                              <vxs:Description>Scheinwerfer-Reinigungsanlage (SRA)</vxs:Description>
                              <vxs:EquipmentGroup>SWRA</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>30109</vxs:DatEquipmentId>
                              <vxs:Description>Sitzbezug / Polsterung: Stoff / Leder</vxs:Description>
                              <vxs:EquipmentGroup>LED1</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>29500</vxs:DatEquipmentId>
                              <vxs:ManufacturerEquipmentId>494</vxs:ManufacturerEquipmentId>
                              <vxs:ManufacturerDescription>SITZHEIZUNG FUER FAHRER/BEIFAHRER</vxs:ManufacturerDescription>
                              <vxs:Description>Sitzheizung vorn</vxs:Description>
                              <vxs:EquipmentGroup>SITB</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>39103</vxs:DatEquipmentId>
                              <vxs:ManufacturerEquipmentId>464</vxs:ManufacturerEquipmentId>
                              <vxs:ManufacturerDescription>SKISACK</vxs:ManufacturerDescription>
                              <vxs:Description>Skisack</vxs:Description>
                              <vxs:EquipmentGroup>DULA</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>3209</vxs:DatEquipmentId>
                              <vxs:ManufacturerEquipmentId>337</vxs:ManufacturerEquipmentId>
                              <vxs:ManufacturerDescription>M SPORTPAKET</vxs:ManufacturerDescription>
                              <vxs:Description>Sport-Paket M / M-Technic</vxs:Description>
                              <vxs:ContainedEquipmentPositions>
                                 <vxs:EquipmentPosition>
                                    <vxs:DatEquipmentId>8701</vxs:DatEquipmentId>
                                    <vxs:Description>Außenausstattung: Shadow-Line</vxs:Description>
                                 </vxs:EquipmentPosition>
                                 <vxs:EquipmentPosition>
                                    <vxs:DatEquipmentId>27804</vxs:DatEquipmentId>
                                    <vxs:Description>Dachhimmel Anthrazit</vxs:Description>
                                 </vxs:EquipmentPosition>
                                 <vxs:EquipmentPosition>
                                    <vxs:DatEquipmentId>30109</vxs:DatEquipmentId>
                                    <vxs:Description>Sitzbezug / Polsterung: Stoff / Leder</vxs:Description>
                                    <vxs:EquipmentGroup>LED1</vxs:EquipmentGroup>
                                 </vxs:EquipmentPosition>
                                 <vxs:EquipmentPosition>
                                    <vxs:DatEquipmentId>31901</vxs:DatEquipmentId>
                                    <vxs:Description>Sportsitze vorn</vxs:Description>
                                    <vxs:EquipmentGroup>SPSI</vxs:EquipmentGroup>
                                 </vxs:EquipmentPosition>
                                 <vxs:EquipmentPosition>
                                    <vxs:DatEquipmentId>42100</vxs:DatEquipmentId>
                                    <vxs:Description>Sportliche Fahrwerksabstimmung</vxs:Description>
                                    <vxs:EquipmentGroup>SPFW</vxs:EquipmentGroup>
                                 </vxs:EquipmentPosition>
                                 <vxs:EquipmentPosition>
                                    <vxs:DatEquipmentId>69204</vxs:DatEquipmentId>
                                    <vxs:Description>Lenkrad (Sport M-Technic)</vxs:Description>
                                    <vxs:EquipmentGroup>LEN6</vxs:EquipmentGroup>
                                 </vxs:EquipmentPosition>
                              </vxs:ContainedEquipmentPositions>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>42100</vxs:DatEquipmentId>
                              <vxs:Description>Sportliche Fahrwerksabstimmung</vxs:Description>
                              <vxs:EquipmentGroup>SPFW</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>31901</vxs:DatEquipmentId>
                              <vxs:ManufacturerEquipmentId>481</vxs:ManufacturerEquipmentId>
                              <vxs:ManufacturerDescription>SPORTSITZE FUER FAHRER/BEIFAHRER</vxs:ManufacturerDescription>
                              <vxs:Description>Sportsitze vorn</vxs:Description>
                              <vxs:EquipmentGroup>SPSI</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>25010</vxs:DatEquipmentId>
                              <vxs:ManufacturerEquipmentId>6FL</vxs:ManufacturerEquipmentId>
                              <vxs:ManufacturerDescription>USB-AUDIO-SCHNITTSTELLE</vxs:ManufacturerDescription>
                              <vxs:Description>USB-Schnittstelle</vxs:Description>
                              <vxs:EquipmentGroup>MP3A</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>24707</vxs:DatEquipmentId>
                              <vxs:Description>Vorrüstung Mobiltelefon/Handy</vxs:Description>
                              <vxs:EquipmentGroup>TEL1</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>24811</vxs:DatEquipmentId>
                              <vxs:Description>Vorrüstung Mobiltelefon/Handy Business mit Bluetooth Schnittstelle</vxs:Description>
                              <vxs:EquipmentGroup>TEL1</vxs:EquipmentGroup>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>18008</vxs:DatEquipmentId>
                              <vxs:ManufacturerEquipmentId>522</vxs:ManufacturerEquipmentId>
                              <vxs:ManufacturerDescription>XENON-LICHT</vxs:ManufacturerDescription>
                              <vxs:Description>Xenon-Scheinwerfer</vxs:Description>
                              <vxs:EquipmentGroup>XELI</vxs:EquipmentGroup>
                              <vxs:ContainedEquipmentPositions>
                                 <vxs:EquipmentPosition>
                                    <vxs:DatEquipmentId>18904</vxs:DatEquipmentId>
                                    <vxs:Description>Tagfahrlicht</vxs:Description>
                                    <vxs:EquipmentGroup>TFAL</vxs:EquipmentGroup>
                                 </vxs:EquipmentPosition>
                                 <vxs:EquipmentPosition>
                                    <vxs:DatEquipmentId>19000</vxs:DatEquipmentId>
                                    <vxs:Description>Scheinwerfer-Reinigungsanlage (SRA)</vxs:Description>
                                    <vxs:EquipmentGroup>SWRA</vxs:EquipmentGroup>
                                 </vxs:EquipmentPosition>
                              </vxs:ContainedEquipmentPositions>
                           </vxs:EquipmentPosition>
                        </vxs:SpecialEquipment>
                     </vxs:Equipment>
                     <vxs:DATECodeEquipment>
                        <vxs:EquipmentPosition>
                           <vxs:DatEquipmentId>92930</vxs:DatEquipmentId>
                           <vxs:Description>Motor 3,0 Ltr. - 173 kW Turbodiesel KAT</vxs:Description>
                           <vxs:EquipmentClass>1</vxs:EquipmentClass>
                        </vxs:EquipmentPosition>
                        <vxs:EquipmentPosition>
                           <vxs:DatEquipmentId>10005</vxs:DatEquipmentId>
                           <vxs:Description>Karosserie: 5-türig</vxs:Description>
                           <vxs:EquipmentClass>2</vxs:EquipmentClass>
                        </vxs:EquipmentPosition>
                        <vxs:EquipmentPosition>
                           <vxs:DatEquipmentId>75904</vxs:DatEquipmentId>
                           <vxs:Description>Getriebe Automatik - mit Steptronic (6-Stufen)</vxs:Description>
                           <vxs:EquipmentClass>11</vxs:EquipmentClass>
                        </vxs:EquipmentPosition>
                     </vxs:DATECodeEquipment>
                     <vxs:VINResult>
                        <vxs:VinInterfaceVersion>2.5</vxs:VinInterfaceVersion>
                        <vxs:VINECodes>
                           <vxs:VINECode>
                              <vxs:Sign>0</vxs:Sign>
                              <vxs:VehicleTypeKey>1</vxs:VehicleTypeKey>
                              <vxs:ManufacturerKey>130</vxs:ManufacturerKey>
                              <vxs:VehicleMainTypeKey>66</vxs:VehicleMainTypeKey>
                              <vxs:VehicleSubTypeKey>34</vxs:VehicleSubTypeKey>
                              <vxs:VehicleSubTypeVariantKey>6</vxs:VehicleSubTypeVariantKey>
                              <vxs:ConstructionTimeMin>4510</vxs:ConstructionTimeMin>
                              <vxs:ConstructionTime>4518</vxs:ConstructionTime>
                              <vxs:ConstructionTimeEdge>4290</vxs:ConstructionTimeEdge>
                              <vxs:ConstructionTimeProd>4518</vxs:ConstructionTimeProd>
                              <vxs:ConstructionTimePriceList>4470</vxs:ConstructionTimePriceList>
                              <vxs:VINContainers>
                                 <vxs:VINContainer>
                                    <vxs:Container>002</vxs:Container>
                                    <vxs:VehicleTypeKey>5</vxs:VehicleTypeKey>
                                    <vxs:ManufacturerKey>130</vxs:ManufacturerKey>
                                    <vxs:VehicleMainTypeKey>3216</vxs:VehicleMainTypeKey>
                                    <vxs:VehicleSubTypeKey>16</vxs:VehicleSubTypeKey>
                                    <vxs:VehicleConstructionTime>4518</vxs:VehicleConstructionTime>
                                 </vxs:VINContainer>
                              </vxs:VINContainers>
                           </vxs:VINECode>
                        </vxs:VINECodes>
                        <vxs:VINEquipments>
                           <vxs:VINEquipment>
                              <vxs:ShortName>Model: 530XD (E61)</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:ManufacturerCode>548</vxs:ManufacturerCode>
                              <vxs:ShortName>KILOMETERTACHO</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:ManufacturerCode>612</vxs:ManufacturerCode>
                              <vxs:ShortName>BMW ASSIST</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:ManufacturerCode>698</vxs:ManufacturerCode>
                              <vxs:ShortName>AREA-CODE 2</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:ManufacturerCode>6AA</vxs:ManufacturerCode>
                              <vxs:ShortName>BMW TELESERVICES</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:ManufacturerCode>851</vxs:ManufacturerCode>
                              <vxs:ShortName>SPRACHVERSION DEUTSCH</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:ManufacturerCode>863</vxs:ManufacturerCode>
                              <vxs:ShortName>SERVICE KONTAKT-FLYER EUROPA</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:ManufacturerCode>8S8</vxs:ManufacturerCode>
                              <vxs:ShortName>LAENDERSPEZ. NAVI ZUST. (FUER ACC)</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:ManufacturerCode>8SA</vxs:ManufacturerCode>
                              <vxs:ShortName>LAENDERSPEZ. NAVI.-FREISCHALTUNG</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:ManufacturerCode>8SP</vxs:ManufacturerCode>
                              <vxs:ShortName>COP STEUERUNG</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:ManufacturerCode>COUNTRY:DE</vxs:ManufacturerCode>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:ManufacturerCode>M57/T2/3.00/173</vxs:ManufacturerCode>
                              <vxs:ShortName>3.00L / 173kW</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:ManufacturerCode>TypeA:PY81</vxs:ManufacturerCode>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:ManufacturerCode>TypeB:PY71</vxs:ManufacturerCode>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:ManufacturerCode>VIN10:0</vxs:ManufacturerCode>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:ManufacturerCode>VIN11:C</vxs:ManufacturerCode>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:ManufacturerCode>WHC:WBA</vxs:ManufacturerCode>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>789</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>320</vxs:ManufacturerCode>
                              <vxs:ShortName>MODELLSCHRIFTZUG ENTFALL</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>1420</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>7RP</vxs:ManufacturerCode>
                              <vxs:ShortName>ADVANTAGE PAKET</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>2701</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>715</vxs:ManufacturerCode>
                              <vxs:ShortName>M AERODYNAMIKPAKET</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>3209</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>337</vxs:ManufacturerCode>
                              <vxs:ShortName>M SPORTPAKET</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>3306</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>715</vxs:ManufacturerCode>
                              <vxs:ShortName>M AERODYNAMIKPAKET</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>4905</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>7RP</vxs:ManufacturerCode>
                              <vxs:ShortName>ADVANTAGE PAKET</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>8701</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>760</vxs:ManufacturerCode>
                              <vxs:ShortName>M HOCHGLANZ SHADOW LINE</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>8702</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>760</vxs:ManufacturerCode>
                              <vxs:ShortName>M HOCHGLANZ SHADOW LINE</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>11000</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>416M</vxs:ManufacturerCode>
                              <vxs:ShortName>CARBONSCHWARZ METALLIC</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>11000</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>M</vxs:ManufacturerCode>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>16000</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>386</vxs:ManufacturerCode>
                              <vxs:ShortName>DACHRELING</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>16195</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>386</vxs:ManufacturerCode>
                              <vxs:ShortName>DACHRELING</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>16302</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>402</vxs:ManufacturerCode>
                              <vxs:ShortName>PANORAMA GLASDACH</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>18008</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>522</vxs:ManufacturerCode>
                              <vxs:ShortName>XENON-LICHT</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>18505</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>522</vxs:ManufacturerCode>
                              <vxs:ShortName>XENON-LICHT</vxs:ShortName>
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
                              <vxs:AvNumberDat>24607</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>676</vxs:ManufacturerCode>
                              <vxs:ShortName>HIFI LAUTSPRECHERSYSTEM</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>24705</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>616</vxs:ManufacturerCode>
                              <vxs:ShortName>BMW ONLINE</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>24709</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>620</vxs:ManufacturerCode>
                              <vxs:ShortName>SPRACHEINGABESYSTEM</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>25010</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>6FL</vxs:ManufacturerCode>
                              <vxs:ShortName>USB-AUDIO-SCHNITTSTELLE</vxs:ShortName>
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
                              <vxs:AvNumberDat>25805</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>633</vxs:ManufacturerCode>
                              <vxs:ShortName>HANDY VORB. BUSINESS/BLUETOOTH-SCH.</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>26710</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>544</vxs:ManufacturerCode>
                              <vxs:ShortName>GESCHWINDIGKEITSREGEL. MIT BREMSF.</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>27804</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>775</vxs:ManufacturerCode>
                              <vxs:ShortName>M DACHHIMMEL ANTHRAZIT</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>27810</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>775</vxs:ManufacturerCode>
                              <vxs:ShortName>M DACHHIMMEL ANTHRAZIT</vxs:ShortName>
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
                              <vxs:ManufacturerCode>LCBA</vxs:ManufacturerCode>
                              <vxs:ShortName>LEDER DAKOTA/BEIGE 3</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>31304</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>438</vxs:ManufacturerCode>
                              <vxs:ShortName>EDELHOLZAUSFUEHRUNG</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>31312</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>438</vxs:ManufacturerCode>
                              <vxs:ShortName>EDELHOLZAUSFUEHRUNG</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>31700</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>438</vxs:ManufacturerCode>
                              <vxs:ShortName>EDELHOLZAUSFUEHRUNG</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>31704</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>438</vxs:ManufacturerCode>
                              <vxs:ShortName>EDELHOLZAUSFUEHRUNG</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>31810</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>481</vxs:ManufacturerCode>
                              <vxs:ShortName>SPORTSITZE FUER FAHRER/BEIFAHRER</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>31901</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>481</vxs:ManufacturerCode>
                              <vxs:ShortName>SPORTSITZE FUER FAHRER/BEIFAHRER</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>32002</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>481</vxs:ManufacturerCode>
                              <vxs:ShortName>SPORTSITZE FUER FAHRER/BEIFAHRER</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>32006</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>481</vxs:ManufacturerCode>
                              <vxs:ShortName>SPORTSITZE FUER FAHRER/BEIFAHRER</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>38908</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>442</vxs:ManufacturerCode>
                              <vxs:ShortName>GETRAENKEHALTER</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>38909</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>442</vxs:ManufacturerCode>
                              <vxs:ShortName>GETRAENKEHALTER</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>38999</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>428</vxs:ManufacturerCode>
                              <vxs:ShortName>WARNDREIECK</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>39103</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>464</vxs:ManufacturerCode>
                              <vxs:ShortName>SKISACK</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>49405</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>2NP</vxs:ManufacturerCode>
                              <vxs:ShortName>M LM R. DOPPELSPEICHE 135 M NOTLAUF</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>69103</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>710</vxs:ManufacturerCode>
                              <vxs:ShortName>M LEDERLENKRAD</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>69204</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>710</vxs:ManufacturerCode>
                              <vxs:ShortName>M LEDERLENKRAD</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>69309</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>710</vxs:ManufacturerCode>
                              <vxs:ShortName>M LEDERLENKRAD</vxs:ShortName>
                           </vxs:VINEquipment>
                           <vxs:VINEquipment>
                              <vxs:AvNumberDat>70410</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>203</vxs:ManufacturerCode>
                              <vxs:ShortName>ALLRADSYSTEM</vxs:ShortName>
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
                              <vxs:AvNumberDat>97741</vxs:AvNumberDat>
                              <vxs:ManufacturerCode>337</vxs:ManufacturerCode>
                              <vxs:ShortName>M SPORTPAKET</vxs:ShortName>
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
                              <vxs:Code>416</vxs:Code>
                              <vxs:Description>CARBONSCHWARZ METALLIC</vxs:Description>
                              <vxs:StandardColor>9</vxs:StandardColor>
                              <vxs:PaintType>31</vxs:PaintType>
                              <vxs:CountCoat>2 COAT</vxs:CountCoat>
                           </vxs:VINColor>
                           <vxs:VINColor>
                              <vxs:ColorID>I1</vxs:ColorID>
                              <vxs:Code>LCBA</vxs:Code>
                              <vxs:Description>LEDER DAKOTA/BEIGE 3</vxs:Description>
                           </vxs:VINColor>
                           <vxs:VINColor>
                              <vxs:ColorID>PM</vxs:ColorID>
                              <vxs:Code/>
                              <vxs:Description>LEDER DAKOTA</vxs:Description>
                           </vxs:VINColor>
                           <vxs:VINColor>
                              <vxs:ColorID>PF</vxs:ColorID>
                              <vxs:Code/>
                              <vxs:Description>BEIGE 3</vxs:Description>
                           </vxs:VINColor>
                        </vxs:VINColors>
                        <vxs:VINVehicle>
                           <vxs:VINumber>
                              <vxs:VinCode>WBAPY71050CU14918</vxs:VinCode>
                           </vxs:VINumber>
                           <vxs:ManufacturerCarCode>PY81</vxs:ManufacturerCarCode>
                        </vxs:VINVehicle>
                     </vxs:VINResult>
                     <vxs:TokenOfVinResult>eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJkYXQiLCJ0aW1lc3RhbXAiOjE2NTIxODQ3MzQxOTksImN1c3RvbWVyIjoiMTM0MDc4OSIsImludGVyZmFjZVBhcnRuZXIiOiIxMzQwNzg5IiwidmluUmVzdWx0SGFzaCI6Imhhc2gwMV8xNTA0ODM2NDQ0In0.nDx1BTidf1NQdiga40nOJksH31kk-vYegQywOtUJ3EU</vxs:TokenOfVinResult>
                  </vxs:Vehicle>
                  <vxs:RepairCalculation>
                     <vxs:Vehicle>
                        <vxs:VehicleIdentNumber>WBAPY71050CU14918</vxs:VehicleIdentNumber>
                        <vxs:DatECode>011300660340006</vxs:DatECode>
                        <vxs:Container>DE002</vxs:Container>
                        <vxs:ConstructionTime>4518</vxs:ConstructionTime>
                        <vxs:ConstructionTimeFrom>4470</vxs:ConstructionTimeFrom>
                        <vxs:ConstructionTimeTo>5049</vxs:ConstructionTimeTo>
                        <vxs:ConstructionTimePriceList>4470</vxs:ConstructionTimePriceList>
                        <vxs:VehicleTypeName>Pkw, SUV, Kleintransporter</vxs:VehicleTypeName>
                        <vxs:VehicleTypeNameN origin="dat">Pkw, SUV, Kleintransporter</vxs:VehicleTypeNameN>
                        <vxs:ManufacturerName origin="dat">BMW</vxs:ManufacturerName>
                        <vxs:BaseModelName origin="dat">Baureihe 5 Touring (E61)(2004->)</vxs:BaseModelName>
                        <vxs:SubModelName origin="dat">530d xDrive</vxs:SubModelName>
                        <vxs:MainTypeGroupName>5</vxs:MainTypeGroupName>
                        <vxs:VehicleType>1</vxs:VehicleType>
                        <vxs:Manufacturer>130</vxs:Manufacturer>
                        <vxs:BaseModel>66</vxs:BaseModel>
                        <vxs:SubModel>34</vxs:SubModel>
                        <vxs:MainTypeGroup>5</vxs:MainTypeGroup>
                        <vxs:IdentificationSource>IDENTIFICATIONSOURCE_VIN</vxs:IdentificationSource>
                        <vxs:VinAccuracy>0</vxs:VinAccuracy>
                        <vxs:VinActive>true</vxs:VinActive>
                        <vxs:ReleaseIndicator>ALL</vxs:ReleaseIndicator>
                        <vxs:KbaNumbersN>
                           <vxs:KbaNumber>0005/AIT</vxs:KbaNumber>
                        </vxs:KbaNumbersN>
                        <vxs:PaintTypes>
                           <vxs:PaintType>31</vxs:PaintType>
                        </vxs:PaintTypes>
                        <vxs:Equipment>
                           <vxs:SeriesEquipment>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>26803</vxs:DatEquipmentId>
                                 <vxs:Description>Airbag Fahrer-/Beifahrerseite</vxs:Description>
                                 <vxs:EquipmentGroup>AIR1</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>40000</vxs:DatEquipmentId>
                                 <vxs:Description>Anti-Blockier-System (ABS)</vxs:Description>
                                 <vxs:EquipmentGroup>ABS</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>70410</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>203</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>ALLRADSYSTEM</vxs:ManufacturerDescription>
                                 <vxs:Description>Antriebsart: xDrive (Allrad)</vxs:Description>
                                 <vxs:EquipmentGroup>4WD</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>18604</vxs:DatEquipmentId>
                                 <vxs:Description>Automatische Fahrlichtschaltung</vxs:Description>
                                 <vxs:EquipmentGroup>AUFL</vxs:EquipmentGroup>
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
                                 <vxs:DatEquipmentId>72901</vxs:DatEquipmentId>
                                 <vxs:Description>Batterie 90 Ah</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>18504</vxs:DatEquipmentId>
                                 <vxs:Description>Blinkleuchten Weiß</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>25508</vxs:DatEquipmentId>
                                 <vxs:Description>Bordcomputer</vxs:Description>
                                 <vxs:EquipmentGroup>COMP</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>25506</vxs:DatEquipmentId>
                                 <vxs:Description>Bordmonitor mit Farbbildschirm</vxs:Description>
                                 <vxs:EquipmentGroup>COMP</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>25606</vxs:DatEquipmentId>
                                 <vxs:Description>Check-Control-System</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>25300</vxs:DatEquipmentId>
                                 <vxs:Description>Drehzahlmesser</vxs:Description>
                                 <vxs:ContainedEquipmentPositions>
                                    <vxs:EquipmentPosition>
                                       <vxs:DatEquipmentId>25607</vxs:DatEquipmentId>
                                       <vxs:Description>Energie-Control (EC)</vxs:Description>
                                    </vxs:EquipmentPosition>
                                 </vxs:ContainedEquipmentPositions>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>70100</vxs:DatEquipmentId>
                                 <vxs:Description>Dynamische Stabilitäts-Control (DSC)</vxs:Description>
                                 <vxs:EquipmentGroup>ESP</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>25607</vxs:DatEquipmentId>
                                 <vxs:Description>Energie-Control (EC)</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>35000</vxs:DatEquipmentId>
                                 <vxs:Description>Fensterheber elektrisch</vxs:Description>
                                 <vxs:EquipmentGroup>FH2</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>35405</vxs:DatEquipmentId>
                                 <vxs:Description>Fernbedienung für Zentralverriegelung</vxs:Description>
                                 <vxs:EquipmentGroup>ZV</vxs:EquipmentGroup>
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
                                 <vxs:DatEquipmentId>26708</vxs:DatEquipmentId>
                                 <vxs:Description>Geschwindigkeits-Regelanlage (Tempomat)</vxs:Description>
                                 <vxs:EquipmentGroup>TEMP</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>18802</vxs:DatEquipmentId>
                                 <vxs:Description>Heckleuchten LED</vxs:Description>
                                 <vxs:EquipmentGroup>LEDH</vxs:EquipmentGroup>
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
                                 <vxs:DatEquipmentId>34805</vxs:DatEquipmentId>
                                 <vxs:Description>Kopfstützen hinten</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>34904</vxs:DatEquipmentId>
                                 <vxs:Description>Kopfstützen hinten mechan. verstellbar (3 Stück)</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>69505</vxs:DatEquipmentId>
                                 <vxs:Description>Lenksäule (Lenkrad) mechan. verstellbar</vxs:Description>
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
                                 <vxs:DatEquipmentId>92930</vxs:DatEquipmentId>
                                 <vxs:Description>Motor 3,0 Ltr. - 173 kW Turbodiesel KAT</vxs:Description>
                                 <vxs:EquipmentClass>1</vxs:EquipmentClass>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>18300</vxs:DatEquipmentId>
                                 <vxs:Description>Nebelscheinwerfer</vxs:Description>
                                 <vxs:EquipmentGroup>BEL</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>42805</vxs:DatEquipmentId>
                                 <vxs:Description>Niveauregulierung</vxs:Description>
                                 <vxs:EquipmentGroup>NIV</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>25903</vxs:DatEquipmentId>
                                 <vxs:Description>Reifendruck-Kontrollsystem</vxs:Description>
                                 <vxs:EquipmentGroup>RDK</vxs:EquipmentGroup>
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
                                 <vxs:DatEquipmentId>33600</vxs:DatEquipmentId>
                                 <vxs:Description>Rücksitzbank klappbar</vxs:Description>
                                 <vxs:EquipmentGroup>SITH</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>77224</vxs:DatEquipmentId>
                                 <vxs:Description>Schadstoffarm nach Abgasnorm Euro 4</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>39205</vxs:DatEquipmentId>
                                 <vxs:Description>Schalt-/Wählhebelgriff Leder</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>23603</vxs:DatEquipmentId>
                                 <vxs:Description>Scheibenkleber für Warmverklebung</vxs:Description>
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
                                 <vxs:DatEquipmentId>26903</vxs:DatEquipmentId>
                                 <vxs:Description>Seitenairbag vorn</vxs:Description>
                                 <vxs:EquipmentGroup>AIR3</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>69811</vxs:DatEquipmentId>
                                 <vxs:Description>Servolenkung Servotronic</vxs:Description>
                                 <vxs:EquipmentGroup>SL</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>32607</vxs:DatEquipmentId>
                                 <vxs:Description>Sitze vorn elektr. verstellbar</vxs:Description>
                                 <vxs:EquipmentGroup>SITE</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>21300</vxs:DatEquipmentId>
                                 <vxs:Description>Stoßfänger Wagenfarbe</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>22005</vxs:DatEquipmentId>
                                 <vxs:Description>Verglasung grün getönt</vxs:Description>
                                 <vxs:EquipmentGroup>WDG</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>22302</vxs:DatEquipmentId>
                                 <vxs:Description>Wärmeschutzverglasung getönt</vxs:Description>
                                 <vxs:EquipmentGroup>WDG</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>35307</vxs:DatEquipmentId>
                                 <vxs:Description>Zentralverriegelung mit Diebstahlsicherung und Crashsensor</vxs:Description>
                                 <vxs:EquipmentGroup>ZV</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                           </vxs:SeriesEquipment>
                           <vxs:SpecialEquipment>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>4905</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>7RP</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>ADVANTAGE PAKET</vxs:ManufacturerDescription>
                                 <vxs:Description>Advantage-Paket</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>2701</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>715</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>M AERODYNAMIKPAKET</vxs:ManufacturerDescription>
                                 <vxs:Description>Aerodynamik-Paket M-Technic</vxs:Description>
                                 <vxs:EquipmentGroup>SPOI</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>25805</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>633</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>HANDY VORB. BUSINESS/BLUETOOTH-SCH.</vxs:ManufacturerDescription>
                                 <vxs:Description>Audio-Navigationssystem Professional mit integrierter Handyvorrüstung</vxs:Description>
                                 <vxs:EquipmentGroup>GPS</vxs:EquipmentGroup>
                                 <vxs:ContainedEquipmentPositions>
                                    <vxs:EquipmentPosition>
                                       <vxs:DatEquipmentId>24106</vxs:DatEquipmentId>
                                       <vxs:Description>Audiosystem BMW Professional (Radio/CD-Player)</vxs:Description>
                                       <vxs:EquipmentGroup>CD</vxs:EquipmentGroup>
                                    </vxs:EquipmentPosition>
                                    <vxs:EquipmentPosition>
                                       <vxs:DatEquipmentId>24707</vxs:DatEquipmentId>
                                       <vxs:Description>Vorrüstung Mobiltelefon/Handy</vxs:Description>
                                       <vxs:EquipmentGroup>TEL1</vxs:EquipmentGroup>
                                    </vxs:EquipmentPosition>
                                    <vxs:EquipmentPosition>
                                       <vxs:DatEquipmentId>24811</vxs:DatEquipmentId>
                                       <vxs:Description>Vorrüstung Mobiltelefon/Handy Business mit Bluetooth Schnittstelle</vxs:Description>
                                       <vxs:EquipmentGroup>TEL1</vxs:EquipmentGroup>
                                    </vxs:EquipmentPosition>
                                 </vxs:ContainedEquipmentPositions>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>8702</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>760</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>M HOCHGLANZ SHADOW LINE</vxs:ManufacturerDescription>
                                 <vxs:Description>Außenausstattung: Shadow-Line Hochglanz</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>27804</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>775</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>M DACHHIMMEL ANTHRAZIT</vxs:ManufacturerDescription>
                                 <vxs:Description>Dachhimmel Anthrazit</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>16000</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>386</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>DACHRELING</vxs:ManufacturerDescription>
                                 <vxs:Description>Dachreling</vxs:Description>
                                 <vxs:EquipmentGroup>DARE</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>75904</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>205</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>AUTOMATIC GETRIEBE</vxs:ManufacturerDescription>
                                 <vxs:Description>Getriebe Automatik - mit Steptronic (6-Stufen)</vxs:Description>
                                 <vxs:EquipmentGroup>AG2</vxs:EquipmentGroup>
                                 <vxs:EquipmentClass>11</vxs:EquipmentClass>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>38908</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>442</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>GETRAENKEHALTER</vxs:ManufacturerDescription>
                                 <vxs:Description>Getränkehalter</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>24607</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>676</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>HIFI LAUTSPRECHERSYSTEM</vxs:ManufacturerDescription>
                                 <vxs:Description>HiFi-Lautsprechersystem</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>31704</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>438</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>EDELHOLZAUSFUEHRUNG</vxs:ManufacturerDescription>
                                 <vxs:Description>Innenausstattung: Edelholz</vxs:Description>
                                 <vxs:ContainedEquipmentPositions>
                                    <vxs:EquipmentPosition>
                                       <vxs:DatEquipmentId>26217</vxs:DatEquipmentId>
                                       <vxs:Description>Innenausstattung: Interieurleisten Edelholz</vxs:Description>
                                    </vxs:EquipmentPosition>
                                 </vxs:ContainedEquipmentPositions>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>26217</vxs:DatEquipmentId>
                                 <vxs:Description>Innenausstattung: Interieurleisten Edelholz</vxs:Description>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>28807</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>534</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>KLIMAAUTOMATIK</vxs:ManufacturerDescription>
                                 <vxs:Description>Klimaautomatik erweiterter Umfang</vxs:Description>
                                 <vxs:EquipmentGroup>KLI2</vxs:EquipmentGroup>
                                 <vxs:ContainedEquipmentPositions>
                                    <vxs:EquipmentPosition>
                                       <vxs:DatEquipmentId>27206</vxs:DatEquipmentId>
                                       <vxs:Description>Mittelarmlehne vorn verstellbar</vxs:Description>
                                       <vxs:EquipmentGroup>MALV</vxs:EquipmentGroup>
                                    </vxs:EquipmentPosition>
                                 </vxs:ContainedEquipmentPositions>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>69204</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>710</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>M LEDERLENKRAD</vxs:ManufacturerDescription>
                                 <vxs:Description>Lenkrad (Sport M-Technic)</vxs:Description>
                                 <vxs:EquipmentGroup>LEN6</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>49405</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>2NP</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>M LM R. DOPPELSPEICHE 135 M NOTLAUF</vxs:ManufacturerDescription>
                                 <vxs:Description>LM-Felgen 8x18 (M Doppelspeichen 135)</vxs:Description>
                                 <vxs:EquipmentGroup>ALU</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>11000</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>M</vxs:ManufacturerEquipmentId>
                                 <vxs:Description>Metallic-Lackierung</vxs:Description>
                                 <vxs:EquipmentGroup>SONL</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>27206</vxs:DatEquipmentId>
                                 <vxs:Description>Mittelarmlehne vorn verstellbar</vxs:Description>
                                 <vxs:EquipmentGroup>MALV</vxs:EquipmentGroup>
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
                                 <vxs:DatEquipmentId>19000</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>502</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>SCHEINWERFER-WASCHANLAGE</vxs:ManufacturerDescription>
                                 <vxs:Description>Scheinwerfer-Reinigungsanlage (SRA)</vxs:Description>
                                 <vxs:EquipmentGroup>SWRA</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>30109</vxs:DatEquipmentId>
                                 <vxs:Description>Sitzbezug / Polsterung: Stoff / Leder</vxs:Description>
                                 <vxs:EquipmentGroup>LED1</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>29500</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>494</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>SITZHEIZUNG FUER FAHRER/BEIFAHRER</vxs:ManufacturerDescription>
                                 <vxs:Description>Sitzheizung vorn</vxs:Description>
                                 <vxs:EquipmentGroup>SITB</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>39103</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>464</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>SKISACK</vxs:ManufacturerDescription>
                                 <vxs:Description>Skisack</vxs:Description>
                                 <vxs:EquipmentGroup>DULA</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>3209</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>337</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>M SPORTPAKET</vxs:ManufacturerDescription>
                                 <vxs:Description>Sport-Paket M / M-Technic</vxs:Description>
                                 <vxs:ContainedEquipmentPositions>
                                    <vxs:EquipmentPosition>
                                       <vxs:DatEquipmentId>8701</vxs:DatEquipmentId>
                                       <vxs:Description>Außenausstattung: Shadow-Line</vxs:Description>
                                    </vxs:EquipmentPosition>
                                    <vxs:EquipmentPosition>
                                       <vxs:DatEquipmentId>27804</vxs:DatEquipmentId>
                                       <vxs:Description>Dachhimmel Anthrazit</vxs:Description>
                                    </vxs:EquipmentPosition>
                                    <vxs:EquipmentPosition>
                                       <vxs:DatEquipmentId>30109</vxs:DatEquipmentId>
                                       <vxs:Description>Sitzbezug / Polsterung: Stoff / Leder</vxs:Description>
                                       <vxs:EquipmentGroup>LED1</vxs:EquipmentGroup>
                                    </vxs:EquipmentPosition>
                                    <vxs:EquipmentPosition>
                                       <vxs:DatEquipmentId>31901</vxs:DatEquipmentId>
                                       <vxs:Description>Sportsitze vorn</vxs:Description>
                                       <vxs:EquipmentGroup>SPSI</vxs:EquipmentGroup>
                                    </vxs:EquipmentPosition>
                                    <vxs:EquipmentPosition>
                                       <vxs:DatEquipmentId>42100</vxs:DatEquipmentId>
                                       <vxs:Description>Sportliche Fahrwerksabstimmung</vxs:Description>
                                       <vxs:EquipmentGroup>SPFW</vxs:EquipmentGroup>
                                    </vxs:EquipmentPosition>
                                    <vxs:EquipmentPosition>
                                       <vxs:DatEquipmentId>69204</vxs:DatEquipmentId>
                                       <vxs:Description>Lenkrad (Sport M-Technic)</vxs:Description>
                                       <vxs:EquipmentGroup>LEN6</vxs:EquipmentGroup>
                                    </vxs:EquipmentPosition>
                                 </vxs:ContainedEquipmentPositions>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>42100</vxs:DatEquipmentId>
                                 <vxs:Description>Sportliche Fahrwerksabstimmung</vxs:Description>
                                 <vxs:EquipmentGroup>SPFW</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>31901</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>481</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>SPORTSITZE FUER FAHRER/BEIFAHRER</vxs:ManufacturerDescription>
                                 <vxs:Description>Sportsitze vorn</vxs:Description>
                                 <vxs:EquipmentGroup>SPSI</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>25010</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>6FL</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>USB-AUDIO-SCHNITTSTELLE</vxs:ManufacturerDescription>
                                 <vxs:Description>USB-Schnittstelle</vxs:Description>
                                 <vxs:EquipmentGroup>MP3A</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>24707</vxs:DatEquipmentId>
                                 <vxs:Description>Vorrüstung Mobiltelefon/Handy</vxs:Description>
                                 <vxs:EquipmentGroup>TEL1</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>24811</vxs:DatEquipmentId>
                                 <vxs:Description>Vorrüstung Mobiltelefon/Handy Business mit Bluetooth Schnittstelle</vxs:Description>
                                 <vxs:EquipmentGroup>TEL1</vxs:EquipmentGroup>
                              </vxs:EquipmentPosition>
                              <vxs:EquipmentPosition>
                                 <vxs:DatEquipmentId>18008</vxs:DatEquipmentId>
                                 <vxs:ManufacturerEquipmentId>522</vxs:ManufacturerEquipmentId>
                                 <vxs:ManufacturerDescription>XENON-LICHT</vxs:ManufacturerDescription>
                                 <vxs:Description>Xenon-Scheinwerfer</vxs:Description>
                                 <vxs:EquipmentGroup>XELI</vxs:EquipmentGroup>
                                 <vxs:ContainedEquipmentPositions>
                                    <vxs:EquipmentPosition>
                                       <vxs:DatEquipmentId>18904</vxs:DatEquipmentId>
                                       <vxs:Description>Tagfahrlicht</vxs:Description>
                                       <vxs:EquipmentGroup>TFAL</vxs:EquipmentGroup>
                                    </vxs:EquipmentPosition>
                                    <vxs:EquipmentPosition>
                                       <vxs:DatEquipmentId>19000</vxs:DatEquipmentId>
                                       <vxs:Description>Scheinwerfer-Reinigungsanlage (SRA)</vxs:Description>
                                       <vxs:EquipmentGroup>SWRA</vxs:EquipmentGroup>
                                    </vxs:EquipmentPosition>
                                 </vxs:ContainedEquipmentPositions>
                              </vxs:EquipmentPosition>
                           </vxs:SpecialEquipment>
                        </vxs:Equipment>
                        <vxs:DATECodeEquipment>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>92930</vxs:DatEquipmentId>
                              <vxs:Description>Motor 3,0 Ltr. - 173 kW Turbodiesel KAT</vxs:Description>
                              <vxs:EquipmentClass>1</vxs:EquipmentClass>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>10005</vxs:DatEquipmentId>
                              <vxs:Description>Karosserie: 5-türig</vxs:Description>
                              <vxs:EquipmentClass>2</vxs:EquipmentClass>
                           </vxs:EquipmentPosition>
                           <vxs:EquipmentPosition>
                              <vxs:DatEquipmentId>75904</vxs:DatEquipmentId>
                              <vxs:Description>Getriebe Automatik - mit Steptronic (6-Stufen)</vxs:Description>
                              <vxs:EquipmentClass>11</vxs:EquipmentClass>
                           </vxs:EquipmentPosition>
                        </vxs:DATECodeEquipment>
                        <vxs:VINResult>
                           <vxs:VinInterfaceVersion>2.5</vxs:VinInterfaceVersion>
                           <vxs:VINECodes>
                              <vxs:VINECode>
                                 <vxs:Sign>0</vxs:Sign>
                                 <vxs:VehicleTypeKey>1</vxs:VehicleTypeKey>
                                 <vxs:ManufacturerKey>130</vxs:ManufacturerKey>
                                 <vxs:VehicleMainTypeKey>66</vxs:VehicleMainTypeKey>
                                 <vxs:VehicleSubTypeKey>34</vxs:VehicleSubTypeKey>
                                 <vxs:VehicleSubTypeVariantKey>6</vxs:VehicleSubTypeVariantKey>
                                 <vxs:ConstructionTimeMin>4510</vxs:ConstructionTimeMin>
                                 <vxs:ConstructionTime>4518</vxs:ConstructionTime>
                                 <vxs:ConstructionTimeEdge>4290</vxs:ConstructionTimeEdge>
                                 <vxs:ConstructionTimeProd>4518</vxs:ConstructionTimeProd>
                                 <vxs:ConstructionTimePriceList>4470</vxs:ConstructionTimePriceList>
                                 <vxs:VINContainers>
                                    <vxs:VINContainer>
                                       <vxs:Container>002</vxs:Container>
                                       <vxs:VehicleTypeKey>5</vxs:VehicleTypeKey>
                                       <vxs:ManufacturerKey>130</vxs:ManufacturerKey>
                                       <vxs:VehicleMainTypeKey>3216</vxs:VehicleMainTypeKey>
                                       <vxs:VehicleSubTypeKey>16</vxs:VehicleSubTypeKey>
                                       <vxs:VehicleConstructionTime>4518</vxs:VehicleConstructionTime>
                                    </vxs:VINContainer>
                                 </vxs:VINContainers>
                              </vxs:VINECode>
                           </vxs:VINECodes>
                           <vxs:VINEquipments>
                              <vxs:VINEquipment>
                                 <vxs:ShortName>Model: 530XD (E61)</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>548</vxs:ManufacturerCode>
                                 <vxs:ShortName>KILOMETERTACHO</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>612</vxs:ManufacturerCode>
                                 <vxs:ShortName>BMW ASSIST</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>698</vxs:ManufacturerCode>
                                 <vxs:ShortName>AREA-CODE 2</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>6AA</vxs:ManufacturerCode>
                                 <vxs:ShortName>BMW TELESERVICES</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>851</vxs:ManufacturerCode>
                                 <vxs:ShortName>SPRACHVERSION DEUTSCH</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>863</vxs:ManufacturerCode>
                                 <vxs:ShortName>SERVICE KONTAKT-FLYER EUROPA</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>8S8</vxs:ManufacturerCode>
                                 <vxs:ShortName>LAENDERSPEZ. NAVI ZUST. (FUER ACC)</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>8SA</vxs:ManufacturerCode>
                                 <vxs:ShortName>LAENDERSPEZ. NAVI.-FREISCHALTUNG</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>8SP</vxs:ManufacturerCode>
                                 <vxs:ShortName>COP STEUERUNG</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>COUNTRY:DE</vxs:ManufacturerCode>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>M57/T2/3.00/173</vxs:ManufacturerCode>
                                 <vxs:ShortName>3.00L / 173kW</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>TypeA:PY81</vxs:ManufacturerCode>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>TypeB:PY71</vxs:ManufacturerCode>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>VIN10:0</vxs:ManufacturerCode>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>VIN11:C</vxs:ManufacturerCode>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:ManufacturerCode>WHC:WBA</vxs:ManufacturerCode>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>789</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>320</vxs:ManufacturerCode>
                                 <vxs:ShortName>MODELLSCHRIFTZUG ENTFALL</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>1420</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>7RP</vxs:ManufacturerCode>
                                 <vxs:ShortName>ADVANTAGE PAKET</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>2701</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>715</vxs:ManufacturerCode>
                                 <vxs:ShortName>M AERODYNAMIKPAKET</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>3209</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>337</vxs:ManufacturerCode>
                                 <vxs:ShortName>M SPORTPAKET</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>3306</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>715</vxs:ManufacturerCode>
                                 <vxs:ShortName>M AERODYNAMIKPAKET</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>4905</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>7RP</vxs:ManufacturerCode>
                                 <vxs:ShortName>ADVANTAGE PAKET</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>8701</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>760</vxs:ManufacturerCode>
                                 <vxs:ShortName>M HOCHGLANZ SHADOW LINE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>8702</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>760</vxs:ManufacturerCode>
                                 <vxs:ShortName>M HOCHGLANZ SHADOW LINE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>11000</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>416M</vxs:ManufacturerCode>
                                 <vxs:ShortName>CARBONSCHWARZ METALLIC</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>11000</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>M</vxs:ManufacturerCode>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>16000</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>386</vxs:ManufacturerCode>
                                 <vxs:ShortName>DACHRELING</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>16195</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>386</vxs:ManufacturerCode>
                                 <vxs:ShortName>DACHRELING</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>16302</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>402</vxs:ManufacturerCode>
                                 <vxs:ShortName>PANORAMA GLASDACH</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>18008</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>522</vxs:ManufacturerCode>
                                 <vxs:ShortName>XENON-LICHT</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>18505</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>522</vxs:ManufacturerCode>
                                 <vxs:ShortName>XENON-LICHT</vxs:ShortName>
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
                                 <vxs:AvNumberDat>24607</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>676</vxs:ManufacturerCode>
                                 <vxs:ShortName>HIFI LAUTSPRECHERSYSTEM</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>24705</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>616</vxs:ManufacturerCode>
                                 <vxs:ShortName>BMW ONLINE</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>24709</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>620</vxs:ManufacturerCode>
                                 <vxs:ShortName>SPRACHEINGABESYSTEM</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>25010</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>6FL</vxs:ManufacturerCode>
                                 <vxs:ShortName>USB-AUDIO-SCHNITTSTELLE</vxs:ShortName>
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
                                 <vxs:AvNumberDat>25805</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>633</vxs:ManufacturerCode>
                                 <vxs:ShortName>HANDY VORB. BUSINESS/BLUETOOTH-SCH.</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>26710</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>544</vxs:ManufacturerCode>
                                 <vxs:ShortName>GESCHWINDIGKEITSREGEL. MIT BREMSF.</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>27804</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>775</vxs:ManufacturerCode>
                                 <vxs:ShortName>M DACHHIMMEL ANTHRAZIT</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>27810</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>775</vxs:ManufacturerCode>
                                 <vxs:ShortName>M DACHHIMMEL ANTHRAZIT</vxs:ShortName>
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
                                 <vxs:ManufacturerCode>LCBA</vxs:ManufacturerCode>
                                 <vxs:ShortName>LEDER DAKOTA/BEIGE 3</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>31304</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>438</vxs:ManufacturerCode>
                                 <vxs:ShortName>EDELHOLZAUSFUEHRUNG</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>31312</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>438</vxs:ManufacturerCode>
                                 <vxs:ShortName>EDELHOLZAUSFUEHRUNG</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>31700</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>438</vxs:ManufacturerCode>
                                 <vxs:ShortName>EDELHOLZAUSFUEHRUNG</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>31704</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>438</vxs:ManufacturerCode>
                                 <vxs:ShortName>EDELHOLZAUSFUEHRUNG</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>31810</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>481</vxs:ManufacturerCode>
                                 <vxs:ShortName>SPORTSITZE FUER FAHRER/BEIFAHRER</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>31901</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>481</vxs:ManufacturerCode>
                                 <vxs:ShortName>SPORTSITZE FUER FAHRER/BEIFAHRER</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>32002</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>481</vxs:ManufacturerCode>
                                 <vxs:ShortName>SPORTSITZE FUER FAHRER/BEIFAHRER</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>32006</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>481</vxs:ManufacturerCode>
                                 <vxs:ShortName>SPORTSITZE FUER FAHRER/BEIFAHRER</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>38908</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>442</vxs:ManufacturerCode>
                                 <vxs:ShortName>GETRAENKEHALTER</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>38909</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>442</vxs:ManufacturerCode>
                                 <vxs:ShortName>GETRAENKEHALTER</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>38999</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>428</vxs:ManufacturerCode>
                                 <vxs:ShortName>WARNDREIECK</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>39103</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>464</vxs:ManufacturerCode>
                                 <vxs:ShortName>SKISACK</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>49405</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>2NP</vxs:ManufacturerCode>
                                 <vxs:ShortName>M LM R. DOPPELSPEICHE 135 M NOTLAUF</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>69103</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>710</vxs:ManufacturerCode>
                                 <vxs:ShortName>M LEDERLENKRAD</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>69204</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>710</vxs:ManufacturerCode>
                                 <vxs:ShortName>M LEDERLENKRAD</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>69309</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>710</vxs:ManufacturerCode>
                                 <vxs:ShortName>M LEDERLENKRAD</vxs:ShortName>
                              </vxs:VINEquipment>
                              <vxs:VINEquipment>
                                 <vxs:AvNumberDat>70410</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>203</vxs:ManufacturerCode>
                                 <vxs:ShortName>ALLRADSYSTEM</vxs:ShortName>
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
                                 <vxs:AvNumberDat>97741</vxs:AvNumberDat>
                                 <vxs:ManufacturerCode>337</vxs:ManufacturerCode>
                                 <vxs:ShortName>M SPORTPAKET</vxs:ShortName>
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
                                 <vxs:Code>416</vxs:Code>
                                 <vxs:Description>CARBONSCHWARZ METALLIC</vxs:Description>
                                 <vxs:StandardColor>9</vxs:StandardColor>
                                 <vxs:PaintType>31</vxs:PaintType>
                                 <vxs:CountCoat>2 COAT</vxs:CountCoat>
                              </vxs:VINColor>
                              <vxs:VINColor>
                                 <vxs:ColorID>I1</vxs:ColorID>
                                 <vxs:Code>LCBA</vxs:Code>
                                 <vxs:Description>LEDER DAKOTA/BEIGE 3</vxs:Description>
                              </vxs:VINColor>
                              <vxs:VINColor>
                                 <vxs:ColorID>PM</vxs:ColorID>
                                 <vxs:Code/>
                                 <vxs:Description>LEDER DAKOTA</vxs:Description>
                              </vxs:VINColor>
                              <vxs:VINColor>
                                 <vxs:ColorID>PF</vxs:ColorID>
                                 <vxs:Code/>
                                 <vxs:Description>BEIGE 3</vxs:Description>
                              </vxs:VINColor>
                           </vxs:VINColors>
                           <vxs:VINVehicle>
                              <vxs:VINumber>
                                 <vxs:VinCode>WBAPY71050CU14918</vxs:VinCode>
                              </vxs:VINumber>
                              <vxs:ManufacturerCarCode>PY81</vxs:ManufacturerCarCode>
                           </vxs:VINVehicle>
                        </vxs:VINResult>
                        <vxs:TokenOfVinResult>eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJkYXQiLCJ0aW1lc3RhbXAiOjE2NTIxODQ3MzQxOTksImN1c3RvbWVyIjoiMTM0MDc4OSIsImludGVyZmFjZVBhcnRuZXIiOiIxMzQwNzg5IiwidmluUmVzdWx0SGFzaCI6Imhhc2gwMV8xNTA0ODM2NDQ0In0.nDx1BTidf1NQdiga40nOJksH31kk-vYegQywOtUJ3EU</vxs:TokenOfVinResult>
                     </vxs:Vehicle>
                     <vxs:RepairParameters>
                        <vxs:PhantomCalculation>false</vxs:PhantomCalculation>
                     </vxs:RepairParameters>
                     <vxs:ProcedureRelatedParameters>
                        <vxs:ProcedureRelatedParameter factor="CalculationFactor" attribute="serialCalculation" type="CrossSeriesState">NO</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="CalculationFactor" attribute="timeUnit" type="TimeUnitSystem">HOUR</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="CalculationFactor" attribute="timeUnitsPerHour" type="Integer">1</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="LabourCostFactor" attribute="mechanicWage1" type="Price" mode="PER_HOUR">105.00</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="LabourCostFactor" attribute="electricWage1" type="Price" mode="PER_HOUR">105.00</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="LabourCostFactor" attribute="bodyWage1" type="Price" mode="PER_HOUR">105.00</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter type="Price" attribute="dentWage" factor="LabourCostFactor" mode="PER_HOUR">78.00</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter type="LacquerMethod" attribute="selectedLacquerMethod" factor="CalculationFactor">MANUFACTURER_SPECIFIC</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter attribute="type" factor="ManufacturerLacquerFactor" type="String">12</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter type="TimeUnitSystem" attribute="timeUnit" factor="ManufacturerLacquerFactor">HOUR</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="ManufacturerLacquerFactor" attribute="wage" type="Price" mode="PER_HOUR">120.00</vxs:ProcedureRelatedParameter>
                        <vxs:ProcedureRelatedParameter factor="ManufacturerLacquerFactor" attribute="materialFlatRatePercent" type="Double">25</vxs:ProcedureRelatedParameter>
                     </vxs:ProcedureRelatedParameters>
                     <vxs:RepairPositions>
                        <!--Frontklappe ersetzen-->
                        <vxs:RepairPosition>
                           <vxs:DATProcessId>44210</vxs:DATProcessId>
                           <vxs:RepairType>replace</vxs:RepairType>
                           <vxs:Description>Frontklappe</vxs:Description>
                           <vxs:ConstructionGroupId>1</vxs:ConstructionGroupId>
                           <vxs:ConstructionGroup>VORDERWAGEN AUSSEN</vxs:ConstructionGroup>
                           <vxs:PositionEntryType>graphical</vxs:PositionEntryType>
                           <vxs:ConstructionType>6</vxs:ConstructionType>
                           <vxs:SparePartUsed>false</vxs:SparePartUsed>
                           <vxs:PreDamage>false</vxs:PreDamage>
                        </vxs:RepairPosition>
                        <!--Kotflügl instandssetzen-->
                        <vxs:RepairPosition>
                           <vxs:DATProcessId>43711</vxs:DATProcessId>
                           <vxs:RepairType>overhaul</vxs:RepairType>
                           <vxs:Description>Kotflügel</vxs:Description>
                           <vxs:ConstructionGroupId>1</vxs:ConstructionGroupId>
                           <vxs:ConstructionGroup>VORDERWAGEN AUSSEN</vxs:ConstructionGroup>
                           <vxs:PositionEntryType>graphical</vxs:PositionEntryType>
                           <vxs:ConstructionType>6</vxs:ConstructionType>
                           <vxs:SparePartUsed>false</vxs:SparePartUsed>
                           <vxs:WorkTime>0.1</vxs:WorkTime>
                           <vxs:PreDamage>false</vxs:PreDamage>
                        </vxs:RepairPosition>
                     </vxs:RepairPositions>
                  </vxs:RepairCalculation>
                  <vxs:RepairOrder>
                     <vxs:DamageDate>2017-02-01T00:00:00+01:00</vxs:DamageDate>
                     <vxs:PolicyNumber>12345678</vxs:PolicyNumber>
                     <vxs:Retention>true</vxs:Retention>
                     <vxs:RetentionAmount>300</vxs:RetentionAmount>
                     <vxs:InsuranceId>999</vxs:InsuranceId>
                     <vxs:InsuranceGroupId>DAT01</vxs:InsuranceGroupId>
                     <vxs:InsuranceType>partial</vxs:InsuranceType>
                     <vxs:DamageType>912</vxs:DamageType>
                     <vxs:DeclarationOfAssignment>true</vxs:DeclarationOfAssignment>
                     <vxs:CreationDateTime>2017-03-14T08:31:11.081+01:00</vxs:CreationDateTime>
                     <vxs:InsuranceNumber>DAT01</vxs:InsuranceNumber>
                     <vxs:TypeOfInsurance>1</vxs:TypeOfInsurance>
                     <vxs:InsuranceName>DAT Testversicherung</vxs:InsuranceName>
                  </vxs:RepairOrder>
                  <vxs:InsuranceClaim>true</vxs:InsuranceClaim>
               </vxs:Dossier>
            </dossiers>
            <locale country="DE" datCountryIndicator="DE" language="de"/>
            <withoutCafi>false</withoutCafi>
         </request>
      </veh:importDossier>
   </soapenv:Body>
</soapenv:Envelope>
