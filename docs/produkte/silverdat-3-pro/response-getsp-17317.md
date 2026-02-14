---
title: "Response getSparePartsDetails"
topic_id: "17317"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > Ermittlung von Fahrzeuginformationen, DVN, Verbauungsbedingungen und/oder Preishistorie > Response getSparePartsDetails"
---

# Response getSparePartsDetails

```
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns3:getSparePartsDetailsResponse xmlns:ns3="http://www.dat.eu/myClaim/soap/v2/VehicleRepairService">
         <SparePartsDetailsResponse>
            <sparePartsResultPerSparePartNumber>
               <pageSize>20</pageSize>
               <pageNumber>1</pageNumber>
               <partNumber>51317070292</partNumber>
               <vehiclesFound>4</vehiclesFound>
               <vehiclesReturned>4</vehiclesReturned>
               <sparePartsInformations>
                  <sparePartsInformation>
                     <name>FRONTSCHEIBE</name>
                     <partNumber>51317070292</partNumber>
                     <price>354.56</price>
                     <priceDate>2022-10-01</priceDate>
                     <orderable>yes</orderable>
                     <possibleNames>
                        <identifier>*</identifier>
                        <name>FRONTSCHEIBE</name>
                     </possibleNames>
                     <previousPrices>
                        <previousPrice>
                           <price>354.56</price>
                           <priceDate>2022-09-01</priceDate>
                        </previousPrice>
                     </previousPrices>
                     <repairSet>
                        <sparePartsInformation>
                           <name>KLEBEDICHTMASSE SCHEIBE</name>
                           <partNumber>83192289286</partNumber>
                           <price>16.81</price>
                           <priceDate>2022-10-01</priceDate>
                           <amount>1</amount>
                           <orderable>yes</orderable>
                           <possibleNames>
                              <identifier>*</identifier>
                              <name>KLEBEDICHTMASSE SCHEIBE</name>
                           </possibleNames>
                           <previousPrices>
                              <previousPrice>
                                 <price>16.81</price>
                                 <priceDate>2022-09-01</priceDate>
                              </previousPrice>
                           </previousPrices>
                        </sparePartsInformation>
                     </repairSet>
                  </sparePartsInformation>
               </sparePartsInformations>
               <sparePartsVehicles>
                  <sparePartsVehicle>
                     <datProcessNumber>44910</datProcessNumber>
                     <partNumber>51317070292</partNumber>
                     <vehicleType>1</vehicleType>
                     <vehicleTypeName>Pkw, SUV, Kleintransporter</vehicleTypeName>
                     <manufacturer>130</manufacturer>
                     <manufacturerName>BMW</manufacturerName>
                     <baseModel>66</baseModel>
                     <baseModelName>Baureihe 5 Touring (E61)(2004->)</baseModelName>
                     <constructionTimeFrom>1</constructionTimeFrom>
                     <constructionTimeTo>9999</constructionTimeTo>
                     <constructionCondition>28807&amp;99952</constructionCondition>
                     <excludingCondition>22204/22506/25204</excludingCondition>
                     <descriptionIdentifier>*</descriptionIdentifier>
                     <sparePartsSubModels>
                        <sparePartsSubModel>
                           <subModel>1</subModel>
                           <subModelName>520i</subModelName>
                        </sparePartsSubModel>
                        <sparePartsSubModel>
                           <subModel>3</subModel>
                           <subModelName>523i</subModelName>
                        </sparePartsSubModel>
                        <sparePartsSubModel>
                           <subModel>5</subModel>
                           <subModelName>525i</subModelName>
                        </sparePartsSubModel>
                        <sparePartsSubModel>
                           <subModel>6</subModel>
                           <subModelName>525i xDrive</subModelName>
                        </sparePartsSubModel>
                        <sparePartsSubModel>
...................................................................
                     </sparePartsSubModels>
                  </sparePartsVehicle>
                  <sparePartsVehicle>
                     <datProcessNumber>44910</datProcessNumber>
                     <partNumber>51317070292</partNumber>
                     <vehicleType>1</vehicleType>
                     <vehicleTypeName>Pkw, SUV, Kleintransporter</vehicleTypeName>
                     <manufacturer>130</manufacturer>
                     <manufacturerName>BMW</manufacturerName>
                     <baseModel>66</baseModel>
                     <baseModelName>Baureihe 5 Touring (E61)(2004->)</baseModelName>
                     <constructionTimeFrom>1</constructionTimeFrom>
                     <constructionTimeTo>9999</constructionTimeTo>
                     <constructionCondition>99952</constructionCondition>
                     <excludingCondition>22204/22506/25204/28807</excludingCondition>
                     <descriptionIdentifier>*</descriptionIdentifier>
                     <sparePartsSubModels>
………………………………………………………………………...................................................
                                          </sparePartsVehicle>
                  <sparePartsVehicle>
                     <datProcessNumber>44910</datProcessNumber>
                     <partNumber>51317070292</partNumber>
                     <vehicleType>1</vehicleType>
                     <vehicleTypeName>Pkw, SUV, Kleintransporter</vehicleTypeName>
                     <manufacturer>130</manufacturer>
                     <manufacturerName>BMW</manufacturerName>
                     <baseModel>66</baseModel>
                     <baseModelName>Baureihe 5 Touring (E61)(2004->)</baseModelName>
                     <constructionTimeFrom>1</constructionTimeFrom>
                     <constructionTimeTo>9999</constructionTimeTo>
                     <excludingCondition>22204/22506/25204/28807/99952</excludingCondition>
                     <descriptionIdentifier>*</descriptionIdentifier>
                     <sparePartsSubModels>
…………………………………………………………...................................................................
                                             </sparePartsSubModels>
                  </sparePartsVehicle>
                  <sparePartsVehicle>
                     <datProcessNumber>44910</datProcessNumber>
                     <partNumber>51317070292</partNumber>
                     <vehicleType>1</vehicleType>
                     <vehicleTypeName>Pkw, SUV, Kleintransporter</vehicleTypeName>
                     <manufacturer>130</manufacturer>
                     <manufacturerName>BMW</manufacturerName>
                     <baseModel>66</baseModel>
                     <baseModelName>Baureihe 5 Touring (E61)(2004->)</baseModelName>
                     <constructionTimeFrom>1</constructionTimeFrom>
                     <constructionTimeTo>9999</constructionTimeTo>
                     <constructionCondition>28807</constructionCondition>
                     <excludingCondition>22204/22506/25204/99952</excludingCondition>
                     <descriptionIdentifier>*</descriptionIdentifier>
                     <sparePartsSubModels>
…………………………………………………………………............................................................
                     </sparePartsSubModels>
                  </sparePartsVehicle>
               </sparePartsVehicles>
               <equipments>
                  <equipment>
                     <name>Verglasung Verbundglas (Ausführung: Klimakomfort)</name>
                     <number>22204</number>
                  </equipment>
                  <equipment>
                     <name>Frontscheibe mit Bandfilter oben</name>
                     <number>22506</number>
                  </equipment>
                  <equipment>
                     <name>Head-up-Display</name>
                     <number>25204</number>
                  </equipment>
                  <equipment>
                     <name>Klimaautomatik erweiterter Umfang</name>
                     <number>28807</number>
                  </equipment>
                  <equipment>
                     <name>Länder-AV China</name>
                     <number>99952</number>
                  </equipment>
               </equipments>
            </sparePartsResultPerSparePartNumber>
         </SparePartsDetailsResponse>
      </ns3:getSparePartsDetailsResponse>
   </S:Body>
</S:Envelope>
```
