---
title: "Definition Webservice"
topic_id: "1565"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > Arbeiten mit den Webservices > Definition Webservice"
---

# Definition Webservice

Webservice

Ein Webservice hat ein Interface, das mit der Webservice-Definition Language (WSDL) spezifiziert wird. Die WSDL dient dazu, die Schnittstellen und Funktionalitäten eines Webservices zu beschreiben.

Ein Webservice ist ein Dienst, der von externen Anwendungen angesprochen werden kann. Die Kommunikation
findet über das Simple Object Access Protocol (SOAP), einem XML-basierten Protokoll, statt.

Ziele

- Funktionalität unabhängig von Plattformen und Programmiersprachen zur Verfügung stellen
- Funktionalität der Anwendung (weltweit) zur Verfügung stellen
- Wiederverwendbare Application-Komponenten (z.B. Bauzeitkonverter, VIN-Abfrage)
- Bestehende Software verbinden, indem technische Unterschiede überwunden werden

Implementierungen

Ein Webservice kann in jeder Sprache implementiert werden, da der Webservice und der
Client über offene Standards miteinander kommunizieren.

WSDL

Die Web Services Description Language (WSDL) ist eine Metasprache um die angebotenen Funktionen, Daten, Datentypen und Austauschprotokolle
eines Webservice zu beschreiben. Die in diesem Kapitel gezeigten Beispiele zeigen Teile aus dem Webservice zum Produkt autoglas Plus / SilverDAT calculateGlass.

Die WSDL beschreibt

1. wo ein Webservice aufgerufen wird - durch die URI, die protokollspezifische Adresse
2. wie ein Webservice aufgerufen wird - durch Angabe der Datenformate, Parameter etc.
3. was ein Webservice macht - in Form von Schnittstellenfunktionen
4. welches Ergebnis erwartet werden kann - durch Angabe der Rückgabewerte

Aufbau der WSDL

- In der ersten Zeile finden Sie den Prolog. In den nachfolgenden Zeilen wird das Stammelement (definitions) dargestellt. In
  diesem Stammelement werden die Definitionen der verwendeten Namespaces angegeben. So z.B. mit xmlns:xsd die Definition der XML Scheme Definition oder xmlns:soap der Namespace von SOAP:

```
<definitions xmlns:wsu="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-utility-1.0.xsd"
 xmlns:wsp="http://www.w3.org/ns/ws-policy"
 xmlns:wsp1_2="http://schemas.xmlsoap.org/ws/2004/09/policy"
 xmlns:wsam="http://www.w3.org/2007/05/addressing/metadata"
 xmlns:soap="http://schemas.xmlsoap.org/wsdl/soap/" xmlns:tns="http://sphinx.dat.de/services/GlassRep"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.xmlsoap.org/wsdl/"
 targetNamespace="http://sphinx.dat.de/services/GlassRep" name="DMSGetContracts">
...
</definitions>
```

- Innerhalb des Stammelementes befinden sich die sechs XML-Hauptelemente der WSDL, die Sie auch in unseren WSDL wiederfinden können:

  - types (Datentypen)  
    Definition der Datentypen, die zum Austausch der messages benutzt werden. Dies können
    einfache Typen sein (speichern nur einen Wert) oder komplexe Typen, die ein Tupel
    aus einzelnen Werten speichern. Die Typen werden entsprechend der W3C-Spezifikation definiert. Es können daher auch weiterführende Spezifikationen wie
    restrictions (minLength, maxLength usw.) festgelegt werden. Ebenso sind Verweise auf andere Typdefinitionen möglich.
    Der import-Tag erlaubt es, Elemente aus anderen Namensräumen zu importieren, mit einem Präfix
    zu versehen und damit Schema-Bestandteile aus unterschiedlichen Namensräumen wiederzuverwenden.

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

- message (Nachricht)  
  Definition der übermittelten Nachrichten, die zwischen dem Webservice und dem Client hin- und hergeschickt werden können. Eine Message besteht immer aus 1:.n Teil-Knoten, die die enthaltenen Daten spezifizieren. Eine
  Message kann somit als Daten-Container betrachtet werden. Ein Request sowie ein Response erhalten dabei eigene Nachrichten-Definitionen.  
  Der folgende XML-Code spezifiziert zwei mögliche Nachrichten. Zum einen wird die Message für die Anfrage
  der Vorgangsdaten definiert – getContract mit dem Element getContract (ein selbstdefinierter Typ, daher tns für Targetnamespace) – und zum anderen die Nachricht,
  die die Antwort enthält – getContractResponse mit dem selbstdefinierten Element getContractResponse. Der Name muss im gesamten Webservice unique sein.

```
<message name="getContract"> 
<part name="parameters" element="tns:getContract" /> 
</message>
<message name="getContractResponse"> 
<part name="parameters" element="tns:getContractResponse" /> 
</message> 
```

- portType (Schnittstellentypen)  
  portTypes sind die “Andockpunkte” an den Webservice und definieren die Schnittstellen, über die der Webservice kommunizieren kann. Die Definition setzt dabei auf die vorhandenen types und messages
  auf. Ein portType enthält verschiedene Operationen, die wiederum die oben definierten Nachrichten enthalten.
  Der Name einer operation ist standardmäßig der Name der Methode.

```
<portType name="DMSGetContracts"> 
<operation name="getContract"> 
<input wsam:Action="getContract" message="tns:getContract" /> 
<output wsam:Action="http://sphinx.dat.de/services/GlassRep/DMSGetContracts/getContractResponse"
 message="tns:getContractResponse" /> 
</operation>
```

- binding (Bindung)  
  Im binding werden die verwendeten Protokolle (SOAP, HTTP, SMTP), Message-Styles (rpc, document) und das Encoding/Format (literal – message-parts sind bereits in XML und müssen nicht konvertiert werden, SOAP-Encoding) definiert.   
  Unterscheidung document-style und RPC-style: Im RPC-style werden keine eigenen types definiert, sondern die Typen aus dem xsd-Namespace verwendet. In einem SOAP-Envelope ist eine Validierung somit erschwert. Aus diesem Grund kommt bei der Programmierung
  im Grid überwiegend der Document-Style zum Einsatz.

```
<binding name="DMSGetContractsPortBinding" type="tns:DMSGetContracts"> 
<soap:binding transport="http://schemas.xmlsoap.org/soap/http" style="document" /> 
<operation name="getContract"> 
<soap:operation soapAction="getContract" /> 
<input> 
<soap:body use="literal" /> 
</input> 
<output> 
<soap:body use="literal" /> 
</output> 
</operation>
```

- service (Service)  
  Fasst eine Menge von verwandten Ports zusammen. Ein port ist dabei eine Instanz eines portTypes mit einer eigenen Netzwerk-Adresse.

```
<service name="DMSGetContracts"> 
<port name="DMSGetContractsPort" binding="tns:DMSGetContractsPortBinding"> 
<soap:address location="http://www.dat.de/GlassRep/services/DMSGetContracts" /> 
</port> 
</service>
```
