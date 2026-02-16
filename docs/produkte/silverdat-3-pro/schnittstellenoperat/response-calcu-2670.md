---
title: "Response calculate"
topic_id: "2670"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > Kalkulieren eines Fahrzeugs ohne Speicherung > Response calculate"
---

# Response calculate

<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns10:calculateResponse xmlns:ns10="http://www.dat.eu/myClaim/soap/v2/VehicleRepairService">
         <calculationResult source="SD3" type="VehicleRepairOnline">
            <ns1:Dossier xmlns:ns1="http://www.dat.de/vxs">
               <ns1:UUID>be6c971e-4c4a-42b1-acc2-cf8185684452</ns1:UUID>
               <ns1:DossierId>0</ns1:DossierId>
               <ns1:IdSD3Network>0</ns1:IdSD3Network>
               <ns1:Country>DE</ns1:Country>
               <ns1:Language>de_DE</ns1:Language>
               <ns1:DataVersion>1</ns1:DataVersion>
               <ns1:Currency>EUR</ns1:Currency>
               <ns1:DatCustomerId>999999</ns1:DatCustomerId>
               <ns1:DossierType>myClaim</ns1:DossierType>
               <ns1:CreateDate>2023-12-22T14:51:28.178+01:00</ns1:CreateDate>
               <ns1:CreateUser>Anwender</ns1:CreateUser>
               <ns1:ChangeDate>2023-12-22T14:51:28.400+01:00</ns1:ChangeDate>
               <ns1:DatCustomerAddress>
                  <ns1:Title>titleCompany</ns1:Title>
                  <ns1:CompanyName>PL-C-S Test</ns1:CompanyName>
                  <ns1:NameLong>DAT intern</ns1:NameLong>
                  <ns1:Country>DE</ns1:Country>
                  <ns1:TaxNumber>123123</ns1:TaxNumber>
                  <ns1:CustomerNumber>999999</ns1:CustomerNumber>
                  <ns1:CustomerType>999999</ns1:CustomerType>
                  <ns1:Street>Hellmuth-Hirth-Str.</ns1:Street>
                  <ns1:StreetNumber>1</ns1:StreetNumber>
                  <ns1:StreetZipCode>73630</ns1:StreetZipCode>
                  <ns1:StreetCity>Ostfildern</ns1:StreetCity>
                  <ns1:EMail>email@dat.de</ns1:EMail>
                  <ns1:BIC>123123</ns1:BIC>
                  <ns1:IBAN>DE123123123</ns1:IBAN>
                  <ns1:UsageFlag>9</ns1:UsageFlag>
               </ns1:DatCustomerAddress>
               <ns1:Vehicle>
                  <ns1:DatECode>011940020020001</ns1:DatECode>
                  <ns1:ConstructionTime>4567</ns1:ConstructionTime>
                  <ns1:VehicleTypeName origin="dat">Pkw, SUV, Kleintransporter</ns1:VehicleTypeName>
                  <ns1:VehicleTypeNameN origin="dat">Pkw, SUV, Kleintransporter</ns1:VehicleTypeNameN>
                  <ns1:ManufacturerName origin="dat">Dacia</ns1:ManufacturerName>
                  <ns1:BaseModelName origin="dat">Logan MCV Kombi (12.2006->)</ns1:BaseModelName>
                  <ns1:SubModelName origin="dat">Ambiance</ns1:SubModelName>
                  <ns1:VehicleType>1</ns1:VehicleType>
                  <ns1:Manufacturer>194</ns1:Manufacturer>
                  <ns1:BaseModel>2</ns1:BaseModel>
                  <ns1:SubModel>2</ns1:SubModel>
                  <ns1:Country>DE</ns1:Country>
                  <ns1:SubModelVariant>1</ns1:SubModelVariant>
                  <ns1:RegistrationData/>
                  <ns1:Engine>
                     <ns1:EnginePowerKw origin="dat">55</ns1:EnginePowerKw>
                     <ns1:EnginePowerHp origin="dat">74</ns1:EnginePowerHp>
                     <ns1:Cylinders origin="dat">4</ns1:Cylinders>
                     <ns1:Capacity origin="dat">1390</ns1:Capacity>
                     <ns1:Consumption>7.6</ns1:Consumption>
                     <ns1:Co2Emission>180.0</ns1:Co2Emission>
                  </ns1:Engine>
                  <ns1:TechInfo>
                     <ns1:FillingQuantities>
                        <ns1:Fluid code="JH3 5/1" desc="Schalttransaxle" type="3">
                           <ns1:Capacity desc="Füllmenge (gesamt)" min="2.80" unit="Liter"/>
                           <ns1:Recommendation>
                              <ns1:Usage type="0">Normal</ns1:Usage>
                              <ns1:Product>TITAN SINTOFLUID SAE 75W-80</ns1:Product>
                           </ns1:Recommendation>
                        </ns1:Fluid>
                        <ns1:Fluid desc="Kühlsystem" type="8">
                           <ns1:Capacity desc="Füllmenge (gesamt)" min="4.50" unit="Liter"/>
                           <ns1:Recommendation>
                              <ns1:Usage type="0">Normal</ns1:Usage>
                              <ns1:Interval type="1">Wechseln 90000 km/ 48 Monate</ns1:Interval>
                              <ns1:Interval type="2">Prüfen 15000 km/ 12 Monate</ns1:Interval>
                              <ns1:Product>MAINTAIN FRICOFIN LL</ns1:Product>
                           </ns1:Recommendation>
                        </ns1:Fluid>
                        <ns1:Fluid code="JH1 5/1" desc="Schalttransaxle" type="3">
                           <ns1:Capacity desc="Füllmenge (gesamt)" min="2.80" unit="Liter"/>
                           <ns1:Recommendation>
                              <ns1:Usage type="0">Normal</ns1:Usage>
                              <ns1:Product>TITAN SINTOFLUID SAE 75W-80</ns1:Product>
                           </ns1:Recommendation>
                        </ns1:Fluid>
                        <ns1:Fluid desc="Hydraulisches Brems-/Kupplungssystem" type="4">
                           <ns1:Capacity desc="Füllmenge (gesamt)" min="0.50" unit="Liter"/>
                           <ns1:Recommendation>
                              <ns1:Usage type="0">Normal</ns1:Usage>
                              <ns1:Interval type="2">Prüfen 15000 km/ 12 Monate</ns1:Interval>
                              <ns1:Interval type="1">Wechseln 90000 km/ 48 Monate</ns1:Interval>
                              <ns1:Product>MAINTAIN DOT 5.1</ns1:Product>
                              <ns1:Product>MAINTAIN DOT 4</ns1:Product>
                           </ns1:Recommendation>
                        </ns1:Fluid>
                        <ns1:Fluid code="K7J" desc="Motor" type="1">
                           <ns1:Capacity desc="Filterkapazität" min="0.10" unit="Liter"/>
                           <ns1:Recommendation>
                              <ns1:Usage type="3449">Schwere Einsatzbedingungen</ns1:Usage>
                              <ns1:Interval type="1">Wechseln 15000 km/ 6 Monate</ns1:Interval>
                              <ns1:Product>TITAN Supersyn SAE 5W-30</ns1:Product>
                              <ns1:Product>TITAN Supersyn SAE 5W-40</ns1:Product>
                              <ns1:Product>TITAN Supersyn LONGLIFE SAE 0W-40</ns1:Product>
                              <ns1:Product>TITAN SYN MC SAE 10W-40</ns1:Product>
                              <ns1:Product>TITAN Supersyn F Eco-DT SAE 5W-30</ns1:Product>
                              <ns1:Product>TITAN Supersyn LONGLIFE SAE 0W-30</ns1:Product>
                              <ns1:Product>TITAN GT1 PRO 229.6 SAE 5W-30 (XTL-Technology)</ns1:Product>
                              <ns1:Product>TITAN Supersyn FE SAE 0W-30</ns1:Product>
                              <ns1:Product>TITAN Supersyn LONGLIFE SAE 5W-40</ns1:Product>
                              <ns1:Product>TITAN UNIMAX ULTRA MC SAE 10W-40</ns1:Product>
                           </ns1:Recommendation>
                        </ns1:Fluid>
                        <ns1:Fluid code="K7J" desc="Motor" type="1">
                           <ns1:Capacity desc="Filterkapazität" min="0.10" unit="Liter"/>
                           <ns1:Recommendation>
                              <ns1:Usage type="0">Normal</ns1:Usage>
                              <ns1:Interval type="2">Prüfen 15000 km/ 12 Monate</ns1:Interval>
                              <ns1:Interval type="1">Wechseln 30000 km/ 24 Monate</ns1:Interval>
                              <ns1:Product>TITAN Supersyn SAE 5W-30</ns1:Product>
                              <ns1:Product>TITAN GT1 PRO 229.6 SAE 5W-30 (XTL-Technology)</ns1:Product>
                              <ns1:Product>TITAN SYN MC SAE 10W-40</ns1:Product>
                              <ns1:Product>TITAN Supersyn LONGLIFE SAE 5W-40</ns1:Product>
                              <ns1:Product>TITAN Supersyn F Eco-DT SAE 5W-30</ns1:Product>
                              <ns1:Product>TITAN Supersyn LONGLIFE SAE 0W-40</ns1:Product>
                              <ns1:Product>TITAN UNIMAX ULTRA MC SAE 10W-40</ns1:Product>
                              <ns1:Product>TITAN Supersyn LONGLIFE SAE 0W-30</ns1:Product>
                              <ns1:Product>TITAN Supersyn SAE 5W-40</ns1:Product>
                              <ns1:Product>TITAN Supersyn FE SAE 0W-30</ns1:Product>
                           </ns1:Recommendation>
                        </ns1:Fluid>
                        <ns1:Fluid code="JR5 5/1" desc="Schalttransaxle" type="3">
                           <ns1:Capacity desc="Füllmenge (gesamt)" min="2.50" unit="Liter"/>
                           <ns1:Recommendation>
                              <ns1:Usage type="0">Normal</ns1:Usage>
                              <ns1:Product>TITAN SINTOFLUID SAE 75W-80</ns1:Product>
                           </ns1:Recommendation>
                        </ns1:Fluid>
                     </ns1:FillingQuantities>
                     <ns1:PowerHp origin="dat">75</ns1:PowerHp>
                     <ns1:PowerKw origin="dat">55.0</ns1:PowerKw>
                     <ns1:Capacity origin="dat">1390</ns1:Capacity>
                     <ns1:Cylinder origin="dat">4</ns1:Cylinder>
                     <ns1:CylinderArrangement origin="dat">R</ns1:CylinderArrangement>
                     <ns1:GearboxType>manual</ns1:GearboxType>
                     <ns1:ConsumptionInTown origin="dat">10.0</ns1:ConsumptionInTown>
                     <ns1:ConsumptionOutOfTown origin="dat">6.2</ns1:ConsumptionOutOfTown>
                     <ns1:Consumption origin="dat">7.6</ns1:Consumption>
                     <ns1:Co2Emission origin="dat">180.0</ns1:Co2Emission>
                     <ns1:TechInfoWltp/>
                  </ns1:TechInfo>
                  <ns1:Equipment>
                     <ns1:Color origin="dat">Weiß</ns1:Color>
                     <ns1:SeriesEquipment>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>303</ns1:DatEquipmentId>
                           <ns1:Description>Ausstattungs-Niveau E1 (siehe Typenschild B-Säule)</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>15006</ns1:DatEquipmentId>
                           <ns1:Description>Außenspiegel mech. von innen verstellbar, beide</ns1:Description>
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
                           <ns1:DatEquipmentId>20006</ns1:DatEquipmentId>
                           <ns1:Description>Schutzzierleisten seitlich</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>21300</ns1:DatEquipmentId>
                           <ns1:Description>Stoßfänger Wagenfarbe</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>22000</ns1:DatEquipmentId>
                           <ns1:Description>Verglasung getönt</ns1:Description>
                           <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
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
                           <ns1:DatEquipmentId>23509</ns1:DatEquipmentId>
                           <ns1:Description>1-K-Kleber für Scheiben</ns1:Description>
                           <ns1:EquipmentType>glass</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>24405</ns1:DatEquipmentId>
                           <ns1:Description>Radiovorbereitung</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
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
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>26909</ns1:DatEquipmentId>
                           <ns1:Description>Airbag Beifahrerseite abschaltbar</ns1:Description>
                           <ns1:EquipmentGroup>AIR2</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27024</ns1:DatEquipmentId>
                           <ns1:Description>Mittelkonsole mit Getränkehalter vorn und hinten</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>27577</ns1:DatEquipmentId>
                           <ns1:Description>Gepäckraumabdeckung</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>33615</ns1:DatEquipmentId>
                           <ns1:Description>Rücksitzbank (2.Reihe) geteilt, klappbar (1/3-2/3)</ns1:Description>
                           <ns1:EquipmentGroup>SITH</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>37004</ns1:DatEquipmentId>
                           <ns1:Description>Sicherheitsgurte vorn höhenverstellbar</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>38104</ns1:DatEquipmentId>
                           <ns1:Description>Wegfahrsperre mit Transponder</ns1:Description>
                           <ns1:EquipmentGroup>WFS</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>39308</ns1:DatEquipmentId>
                           <ns1:Description>Isofix-Aufnahmen für Kindersitz an Rücksitz</ns1:Description>
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
                           <ns1:DatEquipmentId>40307</ns1:DatEquipmentId>
                           <ns1:Description>Elektr. Bremskraftverteilung</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>40405</ns1:DatEquipmentId>
                           <ns1:Description>Bremsscheiben innenbelüftet</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>43709</ns1:DatEquipmentId>
                           <ns1:Description>Stahlfelgen 6x15</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>69800</ns1:DatEquipmentId>
                           <ns1:Description>Servolenkung</ns1:Description>
                           <ns1:EquipmentGroup>SL</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>82503</ns1:DatEquipmentId>
                           <ns1:Description>Motor 1,4 Ltr. - 55 kW KAT</ns1:Description>
                           <ns1:EquipmentType>engine</ns1:EquipmentType>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                           <ns1:Description>Karosserie: 5-türig</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>75005</ns1:DatEquipmentId>
                           <ns1:Description>Getriebe 5-Gang</ns1:Description>
                           <ns1:EquipmentGroup>SG5</ns1:EquipmentGroup>
                           <ns1:GearBoxType>manual</ns1:GearBoxType>
                           <ns1:NrOfGears>5</ns1:NrOfGears>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                     </ns1:SeriesEquipment>
                     <ns1:DeselectedSeriesEquipment>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35300</ns1:DatEquipmentId>
                           <ns1:Description>Zentralverriegelung</ns1:Description>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>57200</ns1:DatEquipmentId>
                           <ns1:Description>Reifen 185/65 R15 ..T</ns1:Description>
                        </ns1:EquipmentPosition>
                     </ns1:DeselectedSeriesEquipment>
                     <ns1:SpecialEquipment>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>57202</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Reifen 185/65 R15 ..T (M+S)</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           <ns1:ContainedEquipmentPositions>
                              <ns1:EquipmentPosition>
                                 <ns1:DatEquipmentId>68800</ns1:DatEquipmentId>
                                 <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                 <ns1:Description>Winterreifen/M+S</ns1:Description>
                                 <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                              </ns1:EquipmentPosition>
                           </ns1:ContainedEquipmentPositions>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35301</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Zentralverriegelung mit Fernbedienung</ns1:Description>
                           <ns1:EquipmentGroup>ZV</ns1:EquipmentGroup>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>68800</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Winterreifen/M+S</ns1:Description>
                           <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                     </ns1:SpecialEquipment>
                     <ns1:AdditionalEquipment>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>98206</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Spoiler vorn</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>98207</ns1:DatEquipmentId>
                           <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                           <ns1:Description>Spoiler hinten</ns1:Description>
                           <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                        </ns1:EquipmentPosition>
                     </ns1:AdditionalEquipment>
                     <ns1:DenialCaseEquipment>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>35300</ns1:DatEquipmentId>
                           <ns1:Description>35300, weil 35301 vorhanden</ns1:Description>
                           <ns1:DatEquipmentIdReason>35301</ns1:DatEquipmentIdReason>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>57200</ns1:DatEquipmentId>
                           <ns1:Description>57200, weil 57202 vorhanden</ns1:Description>
                           <ns1:DatEquipmentIdReason>57202</ns1:DatEquipmentIdReason>
                        </ns1:EquipmentPosition>
                     </ns1:DenialCaseEquipment>
                  </ns1:Equipment>
                  <ns1:Tires>
                     <ns1:Axles/>
                  </ns1:Tires>
                  <ns1:DATECodeEquipment>
                     <ns1:EquipmentPosition>
                        <ns1:DatEquipmentId>82503</ns1:DatEquipmentId>
                        <ns1:Description>Motor 1,4 Ltr. - 55 kW KAT</ns1:Description>
                        <ns1:EquipmentClass>1</ns1:EquipmentClass>
                     </ns1:EquipmentPosition>
                     <ns1:EquipmentPosition>
                        <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                        <ns1:Description>Karosserie: 5-türig</ns1:Description>
                        <ns1:EquipmentClass>2</ns1:EquipmentClass>
                     </ns1:EquipmentPosition>
                     <ns1:EquipmentPosition>
                        <ns1:DatEquipmentId>75005</ns1:DatEquipmentId>
                        <ns1:Description>Getriebe 5-Gang</ns1:Description>
                        <ns1:EquipmentClass>11</ns1:EquipmentClass>
                     </ns1:EquipmentPosition>
                  </ns1:DATECodeEquipment>
               </ns1:Vehicle>
               <ns1:VAT>
                  <ns1:VatAtCalculationTime>19</ns1:VatAtCalculationTime>
               </ns1:VAT>
               <ns1:TradingData>
                  <ns1:Owner>
                     <ns1:CompanyName/>
                     <ns1:NameLong/>
                     <ns1:UsageFlag>2</ns1:UsageFlag>
                  </ns1:Owner>
                  <ns1:ClientContactAddresses>
                     <ns1:ClientContactAddress>
                        <ns1:Title>titleCompany</ns1:Title>
                        <ns1:CompanyName>Firma</ns1:CompanyName>
                        <ns1:NameLong>Name2</ns1:NameLong>
                        <ns1:Country>DE</ns1:Country>
                        <ns1:TaxNumber>123123</ns1:TaxNumber>
                        <ns1:CustomerNumber>999999</ns1:CustomerNumber>
                        <ns1:CustomerType>999999</ns1:CustomerType>
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
                     <ns1:DatECode>011940020020001</ns1:DatECode>
                     <ns1:ConstructionTime>4567</ns1:ConstructionTime>
                     <ns1:VehicleTypeName origin="dat">Pkw, SUV, Kleintransporter</ns1:VehicleTypeName>
                     <ns1:VehicleTypeNameN origin="dat">Pkw, SUV, Kleintransporter</ns1:VehicleTypeNameN>
                     <ns1:ManufacturerName origin="dat">Dacia</ns1:ManufacturerName>
                     <ns1:BaseModelName origin="dat">Logan MCV Kombi (12.2006->)</ns1:BaseModelName>
                     <ns1:SubModelName origin="dat">Ambiance</ns1:SubModelName>
                     <ns1:VehicleType>1</ns1:VehicleType>
                     <ns1:Manufacturer>194</ns1:Manufacturer>
                     <ns1:BaseModel>2</ns1:BaseModel>
                     <ns1:SubModel>2</ns1:SubModel>
                     <ns1:Country>DE</ns1:Country>
                     <ns1:SubModelVariant>1</ns1:SubModelVariant>
                     <ns1:RegistrationData/>
                     <ns1:Engine>
                        <ns1:EnginePowerKw origin="dat">55</ns1:EnginePowerKw>
                        <ns1:EnginePowerHp origin="dat">74</ns1:EnginePowerHp>
                        <ns1:Cylinders origin="dat">4</ns1:Cylinders>
                        <ns1:Capacity origin="dat">1390</ns1:Capacity>
                        <ns1:Consumption>7.6</ns1:Consumption>
                        <ns1:Co2Emission>180.0</ns1:Co2Emission>
                     </ns1:Engine>
                     <ns1:TechInfo>
                        <ns1:FillingQuantities>
                           <ns1:Fluid code="JH3 5/1" desc="Schalttransaxle" type="3">
                              <ns1:Capacity desc="Füllmenge (gesamt)" min="2.80" unit="Liter"/>
                              <ns1:Recommendation>
                                 <ns1:Usage type="0">Normal</ns1:Usage>
                                 <ns1:Product>TITAN SINTOFLUID SAE 75W-80</ns1:Product>
                              </ns1:Recommendation>
                           </ns1:Fluid>
                           <ns1:Fluid desc="Kühlsystem" type="8">
                              <ns1:Capacity desc="Füllmenge (gesamt)" min="4.50" unit="Liter"/>
                              <ns1:Recommendation>
                                 <ns1:Usage type="0">Normal</ns1:Usage>
                                 <ns1:Interval type="1">Wechseln 90000 km/ 48 Monate</ns1:Interval>
                                 <ns1:Interval type="2">Prüfen 15000 km/ 12 Monate</ns1:Interval>
                                 <ns1:Product>MAINTAIN FRICOFIN LL</ns1:Product>
                              </ns1:Recommendation>
                           </ns1:Fluid>
                           <ns1:Fluid code="JH1 5/1" desc="Schalttransaxle" type="3">
                              <ns1:Capacity desc="Füllmenge (gesamt)" min="2.80" unit="Liter"/>
                              <ns1:Recommendation>
                                 <ns1:Usage type="0">Normal</ns1:Usage>
                                 <ns1:Product>TITAN SINTOFLUID SAE 75W-80</ns1:Product>
                              </ns1:Recommendation>
                           </ns1:Fluid>
                           <ns1:Fluid desc="Hydraulisches Brems-/Kupplungssystem" type="4">
                              <ns1:Capacity desc="Füllmenge (gesamt)" min="0.50" unit="Liter"/>
                              <ns1:Recommendation>
                                 <ns1:Usage type="0">Normal</ns1:Usage>
                                 <ns1:Interval type="2">Prüfen 15000 km/ 12 Monate</ns1:Interval>
                                 <ns1:Interval type="1">Wechseln 90000 km/ 48 Monate</ns1:Interval>
                                 <ns1:Product>MAINTAIN DOT 5.1</ns1:Product>
                                 <ns1:Product>MAINTAIN DOT 4</ns1:Product>
                              </ns1:Recommendation>
                           </ns1:Fluid>
                           <ns1:Fluid code="K7J" desc="Motor" type="1">
                              <ns1:Capacity desc="Filterkapazität" min="0.10" unit="Liter"/>
                              <ns1:Recommendation>
                                 <ns1:Usage type="3449">Schwere Einsatzbedingungen</ns1:Usage>
                                 <ns1:Interval type="1">Wechseln 15000 km/ 6 Monate</ns1:Interval>
                                 <ns1:Product>TITAN Supersyn SAE 5W-30</ns1:Product>
                                 <ns1:Product>TITAN Supersyn SAE 5W-40</ns1:Product>
                                 <ns1:Product>TITAN Supersyn LONGLIFE SAE 0W-40</ns1:Product>
                                 <ns1:Product>TITAN SYN MC SAE 10W-40</ns1:Product>
                                 <ns1:Product>TITAN Supersyn F Eco-DT SAE 5W-30</ns1:Product>
                                 <ns1:Product>TITAN Supersyn LONGLIFE SAE 0W-30</ns1:Product>
                                 <ns1:Product>TITAN GT1 PRO 229.6 SAE 5W-30 (XTL-Technology)</ns1:Product>
                                 <ns1:Product>TITAN Supersyn FE SAE 0W-30</ns1:Product>
                                 <ns1:Product>TITAN Supersyn LONGLIFE SAE 5W-40</ns1:Product>
                                 <ns1:Product>TITAN UNIMAX ULTRA MC SAE 10W-40</ns1:Product>
                              </ns1:Recommendation>
                           </ns1:Fluid>
                           <ns1:Fluid code="K7J" desc="Motor" type="1">
                              <ns1:Capacity desc="Filterkapazität" min="0.10" unit="Liter"/>
                              <ns1:Recommendation>
                                 <ns1:Usage type="0">Normal</ns1:Usage>
                                 <ns1:Interval type="2">Prüfen 15000 km/ 12 Monate</ns1:Interval>
                                 <ns1:Interval type="1">Wechseln 30000 km/ 24 Monate</ns1:Interval>
                                 <ns1:Product>TITAN Supersyn SAE 5W-30</ns1:Product>
                                 <ns1:Product>TITAN GT1 PRO 229.6 SAE 5W-30 (XTL-Technology)</ns1:Product>
                                 <ns1:Product>TITAN SYN MC SAE 10W-40</ns1:Product>
                                 <ns1:Product>TITAN Supersyn LONGLIFE SAE 5W-40</ns1:Product>
                                 <ns1:Product>TITAN Supersyn F Eco-DT SAE 5W-30</ns1:Product>
                                 <ns1:Product>TITAN Supersyn LONGLIFE SAE 0W-40</ns1:Product>
                                 <ns1:Product>TITAN UNIMAX ULTRA MC SAE 10W-40</ns1:Product>
                                 <ns1:Product>TITAN Supersyn LONGLIFE SAE 0W-30</ns1:Product>
                                 <ns1:Product>TITAN Supersyn SAE 5W-40</ns1:Product>
                                 <ns1:Product>TITAN Supersyn FE SAE 0W-30</ns1:Product>
                              </ns1:Recommendation>
                           </ns1:Fluid>
                           <ns1:Fluid code="JR5 5/1" desc="Schalttransaxle" type="3">
                              <ns1:Capacity desc="Füllmenge (gesamt)" min="2.50" unit="Liter"/>
                              <ns1:Recommendation>
                                 <ns1:Usage type="0">Normal</ns1:Usage>
                                 <ns1:Product>TITAN SINTOFLUID SAE 75W-80</ns1:Product>
                              </ns1:Recommendation>
                           </ns1:Fluid>
                        </ns1:FillingQuantities>
                        <ns1:PowerHp origin="dat">75</ns1:PowerHp>
                        <ns1:PowerKw origin="dat">55.0</ns1:PowerKw>
                        <ns1:Capacity origin="dat">1390</ns1:Capacity>
                        <ns1:Cylinder origin="dat">4</ns1:Cylinder>
                        <ns1:CylinderArrangement origin="dat">R</ns1:CylinderArrangement>
                        <ns1:GearboxType>manual</ns1:GearboxType>
                        <ns1:ConsumptionInTown origin="dat">10.0</ns1:ConsumptionInTown>
                        <ns1:ConsumptionOutOfTown origin="dat">6.2</ns1:ConsumptionOutOfTown>
                        <ns1:Consumption origin="dat">7.6</ns1:Consumption>
                        <ns1:Co2Emission origin="dat">180.0</ns1:Co2Emission>
                        <ns1:TechInfoWltp/>
                     </ns1:TechInfo>
                     <ns1:Equipment>
                        <ns1:Color origin="dat">Weiß</ns1:Color>
                        <ns1:SeriesEquipment>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>303</ns1:DatEquipmentId>
                              <ns1:Description>Ausstattungs-Niveau E1 (siehe Typenschild B-Säule)</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>15006</ns1:DatEquipmentId>
                              <ns1:Description>Außenspiegel mech. von innen verstellbar, beide</ns1:Description>
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
                              <ns1:DatEquipmentId>20006</ns1:DatEquipmentId>
                              <ns1:Description>Schutzzierleisten seitlich</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>21300</ns1:DatEquipmentId>
                              <ns1:Description>Stoßfänger Wagenfarbe</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>22000</ns1:DatEquipmentId>
                              <ns1:Description>Verglasung getönt</ns1:Description>
                              <ns1:EquipmentGroup>WDG</ns1:EquipmentGroup>
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
                              <ns1:DatEquipmentId>23509</ns1:DatEquipmentId>
                              <ns1:Description>1-K-Kleber für Scheiben</ns1:Description>
                              <ns1:EquipmentType>glass</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>24405</ns1:DatEquipmentId>
                              <ns1:Description>Radiovorbereitung</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
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
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>26909</ns1:DatEquipmentId>
                              <ns1:Description>Airbag Beifahrerseite abschaltbar</ns1:Description>
                              <ns1:EquipmentGroup>AIR2</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27024</ns1:DatEquipmentId>
                              <ns1:Description>Mittelkonsole mit Getränkehalter vorn und hinten</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>27577</ns1:DatEquipmentId>
                              <ns1:Description>Gepäckraumabdeckung</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>33615</ns1:DatEquipmentId>
                              <ns1:Description>Rücksitzbank (2.Reihe) geteilt, klappbar (1/3-2/3)</ns1:Description>
                              <ns1:EquipmentGroup>SITH</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>37004</ns1:DatEquipmentId>
                              <ns1:Description>Sicherheitsgurte vorn höhenverstellbar</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>38104</ns1:DatEquipmentId>
                              <ns1:Description>Wegfahrsperre mit Transponder</ns1:Description>
                              <ns1:EquipmentGroup>WFS</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>39308</ns1:DatEquipmentId>
                              <ns1:Description>Isofix-Aufnahmen für Kindersitz an Rücksitz</ns1:Description>
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
                              <ns1:DatEquipmentId>40307</ns1:DatEquipmentId>
                              <ns1:Description>Elektr. Bremskraftverteilung</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>40405</ns1:DatEquipmentId>
                              <ns1:Description>Bremsscheiben innenbelüftet</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>43709</ns1:DatEquipmentId>
                              <ns1:Description>Stahlfelgen 6x15</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>69800</ns1:DatEquipmentId>
                              <ns1:Description>Servolenkung</ns1:Description>
                              <ns1:EquipmentGroup>SL</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>82503</ns1:DatEquipmentId>
                              <ns1:Description>Motor 1,4 Ltr. - 55 kW KAT</ns1:Description>
                              <ns1:EquipmentType>engine</ns1:EquipmentType>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                              <ns1:Description>Karosserie: 5-türig</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>75005</ns1:DatEquipmentId>
                              <ns1:Description>Getriebe 5-Gang</ns1:Description>
                              <ns1:EquipmentGroup>SG5</ns1:EquipmentGroup>
                              <ns1:GearBoxType>manual</ns1:GearBoxType>
                              <ns1:NrOfGears>5</ns1:NrOfGears>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                        </ns1:SeriesEquipment>
                        <ns1:DeselectedSeriesEquipment>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>35300</ns1:DatEquipmentId>
                              <ns1:Description>Zentralverriegelung</ns1:Description>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>57200</ns1:DatEquipmentId>
                              <ns1:Description>Reifen 185/65 R15 ..T</ns1:Description>
                           </ns1:EquipmentPosition>
                        </ns1:DeselectedSeriesEquipment>
                        <ns1:SpecialEquipment>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>57202</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Reifen 185/65 R15 ..T (M+S)</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                              <ns1:ContainedEquipmentPositions>
                                 <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>68800</ns1:DatEquipmentId>
                                    <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                                    <ns1:Description>Winterreifen/M+S</ns1:Description>
                                    <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                                 </ns1:EquipmentPosition>
                              </ns1:ContainedEquipmentPositions>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>35301</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Zentralverriegelung mit Fernbedienung</ns1:Description>
                              <ns1:EquipmentGroup>ZV</ns1:EquipmentGroup>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>68800</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Winterreifen/M+S</ns1:Description>
                              <ns1:AddedByLogikCheck>true</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                        </ns1:SpecialEquipment>
                        <ns1:AdditionalEquipment>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>98206</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Spoiler vorn</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>98207</ns1:DatEquipmentId>
                              <ns1:ValuationControlType>no valuation</ns1:ValuationControlType>
                              <ns1:Description>Spoiler hinten</ns1:Description>
                              <ns1:AddedByLogikCheck>false</ns1:AddedByLogikCheck>
                           </ns1:EquipmentPosition>
                        </ns1:AdditionalEquipment>
                        <ns1:DenialCaseEquipment>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>35300</ns1:DatEquipmentId>
                              <ns1:Description>35300, weil 35301 vorhanden</ns1:Description>
                              <ns1:DatEquipmentIdReason>35301</ns1:DatEquipmentIdReason>
                           </ns1:EquipmentPosition>
                           <ns1:EquipmentPosition>
                              <ns1:DatEquipmentId>57200</ns1:DatEquipmentId>
                              <ns1:Description>57200, weil 57202 vorhanden</ns1:Description>
                              <ns1:DatEquipmentIdReason>57202</ns1:DatEquipmentIdReason>
                           </ns1:EquipmentPosition>
                        </ns1:DenialCaseEquipment>
                     </ns1:Equipment>
                     <ns1:Tires>
                        <ns1:Axles/>
                     </ns1:Tires>
                     <ns1:DATECodeEquipment>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>82503</ns1:DatEquipmentId>
                           <ns1:Description>Motor 1,4 Ltr. - 55 kW KAT</ns1:Description>
                           <ns1:EquipmentClass>1</ns1:EquipmentClass>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                           <ns1:Description>Karosserie: 5-türig</ns1:Description>
                           <ns1:EquipmentClass>2</ns1:EquipmentClass>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>75005</ns1:DatEquipmentId>
                           <ns1:Description>Getriebe 5-Gang</ns1:Description>
                           <ns1:EquipmentClass>11</ns1:EquipmentClass>
                        </ns1:EquipmentPosition>
                     </ns1:DATECodeEquipment>
                  </ns1:Vehicle>
                  <ns1:RepairParameters>
                     <ns1:PhantomCalculation>false</ns1:PhantomCalculation>
                     <ns1:LacquerType>Metallic (2-Schicht)</ns1:LacquerType>
                     <ns1:LacquerTypeLayers>2</ns1:LacquerTypeLayers>
                     <ns1:TimeUnitsOfManufacturer>false</ns1:TimeUnitsOfManufacturer>
                     <ns1:WithDomusCalculation>false</ns1:WithDomusCalculation>
                     <ns1:DMSCalculation>false</ns1:DMSCalculation>
                  </ns1:RepairParameters>
                  <ns1:ProcedureRelatedParameters>
                     <ns1:ProcedureRelatedParameter attribute="biwOptimizationMode" factor="CalculationFactor" type="BiwOptimizationMode">AUTOMATIC</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="selectedLacquerMethod" factor="CalculationFactor" type="LacquerMethod">EURO_LACQUER</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="crossSeries" factor="CalculationFactor" type="CrossSeriesState">NO</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="withoutValuesOfAdditionallyRequiredPositions" factor="CalculationFactor" type="Boolean">false</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnit" factor="CalculationFactor" type="TimeUnitSystem">HOUR</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="CalculationFactor" type="Integer">1</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="dataCurrency" factor="CalculationFactor" type="String">EUR</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="smallSparePartCalculationModel" factor="SparePartFactor" type="SmallPartsCalculationModel">PERCENT_OF_PARTS</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="priceSource" factor="SparePartFactor" type="PriceSource">DAT</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="smallSparePartPercentOfPart" factor="SparePartFactor" type="Double">2.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="dentWage" factor="LabourCostFactor" mode="PER_HOUR" type="Price">25.0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="mechanicWage1" factor="LabourCostFactor" mode="PER_HOUR" type="Price">145.5</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="electricWage1" factor="LabourCostFactor" mode="PER_HOUR" type="Price">132.1</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnit" factor="LabourCostFactor" type="TimeUnitSystem">HOUR</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="LabourCostFactor" type="Integer">1</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="bodyWage1" factor="LabourCostFactor" mode="PER_HOUR" type="Price">136.6</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="colorName" factor="EuroLacquerFactor" type="String">Weiß</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="materialPriceCategoryName" factor="EuroLacquerFactor" type="String">200</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="materialMode" factor="EuroLacquerFactor" type="LacquerMaterialMode">LACQUER_METHOD</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="type" description="Metallic (2-Schicht)" factor="EuroLacquerFactor" type="String">12</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wage" factor="EuroLacquerFactor" mode="PER_HOUR" type="Price">156.51</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="color2ndCode" factor="EuroLacquerFactor" type="String">1</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="typeSaved" factor="EuroLacquerFactor" type="Boolean">false</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="colorType" factor="EuroLacquerFactor" type="String">1</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wageMode" factor="EuroLacquerFactor" type="LacquerWageMode">PER_TIME</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wageInclMaterialMode" factor="EuroLacquerFactor" type="LacquerWageMode">PER_TIME</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="calculationType" factor="EuroLacquerFactor" type="LacquerCalculationMode">WAGE_MATERIAL_SEPARATELY</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="color2ndName" factor="EuroLacquerFactor" type="String">0</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnit" factor="EuroLacquerFactor" type="TimeUnitSystem">HOUR</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="EuroLacquerFactor" type="Integer">1</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="materialMode" factor="ManufacturerLacquerFactor" type="LacquerMaterialMode">LACQUER_METHOD</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="typeSaved" factor="ManufacturerLacquerFactor" type="Boolean">false</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wageMode" factor="ManufacturerLacquerFactor" type="LacquerWageMode">PER_TIME</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="wageInclMaterialMode" factor="ManufacturerLacquerFactor" type="LacquerWageMode">PER_TIME</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="calculationType" factor="ManufacturerLacquerFactor" type="LacquerCalculationMode">WAGE_MATERIAL_SEPARATELY</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnit" factor="ManufacturerLacquerFactor" type="TimeUnitSystem">HOUR</ns1:ProcedureRelatedParameter>
                     <ns1:ProcedureRelatedParameter attribute="timeUnitsPerHour" factor="ManufacturerLacquerFactor" type="Integer">1</ns1:ProcedureRelatedParameter>
                  </ns1:ProcedureRelatedParameters>
                  <ns1:RepairPositions>
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>44210</ns1:DATProcessId>
                        <ns1:RepairType>replace</ns1:RepairType>
                        <ns1:Description>Motorhaube</ns1:Description>
                        <ns1:DescriptionId>76254</ns1:DescriptionId>
                        <ns1:IsManualDescription>false</ns1:IsManualDescription>
                        <ns1:ConstructionGroupId>1</ns1:ConstructionGroupId>
                        <ns1:ConstructionGroup>VORDERWAGEN AUSSEN</ns1:ConstructionGroup>
                        <ns1:ConstructionGroupPolygon>27</ns1:ConstructionGroupPolygon>
                        <ns1:PositionEntryType>graphical</ns1:PositionEntryType>
                        <ns1:IsRepairExtension>false</ns1:IsRepairExtension>
                        <ns1:PreDamage>false</ns1:PreDamage>
                     </ns1:RepairPosition>
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>43712</ns1:DATProcessId>
                        <ns1:RepairType>replace</ns1:RepairType>
                        <ns1:Description>Kotflügel</ns1:Description>
                        <ns1:DescriptionId>76406</ns1:DescriptionId>
                        <ns1:IsManualDescription>false</ns1:IsManualDescription>
                        <ns1:ConstructionGroupId>1</ns1:ConstructionGroupId>
                        <ns1:ConstructionGroup>VORDERWAGEN AUSSEN</ns1:ConstructionGroup>
                        <ns1:ConstructionGroupPolygon>26</ns1:ConstructionGroupPolygon>
                        <ns1:PositionEntryType>graphical</ns1:PositionEntryType>
                        <ns1:IsRepairExtension>false</ns1:IsRepairExtension>
                        <ns1:PreDamage>false</ns1:PreDamage>
                     </ns1:RepairPosition>
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>94030</ns1:DATProcessId>
                        <ns1:RepairType>replace</ns1:RepairType>
                        <ns1:IsManualDescription>false</ns1:IsManualDescription>
                        <ns1:PositionEntryType>maintenance</ns1:PositionEntryType>
                        <ns1:IsRepairExtension>false</ns1:IsRepairExtension>
                        <ns1:OverhaulLocation>front</ns1:OverhaulLocation>
                        <ns1:PreDamage>false</ns1:PreDamage>
                     </ns1:RepairPosition>
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>81715</ns1:DATProcessId>
                        <ns1:RepairType>replace</ns1:RepairType>
                        <ns1:IsManualDescription>false</ns1:IsManualDescription>
                        <ns1:PositionEntryType>maintenance</ns1:PositionEntryType>
                        <ns1:IsRepairExtension>false</ns1:IsRepairExtension>
                        <ns1:OverhaulLocation>top</ns1:OverhaulLocation>
                        <ns1:PreDamage>false</ns1:PreDamage>
                     </ns1:RepairPosition>
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>81715</ns1:DATProcessId>
                        <ns1:RepairType>replace</ns1:RepairType>
                        <ns1:IsManualDescription>false</ns1:IsManualDescription>
                        <ns1:PositionEntryType>maintenance</ns1:PositionEntryType>
                        <ns1:IsRepairExtension>false</ns1:IsRepairExtension>
                        <ns1:OverhaulLocation>back</ns1:OverhaulLocation>
                        <ns1:PreDamage>false</ns1:PreDamage>
                     </ns1:RepairPosition>
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>81691</ns1:DATProcessId>
                        <ns1:RepairType>replace</ns1:RepairType>
                        <ns1:Description>Zahnriemen</ns1:Description>
                        <ns1:DescriptionId>78634</ns1:DescriptionId>
                        <ns1:IsManualDescription>false</ns1:IsManualDescription>
                        <ns1:ConstructionGroupId>21</ns1:ConstructionGroupId>
                        <ns1:ConstructionGroup>MOTOR 1,4 / 1,6 LTR.</ns1:ConstructionGroup>
                        <ns1:ConstructionGroupPolygon>38</ns1:ConstructionGroupPolygon>
                        <ns1:PositionEntryType>graphical</ns1:PositionEntryType>
                        <ns1:IsRepairExtension>false</ns1:IsRepairExtension>
                        <ns1:PreDamage>false</ns1:PreDamage>
                     </ns1:RepairPosition>
                     <ns1:RepairPosition>
                        <ns1:DATProcessId>81200</ns1:DATProcessId>
                        <ns1:RepairType>replace</ns1:RepairType>
                        <ns1:Description>Ölfilter</ns1:Description>
                        <ns1:DescriptionId>276517</ns1:DescriptionId>
                        <ns1:IsManualDescription>false</ns1:IsManualDescription>
                        <ns1:ConstructionGroupId>21</ns1:ConstructionGroupId>
                        <ns1:ConstructionGroup>MOTOR 1,4 / 1,6 LTR.</ns1:ConstructionGroup>
                        <ns1:ConstructionGroupPolygon>16</ns1:ConstructionGroupPolygon>
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
                           <ns1:PartNumber>6001549973</ns1:PartNumber>
                           <ns1:DATPartNumber>6001549973</ns1:DATPartNumber>
                           <ns1:Description>KOTFLUEGEL V.R.</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>130.86</ns1:ValuePerUnit>
                           <ns1:ValueTotal>130.86</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>130.86</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>44210</ns1:DATProcessId>
                           <ns1:PartNumber>6001546685</ns1:PartNumber>
                           <ns1:DATPartNumber>6001546685</ns1:DATPartNumber>
                           <ns1:Description>MOTORHAUBE</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>278.08</ns1:ValuePerUnit>
                           <ns1:ValueTotal>278.08</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>278.08</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>81200</ns1:DATProcessId>
                           <ns1:PartNumber>7711945897</ns1:PartNumber>
                           <ns1:DATPartNumber>7711945897</ns1:DATPartNumber>
                           <ns1:Description>OELFILTER</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>13.16</ns1:ValuePerUnit>
                           <ns1:ValueTotal>13.16</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>13.16</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                     </ns1:MaterialPositions>
                     <ns1:MaterialPositionsMaintenance>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>81715</ns1:DATProcessId>
                           <ns1:PartNumber>7701477024</ns1:PartNumber>
                           <ns1:DATPartNumber>7701477024</ns1:DATPartNumber>
                           <ns1:Description>REP.-SATZ ZAHNRIEMEN</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>230.00</ns1:ValuePerUnit>
                           <ns1:ValueTotal>230.00</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>230.00</ns1:ValueTotalCorrected>
                           <ns1:IsRepairSet>false</ns1:IsRepairSet>
                           <ns1:IsSpecific>false</ns1:IsSpecific>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:PartOrigin>OE</ns1:PartOrigin>
                           <ns1:spoTmpManualPartNumber>false</ns1:spoTmpManualPartNumber>
                        </ns1:MaterialPosition>
                     </ns1:MaterialPositionsMaintenance>
                     <ns1:LabourPositions>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>43712</ns1:DATProcessId>
                           <ns1:LabourPositionKind>1</ns1:LabourPositionKind>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:LabourPosId>4196</ns1:LabourPosId>
                           <ns1:Description>KOTFLUEGEL V.R. A+E/ERS.</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>1.10</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>150.26</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>150.26</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>4196</ns1:WorkNumber>
                           <ns1:SparePartNumber>6001549973</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>45610</ns1:DATProcessId>
                           <ns1:LabourPositionKind>4</ns1:LabourPositionKind>
                           <ns1:RepairType>adjust</ns1:RepairType>
                           <ns1:LabourPosId>8072</ns1:LabourPosId>
                           <ns1:Description>SCHEINWERFER V. EINSTELLEN
