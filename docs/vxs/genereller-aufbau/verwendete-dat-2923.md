---
title: "Verwendete Datentypen"
topic_id: "2923"
breadcrumb: "Datenaustauschformat VXS > Genereller Aufbau > Verwendete Datentypen"
---

# Verwendete Datentypen

VXS hält sich an die üblichen XML-Datentypen (xsd:dateTime, xsd:decimal, etc.).

| Datentyp | xsd-Basis | Beschreibung |
| --- | --- | --- |
| string | xsd:string | Beliebige Zeichenfolgen |
| decimal | xsd:decimal | Gleitkommazahlen mit Dezimalpunkt (z.B. 123.45) |
| long | xsd:long | Ganzzahlen (z.B. 4711) |
| boolean | xsd:boolean | Schalter, „true" oder „false" |
| dateTime | xsd:dateTime | Datum und Zeit im ISO-Standard (z.B. 1998-07-06T05:04:03.210+02:00) |
| date | xsd:date | Datum im ISO-Standard (z.B. 1998-07-06+02:00) |
| binary | xsd:base64Binary | Binäre Daten in Base64-Kodierung (z.B. Bilder) |
