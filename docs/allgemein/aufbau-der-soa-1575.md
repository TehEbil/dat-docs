---
title: "Aufbau der SOAP-Nachrichten bezogen auf das Produkt"
topic_id: "1575"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > Arbeiten mit den Webservices > Aufbau der SOAP-Nachrichten bezogen auf das Produkt"
---

# Aufbau der SOAP-Nachrichten bezogen auf das Produkt

Bei Verständnisschwierigkeiten mit diesem Kapitel, lesen Sie bitte zuerst das Kapitel
"[Definition XML](#showid/1569 "XML Definition ")".

Eine minimale SOAP-Nachricht besteht aus einem Envelope genannten Element, dem ein lokaler Name zugewiesen werden muss. Dieses Element referenziert
üblicherweise mittels eines Namensraum-Attributes auf "http://schemas.xmlsoap.org/soap/envelope/".
Außerdem verwenden wir Namensräume, die wir mithilfe von Präfixen setzen:

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:glas="http://sphinx.dat.de/services/GlassRep" xmlns:vxs="http://www.dat.de/vxs"
 xmlns:dms="http://sphinx.dat.de/services/DMSCreateContract">
```

Kind dieses Elements muss ein Body-Element sein. Optional kann zuvor ein Header-Element
stehen. In diesem können Meta-Informationen, beispielsweise zum Routing, zur Verschlüsselung
oder zu Transaktionsidentifizierung, untergebracht werden.

Header-Element

Üblicherweise übergeben wir in unseren SOAP-Nachrichten ein Header-Element, das eine Komponente des Frameworks JBoss Seam wiedergibt; die conversationId. Die Benutzung der conversationId löst zwei Probleme beim Speichern von Objekten in Sessions:

1. Ein Objekt bleibt mit dem Session-Kontext solange im Speicher, bis die Session aus
   technischen Gründen ausläuft oder das Objekt explizit entfernt wird. Vergisst der
   Entwickler, das Objekt an geeigneter Stelle aus der Session zu entfernen, entsteht
   ein Speicherleck.
2. Alle Browserfenster bzw. -tabs eines Computers teilen sich dieselbe Session. Das kann,
   aus Sicht des Benutzers, zu unerwartetem Verhalten bei mehreren geöffneten Fenstern
   führen, da für alle Fenster dasselbe Objekt benutzt wird.

Durch die Übergabe der conversationId ist es also möglich, einem Benutzer zu erlauben, mehr als ein Fenster mit derselben
Session zu öffnen:

```
<S:Header>
<seam:conversationId xmlns:seam="http://www.jboss.org/seam/webservice">3252</seam:conversationId>
</S:Header>
```

Body-Element

Im Body-Element sind die eigentlichen Nutzdaten untergebracht. Innerhalb des Body-Elements
können sowohl Informationen zum Datenaustausch, als auch Anweisungen für einen entfernten
Prozeduraufruf stehen. Dies ist vom Empfänger entsprechend zu interpretieren.

Struktur einer SOAP-Nachricht:

```
      <?xml version="1.0"?>
      <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
       <soapenv:Header>
       </soapenv:Header>
         <soapenv:Body>
       <!--request -->
         </soapenv:Body>
      </soapenv:Envelope>
```