(INKL. NEBELSCHEINWERFER)</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>0.20</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>27.32</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>27.32</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>true</ns1:hasRequiredByPosition>
                           <ns1:RequiredByPosition>
                              <ns1:DATProcessId>43712</ns1:DATProcessId>
                              <ns1:RepairType>replace</ns1:RepairType>
                           </ns1:RequiredByPosition>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>8072</ns1:WorkNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>44210</ns1:DATProcessId>
                           <ns1:LabourPositionKind>1</ns1:LabourPositionKind>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:LabourPosId>ADT#A4 421001</ns1:LabourPosId>
                           <ns1:Description>MOTORHAUBE A+E/ERS.</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>0.10</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>13.66</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>13.66</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>ADT#A4 421001</ns1:WorkNumber>
                           <ns1:SparePartNumber>6001546685</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>44210</ns1:DATProcessId>
                           <ns1:LabourPositionKind>4</ns1:LabourPositionKind>
                           <ns1:RepairType>dis- and mounting</ns1:RepairType>
                           <ns1:LabourPosId>A15T</ns1:LabourPosId>
                           <ns1:Description>MOTORHAUBE A+E</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>0.40</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>54.64</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>54.64</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>true</ns1:hasRequiredByPosition>
                           <ns1:RequiredByPosition>
                              <ns1:DATProcessId>44210</ns1:DATProcessId>
                              <ns1:RepairType>replace</ns1:RepairType>
                           </ns1:RequiredByPosition>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>A15T</ns1:WorkNumber>
                           <ns1:SparePartNumber>6001546685</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>44210</ns1:DATProcessId>
                           <ns1:LabourPositionKind>4</ns1:LabourPositionKind>
                           <ns1:RepairType>body cavity protection</ns1:RepairType>
                           <ns1:LabourPosId>9353</ns1:LabourPosId>
                           <ns1:Description>MOTORHAUBE HOHLR.-KONSERVIEREN</ns1:Description>
                           <ns1:WageType>car body</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>2</ns1:WageLevel>
                           <ns1:Duration>0.20</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>27.32</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>27.32</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>true</ns1:hasRequiredByPosition>
                           <ns1:RequiredByPosition>
                              <ns1:DATProcessId>44210</ns1:DATProcessId>
                              <ns1:RepairType>replace</ns1:RepairType>
                           </ns1:RequiredByPosition>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>9353</ns1:WorkNumber>
                           <ns1:SparePartNumber>6001546685</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>81200</ns1:DATProcessId>
                           <ns1:LabourPositionKind>1</ns1:LabourPositionKind>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:LabourPosId>0068</ns1:LabourPosId>
                           <ns1:Description>OELFILTER A+E/ERS.</ns1:Description>
                           <ns1:WageType>mechanic</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>0.10</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>14.55</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>14.55</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>0068</ns1:WorkNumber>
                           <ns1:SparePartNumber>7711945897</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                     </ns1:LabourPositions>
                     <ns1:LabourPositionsMaintenance>
                        <ns1:LabourPosition>
                           <ns1:DATProcessId>81715</ns1:DATProcessId>
                           <ns1:LabourPositionKind>1</ns1:LabourPositionKind>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:LabourPosId>1550</ns1:LabourPosId>
                           <ns1:Description>ZAHNRIEMEN MOTORSTEUERUNG MIT SPANN-/UMLENKROLLE ERS.</ns1:Description>
                           <ns1:WageType>mechanic</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>2.10</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>305.55</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>305.55</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>1550</ns1:WorkNumber>
                           <ns1:SparePartNumber>7701477024</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                     </ns1:LabourPositionsMaintenance>
                     <ns1:LacquerPositions>
                        <ns1:LacquerPosition>
                           <ns1:LabourPosId>ARBEITSAUFWAND</ns1:LabourPosId>
                           <ns1:Description>VORBEREITUNG ZUR LACKIERUNG</ns1:Description>
                           <ns1:Duration>1.70</ns1:Duration>
                           <ns1:ManualDuration>false</ns1:ManualDuration>
                           <ns1:ValueTotal>266.07</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>266.07</ns1:ValueTotalCorrected>
                           <ns1:WageLevel1>266.07</ns1:WageLevel1>
                           <ns1:WorkNumber>ARBEITSAUFWAND</ns1:WorkNumber>
                           <ns1:LacquerPositionTimeState/>
                           <ns1:LacquerPositionMaterialState/>
                           <ns1:LacquerPositionPriceState/>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                        </ns1:LacquerPosition>
                        <ns1:LacquerPosition>
                           <ns1:DATProcessId>43712</ns1:DATProcessId>
                           <ns1:LabourPosId>NEUTEIL-M</ns1:LabourPosId>
                           <ns1:Description>KOTFLUEGEL V.R.</ns1:Description>
                           <ns1:Level>4</ns1:Level>
                           <ns1:LevelDescription>new</ns1:LevelDescription>
                           <ns1:Duration>1.00</ns1:Duration>
                           <ns1:ManualDuration>false</ns1:ManualDuration>
                           <ns1:Material>68.40</ns1:Material>
                           <ns1:MaterialPoints>18</ns1:MaterialPoints>
                           <ns1:ValueTotal>224.91</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>224.91</ns1:ValueTotalCorrected>
                           <ns1:WageLevel1>156.51</ns1:WageLevel1>
                           <ns1:WorkNumber>NEUTEIL-M</ns1:WorkNumber>
                           <ns1:LacquerPositionTimeState/>
                           <ns1:LacquerPositionMaterialState/>
                           <ns1:LacquerPositionPriceState/>
                           <ns1:MaterialType>2</ns1:MaterialType>
                           <ns1:SparePartNumber>6001549973</ns1:SparePartNumber>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                        </ns1:LacquerPosition>
                        <ns1:LacquerPosition>
                           <ns1:DATProcessId>44210</ns1:DATProcessId>
                           <ns1:LabourPosId>NEUTEIL-M</ns1:LabourPosId>
                           <ns1:Description>MOTORHAUBE</ns1:Description>
                           <ns1:Level>4</ns1:Level>
                           <ns1:LevelDescription>new</ns1:LevelDescription>
                           <ns1:Duration>2.00</ns1:Duration>
                           <ns1:ManualDuration>false</ns1:ManualDuration>
                           <ns1:Material>216.60</ns1:Material>
                           <ns1:MaterialPoints>57</ns1:MaterialPoints>
                           <ns1:ValueTotal>529.62</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>529.62</ns1:ValueTotalCorrected>
                           <ns1:WageLevel1>313.02</ns1:WageLevel1>
                           <ns1:WorkNumber>NEUTEIL-M</ns1:WorkNumber>
                           <ns1:LacquerPositionTimeState/>
                           <ns1:LacquerPositionMaterialState/>
                           <ns1:LacquerPositionPriceState/>
                           <ns1:MaterialType>2</ns1:MaterialType>
                           <ns1:SparePartNumber>6001546685</ns1:SparePartNumber>
                           <ns1:Extended>true</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                        </ns1:LacquerPosition>
                     </ns1:LacquerPositions>
                     <ns1:PriceDate>2023-12-01+01:00</ns1:PriceDate>
                     <ns1:RepairCalculationSummary>
                        <ns1:SparePartsCosts>
                           <ns1:AllSum>652.10</ns1:AllSum>
                           <ns1:ConsumablesSurcharge>13.04</ns1:ConsumablesSurcharge>
                           <ns1:ConsumablesSurchargePercentage>2.00</ns1:ConsumablesSurchargePercentage>
                           <ns1:TotalSum>665.14</ns1:TotalSum>
                        </ns1:SparePartsCosts>
                        <ns1:AuxiliaryCosts/>
                        <ns1:LabourCosts>
                           <ns1:AllSum>593.30</ns1:AllSum>
                           <ns1:Bodywork>
                              <ns1:Type>CAR BODY</ns1:Type>
                              <ns1:Units>2.00</ns1:Units>
                              <ns1:Price>273.20</ns1:Price>
                           </ns1:Bodywork>
                           <ns1:Electric>
                              <ns1:Type>ELECTRICS</ns1:Type>
                              <ns1:Units>0</ns1:Units>
                              <ns1:Price>0</ns1:Price>
                           </ns1:Electric>
                           <ns1:Mechanic>
                              <ns1:Type>MECHANICS</ns1:Type>
                              <ns1:Units>2.20</ns1:Units>
                              <ns1:Price>320.10</ns1:Price>
                           </ns1:Mechanic>
                           <ns1:TotalSum>593.30</ns1:TotalSum>
                           <ns1:Wages/>
                           <ns1:Works>
                              <ns1:Work>
                                 <ns1:Type>CAR BODY</ns1:Type>
                                 <ns1:WageLevel>1</ns1:WageLevel>
                                 <ns1:Units>1.80</ns1:Units>
                                 <ns1:PricePerUnit>136.60</ns1:PricePerUnit>
                                 <ns1:Price>245.88</ns1:Price>
                              </ns1:Work>
                              <ns1:Work>
                                 <ns1:Type>CAR BODY</ns1:Type>
                                 <ns1:WageLevel>2</ns1:WageLevel>
                                 <ns1:Units>0.20</ns1:Units>
                                 <ns1:PricePerUnit>136.60</ns1:PricePerUnit>
                                 <ns1:Price>27.32</ns1:Price>
                              </ns1:Work>
                              <ns1:Work>
                                 <ns1:Type>MECHANICS</ns1:Type>
                                 <ns1:WageLevel>1</ns1:WageLevel>
                                 <ns1:Units>2.20</ns1:Units>
                                 <ns1:PricePerUnit>145.50</ns1:PricePerUnit>
                                 <ns1:Price>320.10</ns1:Price>
                              </ns1:Work>
                           </ns1:Works>
                        </ns1:LabourCosts>
                        <ns1:LacquerCosts>
                           <ns1:Wage>
                              <ns1:Type>LACQUER WORK</ns1:Type>
                              <ns1:Units>4.70</ns1:Units>
                              <ns1:PricePerUnit>156.51</ns1:PricePerUnit>
                              <ns1:Price>735.60</ns1:Price>
                           </ns1:Wage>
                           <ns1:TotalWages>735.60</ns1:TotalWages>
                           <ns1:Material>
                              <ns1:Replacement>
                                 <ns1:Type>LACQUER MATERIAL REPLACEMENT</ns1:Type>
                                 <ns1:Units>75.00</ns1:Units>
                                 <ns1:PricePerUnit>3.80</ns1:PricePerUnit>
                                 <ns1:Price>285.00</ns1:Price>
                              </ns1:Replacement>
                              <ns1:LacquerConstants>
                                 <ns1:LacquerConstant>
                                    <ns1:Id>LacquerConstantMetal</ns1:Id>
                                    <ns1:Description>KONSTANTE</ns1:Description>
                                    <ns1:Price>49.70</ns1:Price>
                                    <ns1:Unit>Absolute</ns1:Unit>
                                    <ns1:ConstantType>0</ns1:ConstantType>
                                    <ns1:ValueInPositions>false</ns1:ValueInPositions>
                                    <ns1:ValueForInformation>false</ns1:ValueForInformation>
                                 </ns1:LacquerConstant>
                              </ns1:LacquerConstants>
                              <ns1:TotalSum>334.70</ns1:TotalSum>
                              <ns1:SumMaterialCorrected>334.70</ns1:SumMaterialCorrected>
                           </ns1:Material>
                           <ns1:TotalSum>1070.30</ns1:TotalSum>
                        </ns1:LacquerCosts>
                        <ns1:TotalNetCosts>2328.74</ns1:TotalNetCosts>
                        <ns1:TotalVAT>442.46</ns1:TotalVAT>
                        <ns1:TotalGrossCosts>2771.20</ns1:TotalGrossCosts>
                        <ns1:TotalNetCorrected>2328.74</ns1:TotalNetCorrected>
                        <ns1:TotalVATCorrected>442.46</ns1:TotalVATCorrected>
                        <ns1:TotalGrossCorrected>2771.20</ns1:TotalGrossCorrected>
                        <ns1:SumNet>2328.74</ns1:SumNet>
                        <ns1:SumGross>2771.20</ns1:SumGross>
                        <ns1:SumSparePartCosts>652.10</ns1:SumSparePartCosts>
                        <ns1:SumSmallSparePartCosts>13.04</ns1:SumSmallSparePartCosts>
                        <ns1:SumLabourCosts>593.30</ns1:SumLabourCosts>
                        <ns1:MetaPositions>
                           <ns1:MetaPosition key="TIME_UNIT_SYSTEM" value="STD"/>
                           <ns1:MetaPosition key="LACQUER_TIME_UNIT_SYSTEM" value="STD"/>
                           <ns1:MetaPosition key="DAT_EUROLACQUER_IN_HOURS" value="false"/>
                           <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EQUIPMENT" value="false"/>
                           <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EXTENSION" value="false"/>
                           <ns1:MetaPosition key="FLAT_PERCENTAGE_BASE" value="735.60"/>
                        </ns1:MetaPositions>
                     </ns1:RepairCalculationSummary>
                     <ns1:CalcProtocol>
                        <ns1:ProtocolHints>
                           <ns1:ProtocolHint>
                              <ns1:Identifier>H001</ns1:Identifier>
                              <ns1:Description>Serientreue Kalkulation</ns1:Description>
                           </ns1:ProtocolHint>
                        </ns1:ProtocolHints>
                        <ns1:InvalidPositionsProtocol>
                           <ns1:ProtocolEntry>
                              <ns1:DATProcessId>94030</ns1:DATProcessId>
                              <ns1:RepairType>replace</ns1:RepairType>
                              <ns1:Description/>
                              <ns1:Logic>parts</ns1:Logic>
                           </ns1:ProtocolEntry>
                           <ns1:ProtocolEntry>
                              <ns1:DATProcessId>94030</ns1:DATProcessId>
                              <ns1:RepairType>replace</ns1:RepairType>
                              <ns1:Description/>
                              <ns1:Logic>work</ns1:Logic>
                           </ns1:ProtocolEntry>
                        </ns1:InvalidPositionsProtocol>
                        <ns1:PartsOfOtherPositionProtocol>
                           <ns1:ProtocolEntryWithRemoval>
                              <ns1:DATProcessId>81691</ns1:DATProcessId>
                              <ns1:RepairType>replace</ns1:RepairType>
                              <ns1:Description>Zahnriemen</ns1:Description>
                              <ns1:ContainedInDATProcessId>81715</ns1:ContainedInDATProcessId>
                              <ns1:ContainedInRepairType>replace</ns1:ContainedInRepairType>
                              <ns1:Logic>parts</ns1:Logic>
                           </ns1:ProtocolEntryWithRemoval>
                        </ns1:PartsOfOtherPositionProtocol>
                        <ns1:ProtocolData>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biAKMDAwMDAxNzk0MyAwMDAwMCBuIAowMDAwMDMzNTc0IDAwMDAwIG4gCjAwMDAwMDAwMTUgMDAwMDAgbiAKMDAwMDAzMzcyMCAwMDAwMCBuIAowMDAwMDAyMDg2IDAwMDAwIG4gCjAwMDAwMDIxMjEgMDAwMDAgbiAKMDAwMDAxNjYxMiAwMDAwMCBuIAowMDAwMDE2ODA0IDAwMDAwIG4gCjAwMDAwMTczMTIgMDAwMDAgbiAKMDAwMDAxODA4MyAwMDAwMCBuIAowMDAwMDMyMzU1IDAwMDAwIG4gCjAwMDAwMzI1NTggMDAwMDAgbiAKMDAwMDAzMzAxOSAwMDAwMCBuIAowMDAwMDMzNzgzIDAwMDAwIG4gCjAwMDAwMzM4MzggMDAwMDAgbiAKMDAwMDAzMzg3MiAwMDAwMCBuIAowMDAwMDMzOTc3IDAwMDAwIG4gCnRyYWlsZXIKPDwvSW5mbyAxOCAwIFIvSUQgWzw0MTg4NTNlZDQ3NjRmNmMzYTE1MjI4Yzg3OTk4M2IyYT48ODQyMzU5NzcyODBiYTIzNjk1Nzc4NTA2ZmNiYWU2OGU+XS9Sb290IDE3IDAgUi9TaXplIDE5Pj4Kc3RhcnR4cmVmCjM0MTUzCiUlRU9GCg==</ns1:ProtocolData>
                     </ns1:CalcProtocol>
                  </ns1:CalcResultCommon>
                  <ns1:CalcResultMaintenance>
                     <ns1:MaterialPositions>
                        <ns1:MaterialPosition>
                           <ns1:DATProcessId>81715</ns1:DATProcessId>
                           <ns1:PartNumber>7701477024</ns1:PartNumber>
                           <ns1:DATPartNumber>7701477024</ns1:DATPartNumber>
                           <ns1:Description>REP.-SATZ ZAHNRIEMEN</ns1:Description>
                           <ns1:Amount>1</ns1:Amount>
                           <ns1:ValuePerUnit>230.00</ns1:ValuePerUnit>
                           <ns1:ValueTotal>230.00</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ManualAmount>false</ns1:ManualAmount>
                           <ns1:ManualPrice>false</ns1:ManualPrice>
                           <ns1:PriceDerived>false</ns1:PriceDerived>
                           <ns1:UsedPart>false</ns1:UsedPart>
                           <ns1:ValueTotalCorrected>230.00</ns1:ValueTotalCorrected>
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
                           <ns1:DATProcessId>81715</ns1:DATProcessId>
                           <ns1:LabourPositionKind>1</ns1:LabourPositionKind>
                           <ns1:RepairType>replace</ns1:RepairType>
                           <ns1:LabourPosId>1550</ns1:LabourPosId>
                           <ns1:Description>ZAHNRIEMEN MOTORSTEUERUNG MIT SPANN-/UMLENKROLLE ERS.</ns1:Description>
                           <ns1:WageType>mechanic</ns1:WageType>
                           <ns1:ManualWageType>false</ns1:ManualWageType>
                           <ns1:WageLevel>1</ns1:WageLevel>
                           <ns1:Duration>2.10</ns1:Duration>
                           <ns1:ManualDuration>true</ns1:ManualDuration>
                           <ns1:ValueTotal>305.55</ns1:ValueTotal>
                           <ns1:ManualPosition>false</ns1:ManualPosition>
                           <ns1:ValueTotalCorrected>305.55</ns1:ValueTotalCorrected>
                           <ns1:hasRequiredByPosition>false</ns1:hasRequiredByPosition>
                           <ns1:Extended>false</ns1:Extended>
                           <ns1:IncludedInCalculation>true</ns1:IncludedInCalculation>
                           <ns1:LabourPositionPriceState/>
                           <ns1:LabourPositionTimeState/>
                           <ns1:WorkNumber>1550</ns1:WorkNumber>
                           <ns1:SparePartNumber>7701477024</ns1:SparePartNumber>
                        </ns1:LabourPosition>
                     </ns1:LabourPositions>
                  </ns1:CalcResultMaintenance>
                  <ns1:CalculationSummary>
                     <ns1:SparePartsCosts>
                        <ns1:AllSum>652.10</ns1:AllSum>
                        <ns1:ConsumablesSurcharge>13.04</ns1:ConsumablesSurcharge>
                        <ns1:ConsumablesSurchargePercentage>2.00</ns1:ConsumablesSurchargePercentage>
                        <ns1:TotalSum>665.14</ns1:TotalSum>
                     </ns1:SparePartsCosts>
                     <ns1:AuxiliaryCosts/>
                     <ns1:LabourCosts>
                        <ns1:AllSum>593.30</ns1:AllSum>
                        <ns1:Bodywork>
                           <ns1:Type>CAR BODY</ns1:Type>
                           <ns1:Units>2.00</ns1:Units>
                           <ns1:Price>273.20</ns1:Price>
                        </ns1:Bodywork>
                        <ns1:Electric>
                           <ns1:Type>ELECTRICS</ns1:Type>
                           <ns1:Units>0</ns1:Units>
                           <ns1:Price>0</ns1:Price>
                        </ns1:Electric>
                        <ns1:Mechanic>
                           <ns1:Type>MECHANICS</ns1:Type>
                           <ns1:Units>2.20</ns1:Units>
                           <ns1:Price>320.10</ns1:Price>
                        </ns1:Mechanic>
                        <ns1:TotalSum>593.30</ns1:TotalSum>
                        <ns1:Wages/>
                        <ns1:Works>
                           <ns1:Work>
                              <ns1:Type>CAR BODY</ns1:Type>
                              <ns1:WageLevel>1</ns1:WageLevel>
                              <ns1:Units>1.80</ns1:Units>
                              <ns1:PricePerUnit>136.60</ns1:PricePerUnit>
                              <ns1:Price>245.88</ns1:Price>
                           </ns1:Work>
                           <ns1:Work>
                              <ns1:Type>CAR BODY</ns1:Type>
                              <ns1:WageLevel>2</ns1:WageLevel>
                              <ns1:Units>0.20</ns1:Units>
                              <ns1:PricePerUnit>136.60</ns1:PricePerUnit>
                              <ns1:Price>27.32</ns1:Price>
                           </ns1:Work>
                           <ns1:Work>
                              <ns1:Type>MECHANICS</ns1:Type>
                              <ns1:WageLevel>1</ns1:WageLevel>
                              <ns1:Units>2.20</ns1:Units>
                              <ns1:PricePerUnit>145.50</ns1:PricePerUnit>
                              <ns1:Price>320.10</ns1:Price>
                           </ns1:Work>
                        </ns1:Works>
                     </ns1:LabourCosts>
                     <ns1:LacquerCosts>
                        <ns1:Wage>
                           <ns1:Type>LACQUER WORK</ns1:Type>
                           <ns1:Units>4.70</ns1:Units>
                           <ns1:PricePerUnit>156.51</ns1:PricePerUnit>
                           <ns1:Price>735.60</ns1:Price>
                        </ns1:Wage>
                        <ns1:TotalWages>735.60</ns1:TotalWages>
                        <ns1:Material>
                           <ns1:Replacement>
                              <ns1:Type>LACQUER MATERIAL REPLACEMENT</ns1:Type>
                              <ns1:Units>75.00</ns1:Units>
                              <ns1:PricePerUnit>3.80</ns1:PricePerUnit>
                              <ns1:Price>285.00</ns1:Price>
                           </ns1:Replacement>
                           <ns1:LacquerConstants>
                              <ns1:LacquerConstant>
                                 <ns1:Id>LacquerConstantMetal</ns1:Id>
                                 <ns1:Description>KONSTANTE</ns1:Description>
                                 <ns1:Price>49.70</ns1:Price>
                                 <ns1:Unit>Absolute</ns1:Unit>
                                 <ns1:ConstantType>0</ns1:ConstantType>
                                 <ns1:ValueInPositions>false</ns1:ValueInPositions>
                                 <ns1:ValueForInformation>false</ns1:ValueForInformation>
                              </ns1:LacquerConstant>
                           </ns1:LacquerConstants>
                           <ns1:TotalSum>334.70</ns1:TotalSum>
                           <ns1:SumMaterialCorrected>334.70</ns1:SumMaterialCorrected>
                        </ns1:Material>
                        <ns1:TotalSum>1070.30</ns1:TotalSum>
                     </ns1:LacquerCosts>
                     <ns1:TotalNetCosts>2328.74</ns1:TotalNetCosts>
                     <ns1:TotalVAT>442.46</ns1:TotalVAT>
                     <ns1:TotalGrossCosts>2771.20</ns1:TotalGrossCosts>
                     <ns1:TotalNetCorrected>2328.74</ns1:TotalNetCorrected>
                     <ns1:TotalVATCorrected>442.46</ns1:TotalVATCorrected>
                     <ns1:TotalGrossCorrected>2771.20</ns1:TotalGrossCorrected>
                     <ns1:SumNet>2328.74</ns1:SumNet>
                     <ns1:SumGross>2771.20</ns1:SumGross>
                     <ns1:SumSparePartCosts>652.10</ns1:SumSparePartCosts>
                     <ns1:SumSmallSparePartCosts>13.04</ns1:SumSmallSparePartCosts>
                     <ns1:SumLabourCosts>593.30</ns1:SumLabourCosts>
                     <ns1:MetaPositions>
                        <ns1:MetaPosition key="TIME_UNIT_SYSTEM" value="STD"/>
                        <ns1:MetaPosition key="LACQUER_TIME_UNIT_SYSTEM" value="STD"/>
                        <ns1:MetaPosition key="DAT_EUROLACQUER_IN_HOURS" value="false"/>
                        <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EQUIPMENT" value="false"/>
                        <ns1:MetaPosition key="PRINT_OPTION_WITHOUT_EXTENSION" value="false"/>
                        <ns1:MetaPosition key="FLAT_PERCENTAGE_BASE" value="735.60"/>
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
                  <ns1:InvoiceDate>2023-12-22T14:51:29.038+01:00</ns1:InvoiceDate>
               </ns1:RepairOrder>
               <ns1:WearCalculation>false</ns1:WearCalculation>
               <ns1:InsuranceClaim>false</ns1:InsuranceClaim>
               <ns1:ProcessManagement/>
            </ns1:Dossier>
         </calculationResult>
      </ns10:calculateResponse>
   </S:Body>
</S:Envelope>
