---
title: "Response getSparePartsDetailsByVIN"
topic_id: "17166"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, DVNs und Preishistorie > Response getSparePartsDetailsByVIN"
---

# Response getSparePartsDetailsByVIN

```
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns6:getSparePartsDetailsByVINResponse xmlns:ns6="http://sphinx.dat.de/services/VehicleRepairService">
         <SparePartsDetailsByVINResponse>
            <sparePartsResultPerSparePartNumber>
               <partNumber>3G0823031C</partNumber>
               <sparePartsInformations>
                  <sparePartsInformation>
                     <name>FRONTKLAPPE</name>
                     <partNumber>3G0823031C</partNumber>
                     <price>540</price>
                     <priceDate>2022-01-01</priceDate>
                     <orderable>yes</orderable>
                     <possibleNames>
                        <identifier>*</identifier>
                        <name>FRONTKLAPPE</name>
                     </possibleNames>
                     <previousPrices>
                        <previousPrice>
                           <price>520.0</price>
                           <priceDate>2021-12-01</priceDate>
                        </previousPrice>
                     </previousPrices>
                  </sparePartsInformation>
               </sparePartsInformations>
            </sparePartsResultPerSparePartNumber>
            <ns1:Dossiers xmlns:ns1="http://www.dat.de/vxs">
               <ns1:Country>DE</ns1:Country>
               <ns1:Language>de_DE</ns1:Language>
               <ns1:Vehicle>
                  <ns1:DatECode>019051150020002</ns1:DatECode>
                  <ns1:Container>DE001</ns1:Container>
                  <ns1:ConstructionTime>5386</ns1:ConstructionTime>
                  <ns1:ConstructionTimeFrom>5350</ns1:ConstructionTimeFrom>
                  <ns1:ConstructionTimeTo>9999</ns1:ConstructionTimeTo>
                  <ns1:VehicleTypeName>Pkw, SUV, Kleintransporter</ns1:VehicleTypeName>
                  <ns1:VehicleTypeNameN origin="dat">Pkw, SUV, Kleintransporter</ns1:VehicleTypeNameN>
                  <ns1:ManufacturerName origin="dat">Volkswagen</ns1:ManufacturerName>
                  <ns1:BaseModelName origin="dat">Passat Variant (3G5)(07.2014->2019)</ns1:BaseModelName>
                  <ns1:SubModelName origin="dat">Trendline BMT/Start-Stopp</ns1:SubModelName>
                  <ns1:MainTypeGroupName>Passat</ns1:MainTypeGroupName>
                  <ns1:VehicleType>1</ns1:VehicleType>
                  <ns1:Manufacturer>905</ns1:Manufacturer>
                  <ns1:BaseModel>115</ns1:BaseModel>
                  <ns1:SubModel>2</ns1:SubModel>
                  <ns1:MainTypeGroup>PAS</ns1:MainTypeGroup>
                  <ns1:IdentificationSource>IDENTIFICATIONSOURCE_VIN</ns1:IdentificationSource>
            …
            …

                  </ns1:VINResult>
                  <ns1:TokenOfVinResult>eyJhbGciOiJIUzI1NiI…</ns1:TokenOfVinResult>
               </ns1:Vehicle>
            </ns1:Dossiers>
         </SparePartsDetailsByVINResponse>
      </ns6:getSparePartsDetailsByVINResponse>
   </S:Body>
</S:Envelope>
```
