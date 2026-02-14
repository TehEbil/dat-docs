---
title: "Response getSparePartsDetailsForDPNByVIN"
topic_id: "17329"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, Ersatzteilnummer und Preishistorie > Response getSparePartsDetailsForDPNByVIN"
---

# Response getSparePartsDetailsForDPNByVIN

```
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns6:getSparePartsDetailsForDPNByVINResponse xmlns:ns6="http://www.dat.eu/myClaim/soap/v2/VehicleRepairService">
         <SparePartsDetailsForDPNByVINResponse>
            <sparePartsResultPerDPN>
               <datProcessNumber>44210</datProcessNumber>
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
            </sparePartsResultPerDPN>
            <ns1:Dossier xmlns:ns1="http://www.dat.de/vxs">
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
                  <ns1:VinAccuracy>0</ns1:VinAccuracy>
                  <ns1:ReleaseIndicator>ALL</ns1:ReleaseIndicator>
                  <ns1:KbaNumbersN>
                     <ns1:KbaNumber>0603/BQS</ns1:KbaNumber>
                  </ns1:KbaNumbersN>
                  <ns1:PaintTypes>
                     <ns1:PaintType>30</ns1:PaintType>
                  </ns1:PaintTypes>
                  <ns1:Equipment>
                  </ns1:VINResult>
                  …
                  …
<ns1:TokenOfVinResult>eyJhbGciOiJIUzI1NiIsI…</ns1:TokenOfVinResult>
               </ns1:Vehicle>
            </ns1:Dossier>
         </SparePartsDetailsForDPNByVINResponse>
      </ns6:getSparePartsDetailsForDPNByVINResponse>
   </S:Body>
</S:Envelope>
```
