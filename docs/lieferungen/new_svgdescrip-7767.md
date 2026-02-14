---
title: "NEW_svgdescription-xsd"
topic_id: "7767"
breadcrumb: "Datenlieferungen > Satzbeschreibung DAT €uropa-Code > Beschreibung Zusatzelement 4 > NEW_svgdescription-xsd"
---

# NEW_svgdescription-xsd

#### NEW\_svgdescription-xsd

```
<?xml version="1.0" encoding="UTF-8"?>
<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema" elementFormDefault="qualified"
 attributeFormDefault="unqualified">
    <xs:element name="constructiongroups" type="constructiongroupsType"/>
    <!-- Baugruppe  -->
    <xs:complexType name="constructiongroupType">
        <xs:sequence>
            <!-- Fahrzeugart  -->
            <xs:element name="fza" type="xs:byte"/>
            <!-- Hersteller  -->
            <xs:element name="hst" type="xs:short"/>
            <!-- haupttyp  -->
            <xs:element name="ht" type="xs:short"/>
            <!-- Baugruppe ID  -->
            <xs:element name="constructiongroupid" type="xs:short"/>
            <!-- Baugruppenbenennungen  -->
            <xs:element name="constructionGroupNames" type="langsType"/>
            <!-- SVG-Dateiname -->
            <xs:element name="filename" type="xs:string"/>
        </xs:sequence>
    </xs:complexType>
    <xs:complexType name="constructiongroupsType">
        <xs:sequence>
            <xs:element name="constructiongroup" type="constructiongroupType" minOccurs="0"
 maxOccurs="unbounded"/>
        </xs:sequence>
    </xs:complexType>
    <xs:complexType name="langType">
        <xs:simpleContent>
            <xs:extension base="xs:string">
                <xs:attribute name="language" type="xs:string" use="optional"/>
                <xs:attribute name="country" type="xs:string" use="optional"/>
            </xs:extension>
            <!-- sprache -->
            <!-- land -->
        </xs:simpleContent>
    </xs:complexType>
    <xs:complexType name="langsType">
        <xs:choice minOccurs="0" maxOccurs="unbounded">
            <xs:element name="lang" type="langType"/>
        </xs:choice>
    </xs:complexType>
</xs:schema>
```
