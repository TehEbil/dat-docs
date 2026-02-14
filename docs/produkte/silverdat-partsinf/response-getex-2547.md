---
title: "Response getExtPartNoInfoByVinAndIntPartNo"
topic_id: "2547"
breadcrumb: "SilverDAT Produkte > SilverDAT PartsInfo > Schnittstellenoperationen > Rückgabe ETN über VIN und DVN > Response getExtPartNoInfoByVinAndIntPartNo"
---

# Response getExtPartNoInfoByVinAndIntPartNo

```
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns2:getExtPartNoInfoByVinAndIntPartNoResponse xmlns:ns2="http://sphinx.dat.de/services/SpareParts" xmlns:ns3="http://www.dat.de/vxs">
         <result>
            <ns3:Dossiers source="SD3">
               <ns3:Dossier>
                  <ns3:Country>D</ns3:Country>
                  <ns3:Language>de_DE</ns3:Language>
                  <ns3:Vehicle>
                     <ns3:DatECode>011300820150001</ns3:DatECode>
                     <ns3:ManufacturerName>BMW</ns3:ManufacturerName>
                     <ns3:VehicleTypeName>Pkw, SUV, Kleintransporter</ns3:VehicleTypeName>
                     <ns3:BaseModelName>MINI (R56) (2006->)</ns3:BaseModelName>
                     <ns3:SubModelName>Cooper D</ns3:SubModelName>
                     <ns3:Equipment>
                        <ns3:SeriesEquipment>
                           <ns3:EquipmentPosition>
                              <ns3:DatEquipmentId>98607</ns3:DatEquipmentId>
                              <ns3:Description>Lautsprecher - Heck</ns3:Description>
                           </ns3:EquipmentPosition>
                           <ns3:EquipmentPosition>
                              <ns3:DatEquipmentId>98608</ns3:DatEquipmentId>
                              <ns3:Description>Lautsprecher - Tür</ns3:Description>
                           </ns3:EquipmentPosition>
                           <ns3:VINumber>
                              <ns3:VinCode>WMWMG31090TU52263</ns3:VinCode>
                           </ns3:VINumber>
                        </ns3:VINVehicle>
                     </ns3:VINResult>
                  </ns3:Vehicle>
                  <ns3:SparePartPositions>
                     <ns3:SparePartPosition>
                        <ns3:DATProcessId>83110</ns3:DATProcessId>
                        <ns3:PartNumber>13717805323</ns3:PartNumber>
                        <ns3:Description>ANSAUGFILTERGEHAEUSE</ns3:Description>
                        <ns3:LastUPE>94.2000000000000028421709430404007434844970703125</ns3:LastUPE>
                        <ns3:LastUPEDate>2010-05-01T00:00:00+02:00</ns3:LastUPEDate>
                        <ns3:SecondtoLastUPE>94.2000000000000028421709430404007434844970703125</ns3:SecondtoLastUPE>
                        <ns3:SecondtoLastUPEDate>2010-04-01T00:00:00+02:00</ns3:SecondtoLastUPEDate>
                        <ns3:ThirdtoLastUPE>94.2000000000000028421709430404007434844970703125</ns3:ThirdtoLastUPE>
                        <ns3:ThirdtoLastUPEDate>2010-03-01T00:00:00+01:00</ns3:ThirdtoLastUPEDate>
                        <ns3:FourthtoLastUPE>94.2000000000000028421709430404007434844970703125</ns3:FourthtoLastUPE>
                        <ns3:FourthtoLastUPEDate>2010-02-01T00:00:00+01:00</ns3:FourthtoLastUPEDate>
                        <ns3:EquipmentPositions>
                           <ns3:EquipmentPosition>
                              <ns3:DatEquipmentId>83950</ns3:DatEquipmentId>
                              <ns3:Description>Motor 1,6 Ltr. - 80 kW 16V Diesel KAT</ns3:Description>
                           </ns3:EquipmentPosition>
                        </ns3:EquipmentPositions>
                     </ns3:SparePartPosition>
                  </ns3:SparePartPositions>
               </ns3:Dossier>
            </ns3:Dossiers>
         </result>
      </ns2:getExtPartNoInfoByVinAndIntPartNoResponse>
   </S:Body>
</S:Envelope>
```
