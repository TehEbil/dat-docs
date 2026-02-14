---
title: "Request createDossierN with Additional and Specialequipment"
topic_id: "15078"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Erstellen eines neuen Vorgangs > Request createDossierN with Additional and Specialequipment"
---

# Request createDossierN with Additional and Specialequipment

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N" xmlns:vxs="http://www.dat.de/vxs">
   <soapenv:Header/>
   <soapenv:Body>
      <dos:createDossierN>
         <vxs:Dossier>
            <vxs:Name>createDossierN with equipment</vxs:Name>
            <vxs:Language>de_DE</vxs:Language>
            <vxs:Vehicle>
               <vxs:Country>DE</vxs:Country>
               <vxs:DatECode>019050030020043</vxs:DatECode>
               <vxs:Container>DE00L</vxs:Container>
               <vxs:ConstructionTime>4423</vxs:ConstructionTime>
               <vxs:MileageEstimated>99000</vxs:MileageEstimated>
               <vxs:InitialRegistration>2006-05-17+02:00</vxs:InitialRegistration>
               <vxs:Equipment>
                  <vxs:SpecialEquipment>
                     <vxs:EquipmentPosition>
                        <vxs:DatEquipmentId>70308</vxs:DatEquipmentId>
                        <vxs:OriginalPrice>100</vxs:OriginalPrice>
                        <vxs:Description>Audio-Navigationssystem RNS MCD (8 Lautsprecher)</vxs:Description>
                        <vxs:DecreaseType>T1</vxs:DecreaseType>
                        <vxs:InstallDate>2010-10-01+02:00</vxs:InstallDate>
                     </vxs:EquipmentPosition>
                     <vxs:EquipmentPosition>
                        <vxs:DatEquipmentId>70308</vxs:DatEquipmentId>
                     </vxs:EquipmentPosition>
                     <vxs:EquipmentPosition>
                        <vxs:DatEquipmentId>26708</vxs:DatEquipmentId>
                     </vxs:EquipmentPosition>
                     <vxs:EquipmentPosition>
                        <vxs:DatEquipmentId>47607</vxs:DatEquipmentId>
                     </vxs:EquipmentPosition>
                  </vxs:SpecialEquipment>
                  <vxs:AdditionalEquipment>
                     <vxs:EquipmentPosition>
                        <vxs:InstallDate>2010-10-01+02:00</vxs:InstallDate>
                        <vxs:Description>Zusatz</vxs:Description>
                        <vxs:DecreaseType>T1</vxs:DecreaseType>
                        <vxs:OriginalPrice>100</vxs:OriginalPrice>
                     </vxs:EquipmentPosition>
                  </vxs:AdditionalEquipment>
               </vxs:Equipment>
            </vxs:Vehicle>
            <vxs:VAT>
               <vxs:VatType>difference</vxs:VatType>
            </vxs:VAT>
         </vxs:Dossier>
         <Save>false</Save>
      </dos:createDossierN>
   </soapenv:Body>
</soapenv:Envelope>
```
