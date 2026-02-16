---
title: "Response getExtPartNoInfoByModelAndExtPartNo"
topic_id: "2551"
breadcrumb: "SilverDAT Produkte > SilverDAT PartsInfo > Schnittstellenoperationen > Informationsermittlung mit Untertyp und ETN > Response getExtPartNoInfoByModelAndExtPartNo"
---

# Response getExtPartNoInfoByModelAndExtPartNo

```
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns3:getExtPartNoInfoByModelAndExtPartNoResponse xmlns:ns3="http://sphinx.dat.de/services/SpareParts">
         <result>
            <ns1:Dossiers source="SD3" xmlns:ns1="http://www.dat.de/vxs">
               <ns1:Dossier>
                  <ns1:Country>DE</ns1:Country>
                  <ns1:Language>de</ns1:Language>
                  <ns1:Vehicle>
                     <ns1:DatECode>011300660340001</ns1:DatECode>
                     <ns1:VehicleTypeName>Pkw, SUV, Kleintransporter</ns1:VehicleTypeName>
                     <ns1:ManufacturerName origin="dat">BMW</ns1:ManufacturerName>
                     <ns1:BaseModelName origin="dat">Baureihe 5 Touring (E61) (2004->)</ns1:BaseModelName>
                     <ns1:SubModelName origin="dat">530d xDrive</ns1:SubModelName>
                     <ns1:Equipment>
                        <ns1:SeriesEquipment/>
                     </ns1:Equipment>
                     <ns1:DATECodeEquipment>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                           <ns1:Description>Karosserie: 5-türig</ns1:Description>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>75205</ns1:DatEquipmentId>
                           <ns1:Description>Getriebe 6-Gang</ns1:Description>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>92903</ns1:DatEquipmentId>
                           <ns1:Description>Motor 3,0 Ltr. - 170 kW Turbodiesel KAT</ns1:Description>
                        </ns1:EquipmentPosition>
                     </ns1:DATECodeEquipment>
                  </ns1:Vehicle>
                  <ns1:SparePartPositions>
                     <ns1:SparePartPosition>
                        <ns1:DATProcessId>43711</ns1:DATProcessId>
                        <ns1:DATProcessIdName>KOTFLUEGEL L. KPL.</ns1:DATProcessIdName>
                        <ns1:PartNumber>41357111429</ns1:PartNumber>
                        <ns1:Description>SEITENWAND V.L.</ns1:Description>
                        <ns1:LastUPE>327.00</ns1:LastUPE>
                        <ns1:LastUPEDate>2019-08-01T00:00:00+02:00</ns1:LastUPEDate>
                        <ns1:SecondtoLastUPE>327.00</ns1:SecondtoLastUPE>
                        <ns1:SecondtoLastUPEDate>2019-07-01T00:00:00+02:00</ns1:SecondtoLastUPEDate>
                        <ns1:ThirdtoLastUPE>327.00</ns1:ThirdtoLastUPE>
                        <ns1:ThirdtoLastUPEDate>2019-06-01T00:00:00+02:00</ns1:ThirdtoLastUPEDate>
                        <ns1:FourthtoLastUPE>325.55</ns1:FourthtoLastUPE>
                        <ns1:FourthtoLastUPEDate>2019-05-01T00:00:00+02:00</ns1:FourthtoLastUPEDate>
                        <ns1:Orderable>true</ns1:Orderable>
                        <ns1:WorkTimeMin>2.00</ns1:WorkTimeMin>
                        <ns1:WorkTimeMax>2.00</ns1:WorkTimeMax>
                        <ns1:SparePartHistoryPositions>
                           <ns1:SparePartHistoryPosition>
                              <ns1:PartNumber>41357111373</ns1:PartNumber>
                              <ns1:LastUPE>212.47</ns1:LastUPE>
                              <ns1:LastUPEDate>2009-03-03+01:00</ns1:LastUPEDate>
                           </ns1:SparePartHistoryPosition>
                        </ns1:SparePartHistoryPositions>
                     </ns1:SparePartPosition>
                  </ns1:SparePartPositions>
               </ns1:Dossier>
               <ns1:Dossier>
                  <ns1:Country>DE</ns1:Country>
                  <ns1:Language>de</ns1:Language>
                  <ns1:Vehicle>
                     <ns1:DatECode>011300660340005</ns1:DatECode>
                     <ns1:VehicleTypeName>Pkw, SUV, Kleintransporter</ns1:VehicleTypeName>
                     <ns1:ManufacturerName origin="dat">BMW</ns1:ManufacturerName>
                     <ns1:BaseModelName origin="dat">Baureihe 5 Touring (E61) (2004->)</ns1:BaseModelName>
                     <ns1:SubModelName origin="dat">530d xDrive</ns1:SubModelName>
                     <ns1:Equipment>
                        <ns1:SeriesEquipment/>
                     </ns1:Equipment>
                     <ns1:DATECodeEquipment>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>92930</ns1:DatEquipmentId>
                           <ns1:Description>Motor 3,0 Ltr. - 173 kW Turbodiesel KAT</ns1:Description>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                           <ns1:Description>Karosserie: 5-türig</ns1:Description>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>75205</ns1:DatEquipmentId>
                           <ns1:Description>Getriebe 6-Gang</ns1:Description>
                        </ns1:EquipmentPosition>
                     </ns1:DATECodeEquipment>
                  </ns1:Vehicle>
                  <ns1:SparePartPositions>
                     <ns1:SparePartPosition>
                        <ns1:DATProcessId>43711</ns1:DATProcessId>
                        <ns1:DATProcessIdName>KOTFLUEGEL L. KPL.</ns1:DATProcessIdName>
                        <ns1:PartNumber>41357111429</ns1:PartNumber>
                        <ns1:Description>SEITENWAND V.L.</ns1:Description>
                        <ns1:LastUPE>327.00</ns1:LastUPE>
                        <ns1:LastUPEDate>2019-08-01T00:00:00+02:00</ns1:LastUPEDate>
                        <ns1:SecondtoLastUPE>327.00</ns1:SecondtoLastUPE>
                        <ns1:SecondtoLastUPEDate>2019-07-01T00:00:00+02:00</ns1:SecondtoLastUPEDate>
                        <ns1:ThirdtoLastUPE>327.00</ns1:ThirdtoLastUPE>
                        <ns1:ThirdtoLastUPEDate>2019-06-01T00:00:00+02:00</ns1:ThirdtoLastUPEDate>
                        <ns1:FourthtoLastUPE>325.55</ns1:FourthtoLastUPE>
                        <ns1:FourthtoLastUPEDate>2019-05-01T00:00:00+02:00</ns1:FourthtoLastUPEDate>
                        <ns1:Orderable>true</ns1:Orderable>
                        <ns1:WorkTimeMin>2.00</ns1:WorkTimeMin>
                        <ns1:WorkTimeMax>2.00</ns1:WorkTimeMax>
                        <ns1:SparePartHistoryPositions>
                           <ns1:SparePartHistoryPosition>
                              <ns1:PartNumber>41357111373</ns1:PartNumber>
                              <ns1:LastUPE>212.47</ns1:LastUPE>
                              <ns1:LastUPEDate>2009-03-03+01:00</ns1:LastUPEDate>
                           </ns1:SparePartHistoryPosition>
                        </ns1:SparePartHistoryPositions>
                     </ns1:SparePartPosition>
                  </ns1:SparePartPositions>
               </ns1:Dossier>
               <ns1:Dossier>
                  <ns1:Country>DE</ns1:Country>
                  <ns1:Language>de</ns1:Language>
                  <ns1:Vehicle>
                     <ns1:DatECode>011300660340002</ns1:DatECode>
                     <ns1:VehicleTypeName>Pkw, SUV, Kleintransporter</ns1:VehicleTypeName>
                     <ns1:ManufacturerName origin="dat">BMW</ns1:ManufacturerName>
                     <ns1:BaseModelName origin="dat">Baureihe 5 Touring (E61) (2004->)</ns1:BaseModelName>
                     <ns1:SubModelName origin="dat">530d xDrive</ns1:SubModelName>
                     <ns1:Equipment>
                        <ns1:SeriesEquipment/>
                     </ns1:Equipment>
                     <ns1:DATECodeEquipment>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>75904</ns1:DatEquipmentId>
                           <ns1:Description>Getriebe Automatik - mit Steptronic (6-Stufen)</ns1:Description>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                           <ns1:Description>Karosserie: 5-türig</ns1:Description>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>92903</ns1:DatEquipmentId>
                           <ns1:Description>Motor 3,0 Ltr. - 170 kW Turbodiesel KAT</ns1:Description>
                        </ns1:EquipmentPosition>
                     </ns1:DATECodeEquipment>
                  </ns1:Vehicle>
                  <ns1:SparePartPositions>
                     <ns1:SparePartPosition>
                        <ns1:DATProcessId>43711</ns1:DATProcessId>
                        <ns1:DATProcessIdName>KOTFLUEGEL L. KPL.</ns1:DATProcessIdName>
                        <ns1:PartNumber>41357111429</ns1:PartNumber>
                        <ns1:Description>SEITENWAND V.L.</ns1:Description>
                        <ns1:LastUPE>327.00</ns1:LastUPE>
                        <ns1:LastUPEDate>2019-08-01T00:00:00+02:00</ns1:LastUPEDate>
                        <ns1:SecondtoLastUPE>327.00</ns1:SecondtoLastUPE>
                        <ns1:SecondtoLastUPEDate>2019-07-01T00:00:00+02:00</ns1:SecondtoLastUPEDate>
                        <ns1:ThirdtoLastUPE>327.00</ns1:ThirdtoLastUPE>
                        <ns1:ThirdtoLastUPEDate>2019-06-01T00:00:00+02:00</ns1:ThirdtoLastUPEDate>
                        <ns1:FourthtoLastUPE>325.55</ns1:FourthtoLastUPE>
                        <ns1:FourthtoLastUPEDate>2019-05-01T00:00:00+02:00</ns1:FourthtoLastUPEDate>
                        <ns1:Orderable>true</ns1:Orderable>
                        <ns1:WorkTimeMin>2.00</ns1:WorkTimeMin>
                        <ns1:WorkTimeMax>2.00</ns1:WorkTimeMax>
                        <ns1:SparePartHistoryPositions>
                           <ns1:SparePartHistoryPosition>
                              <ns1:PartNumber>41357111373</ns1:PartNumber>
                              <ns1:LastUPE>212.47</ns1:LastUPE>
                              <ns1:LastUPEDate>2009-03-03+01:00</ns1:LastUPEDate>
                           </ns1:SparePartHistoryPosition>
                        </ns1:SparePartHistoryPositions>
                     </ns1:SparePartPosition>
                  </ns1:SparePartPositions>
               </ns1:Dossier>
               <ns1:Dossier>
                  <ns1:Country>DE</ns1:Country>
                  <ns1:Language>de</ns1:Language>
                  <ns1:Vehicle>
                     <ns1:DatECode>011300660340006</ns1:DatECode>
                     <ns1:VehicleTypeName>Pkw, SUV, Kleintransporter</ns1:VehicleTypeName>
                     <ns1:ManufacturerName origin="dat">BMW</ns1:ManufacturerName>
                     <ns1:BaseModelName origin="dat">Baureihe 5 Touring (E61) (2004->)</ns1:BaseModelName>
                     <ns1:SubModelName origin="dat">530d xDrive</ns1:SubModelName>
                     <ns1:Equipment>
                        <ns1:SeriesEquipment/>
                     </ns1:Equipment>
                     <ns1:DATECodeEquipment>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>75904</ns1:DatEquipmentId>
                           <ns1:Description>Getriebe Automatik - mit Steptronic (6-Stufen)</ns1:Description>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>92930</ns1:DatEquipmentId>
                           <ns1:Description>Motor 3,0 Ltr. - 173 kW Turbodiesel KAT</ns1:Description>
                        </ns1:EquipmentPosition>
                        <ns1:EquipmentPosition>
                           <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                           <ns1:Description>Karosserie: 5-türig</ns1:Description>
                        </ns1:EquipmentPosition>
                     </ns1:DATECodeEquipment>
                  </ns1:Vehicle>
                  <ns1:SparePartPositions>
                     <ns1:SparePartPosition>
                        <ns1:DATProcessId>43711</ns1:DATProcessId>
                        <ns1:DATProcessIdName>KOTFLUEGEL L. KPL.</ns1:DATProcessIdName>
                        <ns1:PartNumber>41357111429</ns1:PartNumber>
                        <ns1:Description>SEITENWAND V.L.</ns1:Description>
                        <ns1:LastUPE>327.00</ns1:LastUPE>
                        <ns1:LastUPEDate>2019-08-01T00:00:00+02:00</ns1:LastUPEDate>
                        <ns1:SecondtoLastUPE>327.00</ns1:SecondtoLastUPE>
                        <ns1:SecondtoLastUPEDate>2019-07-01T00:00:00+02:00</ns1:SecondtoLastUPEDate>
                        <ns1:ThirdtoLastUPE>327.00</ns1:ThirdtoLastUPE>
                        <ns1:ThirdtoLastUPEDate>2019-06-01T00:00:00+02:00</ns1:ThirdtoLastUPEDate>
                        <ns1:FourthtoLastUPE>325.55</ns1:FourthtoLastUPE>
                        <ns1:FourthtoLastUPEDate>2019-05-01T00:00:00+02:00</ns1:FourthtoLastUPEDate>
                        <ns1:Orderable>true</ns1:Orderable>
                        <ns1:WorkTimeMin>2.00</ns1:WorkTimeMin>
                        <ns1:WorkTimeMax>2.00</ns1:WorkTimeMax>
                        <ns1:SparePartHistoryPositions>
                           <ns1:SparePartHistoryPosition>
                              <ns1:PartNumber>41357111373</ns1:PartNumber>
                              <ns1:LastUPE>212.47</ns1:LastUPE>
                              <ns1:LastUPEDate>2009-03-03+01:00</ns1:LastUPEDate>
                           </ns1:SparePartHistoryPosition>
                        </ns1:SparePartHistoryPositions>
                     </ns1:SparePartPosition>
                  </ns1:SparePartPositions>
               </ns1:Dossier>
            </ns1:Dossiers>
         </result>
      </ns3:getExtPartNoInfoByModelAndExtPartNoResponse>
   </S:Body>
</S:Envelope>
```
