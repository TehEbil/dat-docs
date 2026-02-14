---
title: "Definition XML-Schema"
topic_id: "1567"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > Arbeiten mit den Webservices > Definition XML-Schema"
---

# Definition XML-Schema

Die Definition der XML-Schemata erfolgt unter Aufteilung der Elemente auf mehrere
XMLSchema-Dateien (Dateiendung .xsd). Im Regelfall gibt es jeweils ein Schema

- zur Beschreibung der Schnittstellenfunktionen und
- zur Beschreibung der verwendeten Datentypen.

Die Pfade zu den Schemata finden Sie in der jeweiligen WSDL, im Element <types>. Über diesen Link können Sie sich die Schemata auch ansehen:

```
<types> 
<xsd:schema> 
<xsd:import namespace="http://www.dat.de/vxs"
 schemaLocation="http://www.dat.de/GlassRep/services/DMSGetContracts?xsd=1" /> 
</xsd:schema> 
<xsd:schema> 
<xsd:import namespace="http://sphinx.dat.de/services/GlassRep"
 schemaLocation="http://www.dat.de/GlassRep/services/DMSGetContracts?xsd=2" /> 
</xsd:schema> 
</types>
```
