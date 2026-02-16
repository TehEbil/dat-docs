---
title: "Darstellung der SVG - XML Schema Definition"
topic_id: "2826"
breadcrumb: "Datenlieferungen > Satzbeschreibung DAT €uropa-Code > Beschreibung Zusatzelement 4 > Erläuterungen zur SVG Schema Definition > Darstellung der SVG - XML Schema Definition"
---

# Darstellung der SVG - XML Schema Definition

```
<?xml version="1.0" encoding="UTF-8"?>
<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema" xmlns:svg="http://www.dat.de/sphinx/svg"
 targetNamespace="http://www.dat.de/sphinx/svg" elementFormDefault="qualified"
 attributeFormDefault="unqualified">
    <xs:element name="text" type="svg:textType"/>
    <xs:element name="objectInfo" type="svg:objectInfoType"/>
    <xs:element name="constructionGroup" type="svg:constructionGroupType"/>
    <xs:complexType name="dvnLeftType">
        <xs:sequence>
            <xs:element name="dvn" type="xs:int"/>
            <xs:element name="etBauart" type="xs:string"/>
            <xs:element name="etBauartOptKz" type="xs:string"/>
            <xs:element name="rcs" type="svg:rcsType"/>
        </xs:sequence>
    </xs:complexType>
    <xs:complexType name="dvnRightType">
        <xs:sequence>
            <xs:element name="dvn" type="xs:int"/>
            <xs:element name="etBauart" type="xs:string"/>
            <xs:element name="etBauartOptKz" type="xs:string"/>
            <xs:element name="rcs" type="svg:rcsType"/>
        </xs:sequence>
    </xs:complexType>
    <xs:complexType name="titleType">
        <xs:sequence>
            <xs:element name="langs" type="svg:langsType"/>
        </xs:sequence>
        <xs:attribute name="stnr" type="xs:int" use="optional"/>
        <xs:attribute name="uebId" type="xs:int" use="optional"/>
    </xs:complexType>
    <xs:complexType name="tooltipType">
        <xs:sequence>
            <xs:element name="langs" type="svg:langsType"/>
        </xs:sequence>
        <xs:attribute name="stnr" type="xs:int" use="optional"/>
        <xs:attribute name="uebId" type="xs:int" use="optional"/>
    </xs:complexType>
    <xs:complexType name="textType">
        <xs:sequence>
            <xs:element name="langs" type="svg:langsType"/>
        </xs:sequence>
        <xs:attribute name="uebId" type="xs:int" use="optional"/>
        <xs:attribute name="stnr" type="xs:int" use="optional"/>
    </xs:complexType>
    <xs:complexType name="objectInfoType">
        <xs:sequence>
            <xs:element name="title" type="svg:titleType"/>
            <xs:element name="tooltip" type="svg:tooltipType"/>
            <xs:element name="text" type="svg:textType"/>
            <xs:element name="dvnGroup" type="xs:byte"/>
            <xs:element name="kzSeite" type="xs:string"/>
            <xs:element name="groups" type="xs:string"/>
            <xs:element name="dvnLeft" type="svg:dvnLeftType" minOccurs="0"/>
            <xs:element name="dvnRight" type="svg:dvnRightType" minOccurs="0"/>
        </xs:sequence>
        <xs:attribute name="position" type="xs:byte" use="optional"/>
    </xs:complexType>
    <xs:complexType name="rcsType">
        <xs:sequence>
            <xs:element name="rc" type="xs:string" minOccurs="0" maxOccurs="unbounded"/>
        </xs:sequence>
    </xs:complexType>
    <xs:complexType name="langType">
        <xs:simpleContent>
            <xs:extension base="xs:string">
                <xs:attribute name="languageCode" type="xs:string" use="optional"/>
                <xs:attribute name="countryCode" type="xs:string" use="optional"/>
                <xs:attribute name="stnr" type="xs:int" use="optional"/>
            </xs:extension>
        </xs:simpleContent>
    </xs:complexType>
    <xs:complexType name="langsType">
        <xs:choice minOccurs="0" maxOccurs="unbounded">
            <xs:element name="lang" type="svg:langType"/>
        </xs:choice>
    </xs:complexType>
    <xs:complexType name="constructionGroupType">
        <xs:sequence>
            <xs:element name="fza" type="xs:byte"/>
            <xs:element name="hst" type="xs:short"/>
            <xs:element name="ht" type="xs:byte"/>
            <xs:element name="constructionGroupId" type="xs:byte"/>
            <xs:element name="lkz" type="xs:string"/>
        </xs:sequence>
    </xs:complexType>
</xs:schema>
```
