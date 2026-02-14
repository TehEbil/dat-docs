---
title: "Entfernung des doppelten Elements ResidualWarrantyValueGross aus TradingServiceN_schema1.xsd"
topic_id: "31079"
breadcrumb: "Technische Informationen > Ausgabe Nr. 93 September 2025 > Fahrzeugbewertung > SilverDAT 3 PRO > Abkündigungen > Entfernung des doppelten Elements ResidualWarrantyValueGross aus TradingServiceN_schema1.xsd"
---

# Entfernung des doppelten Elements ResidualWarrantyValueGross aus TradingServiceN_schema1.xsd

###### Entfernung des doppelten Elements ResidualWarrantyValueGross aus TradingServiceN\_schema1.xsd

Mit dem Dezember Release 2025 wird es eine Anpassung in der schema-Datei https://www.dat.de/myClaim/soap/v2/TradingServiceN\_schema1.xsd geben.

Die doppelten Elemente von ResidualWarrantyValueGross unter purchaseDataResponse und admissionDataResponse werden entfernt.

Auszug aus der schema-Datei:

```
<xs:complexType name="purchaseDataResponse">
   <xs:complexContent>
      <xs:extension base="tns:purchaseData">
         <xs:sequence>
            <xs:element name="ResidualWarrantyValueGross" type="xs:decimal" minOccurs="0"/>
         </xs:sequence>
      </xs:extension>
   </xs:complexContent>
</xs:complexType>
```

```
<xs:complexType name="purchaseData">
   <xs:complexContent>
      <xs:extension base="tns:commonData">
         <xs:sequence>
            <xs:element name="PurchaseDate" type="xs:dateTime"/>
            <xs:element name="PurchasePriceNet" type="xs:decimal"/>
            <xs:element name="MileageExpected" type="xs:int"/>
            <xs:element name="PurchasePriceGross" type="xs:decimal"/>
            <xs:element name="ResidualWarrantyValueGross" type="xs:decimal"/>
         </xs:sequence>
      </xs:extension>
   </xs:complexContent>
</xs:complexType>
```

```
<xs:complexType name="admissionDataResponse">
   <xs:complexContent>
      <xs:extension base="tns:admissionData">
         <xs:sequence>
            <xs:element name="ResidualWarrantyValueGross" type="xs:decimal" minOccurs="0"/>
         </xs:sequence>
      </xs:extension>
   </xs:complexContent>
</xs:complexType>
```

```
<xs:complexType name="admissionData">
   <xs:complexContent>
      <xs:extension base="tns:commonData">
         <xs:sequence>
            <xs:element name="AdmissionDate" type="xs:dateTime"/>
            <xs:element name="AdmissionPriceNet" type="xs:decimal"/>
            <xs:element name="MileageOdometer" type="xs:int" minOccurs="0"/>
            <xs:element name="MileageVehicle" type="xs:int"/>
            <xs:element name="Location" type="xs:string" minOccurs="0"/>
            <xs:element name="AdmissionPriceGross" type="xs:decimal"/>
            <xs:element name="ResidualWarrantyValueGross" type="xs:decimal"/>
            <xs:element name="Labelling" type="tns:labellingData" minOccurs="0"/>
         </xs:sequence>
      </xs:extension>
   </xs:complexContent>
</xs:complexType>
```

Zukünftig sollen purchaseDataResponse und admissionDataResponse folgendermaßen aussehen:

```
<xs:complexType name="purchaseDataResponse">
   <xs:complexContent>
      <xs:extension base="tns:purchaseData">
      </xs:extension>
   </xs:complexContent>
</xs:complexType>
```

```
<xs:complexType name="admissionDataResponse">
   <xs:complexContent>
      <xs:extension base="tns:admissionData">
      </xs:extension>
   </xs:complexContent>
</xs:complexType>
```
