---
title: "Response getExtPartNoInfoByMfrAndExtPartNo"
topic_id: "2545"
breadcrumb: "SilverDAT Produkte > SilverDAT PartsInfo > Schnittstellenoperationen > Informationsermittlung mit Herstellerschlüssel und ETN > Response getExtPartNoInfoByMfrAndExtPartNo"
---

# Response getExtPartNoInfoByMfrAndExtPartNo

```
<?xml version="1.0" encoding="UTF-8" standalone="no"?>
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
    <S:Body>
        <ns3:getExtPartNoInfoByMfrAndExtPartNoResponse xmlns:ns3="http://sphinx.dat.de/services/SpareParts">
            <result>
                <ns1:Dossiers xmlns:ns1="http://www.dat.de/vxs" source="SD3">
                    <ns1:Dossier>
                        <ns1:Country>DE</ns1:Country>
                        <ns1:Language>de</ns1:Language>
                        <ns1:Vehicle>
                            <ns1:DatECode>015800030020007</ns1:DatECode>
                            <ns1:VehicleTypeName>Pkw, SUV, Kleintransporter</ns1:VehicleTypeName>
                            <ns1:ManufacturerName origin="dat">MINI</ns1:ManufacturerName>
                            <ns1:BaseModelName origin="dat">Mini (R56)(2006-&gt;)</ns1:BaseModelName>
                            <ns1:SubModelName origin="dat">One</ns1:SubModelName>
                            <ns1:Equipment>
                                <ns1:SeriesEquipment/>
                            </ns1:Equipment>
                            <ns1:DATECodeEquipment>
                                <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>10003</ns1:DatEquipmentId>
                                    <ns1:Description>Karosserie: 3-türig</ns1:Description>
                                </ns1:EquipmentPosition>
                                <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>96515</ns1:DatEquipmentId>
                                    <ns1:Description>Motor 1,6 Ltr. - 72 kW 16V</ns1:Description>
                                </ns1:EquipmentPosition>
                                <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>75205</ns1:DatEquipmentId>
                                    <ns1:Description>Getriebe 6-Gang</ns1:Description>
                                </ns1:EquipmentPosition>
                            </ns1:DATECodeEquipment>
                        </ns1:Vehicle>
                        <ns1:SparePartPositions>
                            <ns1:SparePartPosition>
                                <ns1:DATProcessId>82526</ns1:DATProcessId>
                                <ns1:DATProcessIdName>ANSAUGLUFT SAUGROHR HALTER H.</ns1:DATProcessIdName>
                                <ns1:PartNumber>11617569966      </ns1:PartNumber>
                                <ns1:Description>STUETZE ANSAUGKRUEMMER</ns1:Description>
                                <ns1:LastUPE>17.83</ns1:LastUPE>
                                <ns1:LastUPEDate>2024-04-01T00:00:00+02:00</ns1:LastUPEDate>
                                <ns1:SecondtoLastUPE>17.83</ns1:SecondtoLastUPE>
                                <ns1:SecondtoLastUPEDate>2024-03-01T00:00:00+01:00</ns1:SecondtoLastUPEDate>
                                <ns1:ThirdtoLastUPE>17.83</ns1:ThirdtoLastUPE>
                                <ns1:ThirdtoLastUPEDate>2024-02-01T00:00:00+01:00</ns1:ThirdtoLastUPEDate>
                                <ns1:FourthtoLastUPE>17.83</ns1:FourthtoLastUPE>
                                <ns1:FourthtoLastUPEDate>2024-01-01T00:00:00+01:00</ns1:FourthtoLastUPEDate>
                                <ns1:EquipmentPositions>
                                    <ns1:EquipmentPosition>
                                        <ns1:DatEquipmentId>83695</ns1:DatEquipmentId>
                                        <ns1:Description>Motor 1,6 Ltr. - 72 kW 16V KAT</ns1:Description>
                                        <ns1:ConstructionTimeFrom>1</ns1:ConstructionTimeFrom>
                                    </ns1:EquipmentPosition>
                                </ns1:EquipmentPositions>
                                <ns1:Orderable>true</ns1:Orderable>
                            </ns1:SparePartPosition>
                        </ns1:SparePartPositions>
                    </ns1:Dossier>
                    <ns1:Dossier>
                        <ns1:Country>DE</ns1:Country>
                        <ns1:Language>de</ns1:Language>
                        <ns1:Vehicle>
                            <ns1:DatECode>015800030020008</ns1:DatECode>
                            <ns1:VehicleTypeName>Pkw, SUV, Kleintransporter</ns1:VehicleTypeName>
                            <ns1:ManufacturerName origin="dat">MINI</ns1:ManufacturerName>
                            <ns1:BaseModelName origin="dat">Mini (R56)(2006-&gt;)</ns1:BaseModelName>
                            <ns1:SubModelName origin="dat">One</ns1:SubModelName>
                            <ns1:Equipment>
                                <ns1:SeriesEquipment/>
                            </ns1:Equipment>
                            <ns1:DATECodeEquipment>
                                <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>75904</ns1:DatEquipmentId>
                                    <ns1:Description>Getriebe Automatik - mit Steptronic (6-Stufen)</ns1:Description>
                                </ns1:EquipmentPosition>
                                <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>10003</ns1:DatEquipmentId>
                                    <ns1:Description>Karosserie: 3-türig</ns1:Description>
                                </ns1:EquipmentPosition>
                                <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>96515</ns1:DatEquipmentId>
                                    <ns1:Description>Motor 1,6 Ltr. - 72 kW 16V</ns1:Description>
                                </ns1:EquipmentPosition>
                            </ns1:DATECodeEquipment>
                        </ns1:Vehicle>
                        <ns1:SparePartPositions>
                            <ns1:SparePartPosition>
                                <ns1:DATProcessId>82526</ns1:DATProcessId>
                                <ns1:DATProcessIdName>ANSAUGLUFT SAUGROHR HALTER H.</ns1:DATProcessIdName>
                                <ns1:PartNumber>11617569966      </ns1:PartNumber>
                                <ns1:Description>STUETZE ANSAUGKRUEMMER</ns1:Description>
                                <ns1:LastUPE>17.83</ns1:LastUPE>
                                <ns1:LastUPEDate>2024-04-01T00:00:00+02:00</ns1:LastUPEDate>
                                <ns1:SecondtoLastUPE>17.83</ns1:SecondtoLastUPE>
                                <ns1:SecondtoLastUPEDate>2024-03-01T00:00:00+01:00</ns1:SecondtoLastUPEDate>
                                <ns1:ThirdtoLastUPE>17.83</ns1:ThirdtoLastUPE>
                                <ns1:ThirdtoLastUPEDate>2024-02-01T00:00:00+01:00</ns1:ThirdtoLastUPEDate>
                                <ns1:FourthtoLastUPE>17.83</ns1:FourthtoLastUPE>
                                <ns1:FourthtoLastUPEDate>2024-01-01T00:00:00+01:00</ns1:FourthtoLastUPEDate>
                                <ns1:EquipmentPositions>
                                    <ns1:EquipmentPosition>
                                        <ns1:DatEquipmentId>83695</ns1:DatEquipmentId>
                                        <ns1:Description>Motor 1,6 Ltr. - 72 kW 16V KAT</ns1:Description>
                                        <ns1:ConstructionTimeFrom>1</ns1:ConstructionTimeFrom>
                                    </ns1:EquipmentPosition>
                                </ns1:EquipmentPositions>
                                <ns1:Orderable>true</ns1:Orderable>
                            </ns1:SparePartPosition>
                        </ns1:SparePartPositions>
                    </ns1:Dossier>
                    ................................................................
                    <ns1:Dossier>
                        <ns1:Country>DE</ns1:Country>
                        <ns1:Language>de</ns1:Language>
                        <ns1:Vehicle>
                            <ns1:DatECode>015800100100001</ns1:DatECode>
                            <ns1:VehicleTypeName>Pkw, SUV, Kleintransporter</ns1:VehicleTypeName>
                            <ns1:ManufacturerName origin="dat">MINI</ns1:ManufacturerName>
                            <ns1:BaseModelName origin="dat">Clubvan (R55)(2012-&gt;2015)</ns1:BaseModelName>
                            <ns1:SubModelName origin="dat">Cooper</ns1:SubModelName>
                            <ns1:Equipment>
                                <ns1:SeriesEquipment/>
                            </ns1:Equipment>
                            <ns1:DATECodeEquipment>
                                <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>71277</ns1:DatEquipmentId>
                                    <ns1:Description>Radstand 2547 mm</ns1:Description>
                                </ns1:EquipmentPosition>
                                <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>84070</ns1:DatEquipmentId>
                                    <ns1:Description>Motor 1,6 Ltr. - 90 kW 16V KAT</ns1:Description>
                                </ns1:EquipmentPosition>
                                <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>10005</ns1:DatEquipmentId>
                                    <ns1:Description>Karosserie: 5-türig</ns1:Description>
                                </ns1:EquipmentPosition>
                                <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>75205</ns1:DatEquipmentId>
                                    <ns1:Description>Getriebe 6-Gang</ns1:Description>
                                </ns1:EquipmentPosition>
                                <ns1:EquipmentPosition>
                                    <ns1:DatEquipmentId>70600</ns1:DatEquipmentId>
                                    <ns1:Description>Antriebsart: Frontantrieb</ns1:Description>
                                </ns1:EquipmentPosition>
                            </ns1:DATECodeEquipment>
                        </ns1:Vehicle>
                        <ns1:SparePartPositions>
                            <ns1:SparePartPosition>
                                <ns1:DATProcessId>82526</ns1:DATProcessId>
                                <ns1:DATProcessIdName>ANSAUGLUFT SAUGROHR HALTER H.</ns1:DATProcessIdName>
                                <ns1:PartNumber>11617569966      </ns1:PartNumber>
                                <ns1:Description>STUETZE ANSAUGKRUEMMER</ns1:Description>
                                <ns1:LastUPE>17.83</ns1:LastUPE>
                                <ns1:LastUPEDate>2024-04-01T00:00:00+02:00</ns1:LastUPEDate>
                                <ns1:SecondtoLastUPE>17.83</ns1:SecondtoLastUPE>
                                <ns1:SecondtoLastUPEDate>2024-03-01T00:00:00+01:00</ns1:SecondtoLastUPEDate>
                                <ns1:ThirdtoLastUPE>17.83</ns1:ThirdtoLastUPE>
                                <ns1:ThirdtoLastUPEDate>2024-02-01T00:00:00+01:00</ns1:ThirdtoLastUPEDate>
                                <ns1:FourthtoLastUPE>17.83</ns1:FourthtoLastUPE>
                                <ns1:FourthtoLastUPEDate>2024-01-01T00:00:00+01:00</ns1:FourthtoLastUPEDate>
                                <ns1:EquipmentPositions>
                                    <ns1:EquipmentPosition>
                                        <ns1:DatEquipmentId>84070</ns1:DatEquipmentId>
                                        <ns1:Description>Motor 1,6 Ltr. - 90 kW 16V KAT</ns1:Description>
                                        <ns1:ConstructionTimeFrom>1</ns1:ConstructionTimeFrom>
                                    </ns1:EquipmentPosition>
                                </ns1:EquipmentPositions>
                                <ns1:Orderable>true</ns1:Orderable>
                            </ns1:SparePartPosition>
                        </ns1:SparePartPositions>
                    </ns1:Dossier>
                </ns1:Dossiers>
            </result>
        </ns3:getExtPartNoInfoByMfrAndExtPartNoResponse>
    </S:Body>
</S:Envelope>
```
