---
title: "Beispiel VXS-Datei Auftragseröffnung"
topic_id: "2070"
breadcrumb: "SilverDAT Produkte > Autoglas Plus SilverDAT inside + SilverDAT calculateGlass > Aufruf der Anwendungsoberfläche über Schnittstelle > Beispiel VXS-Datei Auftragseröffnung"
---

# Beispiel VXS-Datei Auftragseröffnung

```
<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
<!-- für Import aus Nissan Glas --> 
<VXS:Dossiers source="SD3" type="glassrep.nsg" xmlns:VXS="http://www.dat.de/vxs">
    <VXS:Dossier>
        <VXS:DatCustomerId>0000000</VXS:DatCustomerId>
        <VXS:VAT><VXS:VatAtCalculationTime>19</VXS:VatAtCalculationTime></VXS:VAT>
        <VXS:TradingData>
                <VXS:Owner>
                    <VXS:CompanyName>Sabin</VXS:CompanyName>
                    <VXS:Title>titleCom</VXS:Title>
                    <VXS:Country>D</VXS:Country>
                    <VXS:VatEntitled>false</VXS:VatEntitled>
                    <VXS:Street>Hellmuth-Hirth-Straße</VXS:Street>
                    <VXS:StreetZipCode>73760</VXS:StreetZipCode>
                    <VXS:StreetCity>Ostfildern-Scharnhauser Park</VXS:StreetCity>
                    <VXS:StreetNumber>1</VXS:StreetNumber>
                    <VXS:EMail>Cenui.Sabin@dat.de</VXS:EMail>
                    <VXS:PhonePersonal>+4971146503757</VXS:PhonePersonal> 
                </VXS:Owner>
            </VXS:TradingData>
            <VXS:RepairCalculation>
                    <VXS:Comment>Hier eine Bemerkung</VXS:Comment>
                    <VXS:Vehicle>
                        <VXS:VehicleIdentNumber>WAUZZZ8E62A234056</VXS:VehicleIdentNumber>
                        <VXS:MileageOdometer>60000</VXS:MileageOdometer>
                        <VXS:InitialRegistration>2007-12-24</VXS:InitialRegistration>
                        <VXS:RegistrationData>
                            <VXS:LicenseNumber>ES J 1500</VXS:LicenseNumber>
                        </VXS:RegistrationData>
                    </VXS:Vehicle>
            </VXS:RepairCalculation>
            <VXS:RepairOrder>
            <VXS:DamageDate>2009-12-24T01:00:00+01:00</VXS:DamageDate>
            <VXS:RepairCoverage>Complete</VXS:RepairCoverage>
            <VXS:OrderNumber>TWI4</VXS:OrderNumber>
            <VXS:Retention>true</VXS:Retention>
            <VXS:RetentionAmount>300</VXS:RetentionAmount>
            <VXS:InsuranceId>5</VXS:InsuranceId>
            <VXS:DamageNumber>9999999999</VXS:DamageNumber>
            <VXS:PolicyNumber>999999999999999</VXS:PolicyNumber>
            <VXS:DeclarationOfAssignment>true</VXS:DeclarationOfAssignment>
        </VXS:RepairOrder>
    </VXS:Dossier>
</VXS:Dossiers>
```
