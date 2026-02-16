---
title: "Request zum Löschen der Bezeichner der Fahrzeugauswahlparameter"
topic_id: "19556"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Freies Aktenzeichen > Verwalten von freien Aktenzeichen > Löschen der Bezeichner der Fahrzeugauswahlparameter > Request zum Löschen der Bezeichner der Fahrzeugauswahlparameter"
---

# Request zum Löschen der Bezeichner der Fahrzeugauswahlparameter

###### Request zum Löschen der Bezeichner der Fahrzeugauswahlparameter ``` soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:dos="http://www.dat.de/services/Dossier1N" xmlns:vxs="http://www.dat.de/vxs">    <soapenv:Header/>    <soapenv:Body>       <dos:changeDossierN>          <vxs:Dossier>             <vxs:DossierId>12345678</vxs:DossierId>             <vxs:Vehicle>                <vxs:VehicleTypeNameN overwrite="true"></vxs:VehicleTypeNameN>                <vxs:ManufacturerName overwrite="true" />                <vxs:BaseModelName overwrite="true" />                <vxs:SubModelName overwrite="true" />                <vxs:EngineNameManual overwrite="true" />                <vxs:BodyNameManual overwrite="true" />                <vxs:GearboxNameManual overwrite="true"/>                <vxs:EquipmentLineNameManual overwrite="true" />                <vxs:ContainerNameN overwrite="true" />             </vxs:Vehicle>          </vxs:Dossier>          <Coverage>COMPLETE</Coverage>       </dos:changeDossierN>    </soapenv:Body> </soapenv:Envelope> ```
