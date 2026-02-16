---
title: "Request changeDossierN Freies Aktenzeichen"
topic_id: "17180"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Freies Aktenzeichen > Verwalten von freien Aktenzeichen > Ändern eines freien Aktenzeichens > Request changeDossierN Freies Aktenzeichen"
---

# Request changeDossierN Freies Aktenzeichen

###### Request changeDossierN Freies Aktenzeichen ``` <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N" xmlns:vxs="http://www.dat.de/vxs">    <soapenv:Header/>    <soapenv:Body>       <dos:changeDossierN>          <vxs:Dossier>             <vxs:DossierId>3998931</vxs:DossierId>             <vxs:Vehicle>                <vxs:MileageEstimated>200000</vxs:MileageEstimated>                <vxs:InitialRegistration>2015-11-11+01:00</vxs:InitialRegistration>                <vxs:VehicleTypeNameN>Fahrzeugart MJ Test33</vxs:VehicleTypeNameN>                <vxs:ManufacturerName>Hersteller MJ1</vxs:ManufacturerName>                <vxs:BaseModelName>Haupttyp MJ</vxs:BaseModelName>                <vxs:SubModelName>Untertyp MJ</vxs:SubModelName>                <vxs:EngineNameManual>Motor MJ</vxs:EngineNameManual>                <vxs:BodyNameManual>Karosserie: MJ</vxs:BodyNameManual>                <vxs:GearboxNameManual>Getriebe MJ</vxs:GearboxNameManual>                <vxs:EquipmentLineNameManual>Ausstattungslinie</vxs:EquipmentLineNameManual>             </vxs:Vehicle>          </vxs:Dossier>          <Coverage>EXTENDEDBYTRADING</Coverage>       </dos:changeDossierN>    </soapenv:Body> </soapenv:Envelope> ```
