---
title: "Namensräume und Präfixe"
topic_id: "1574"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > Arbeiten mit den Webservices > XML Definition > Namensräume und Präfixe"
---

# Namensräume und Präfixe

Ein XML-Namensraum wird benutzt, um das Vokabular eines XML-Dokumentes eindeutig zu
identifizieren. Namensräume werden durch Uniform Resource Identifier (URI) dargestellt,
meistens also durch normale Webadressen, die allerdings nicht existieren müssen.

- Namensraumangaben sind Case-sensitiv.
- Für Namensräume wird das Attribut xmlns (engl. Namespace) verwendet.
- Für Namensräume existiert ein Präfix-Mechanismus: Elemente werden durch eine Zeichenkette,
  die durch einen Doppelpunkt vom Elementnamen getrennt wird, in einen beliebigen Namensraum
  gesetzt werden. Das Präfix muß zuerst an den Namensraum gebunden werden. Im folgenden
  Beispiel ist das Präfix 'glas':

```
<html xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:glas="http://sphinx.dat.de/services/GlassRep"
 xmlns:dms="http://sphinx.dat.de/services/DMSGetContracts">
```

Bitte beachten Sie bei der Benutzung unserer Webservcies: Jedes unserer Produkte bringt
seine eigenen Namensräume mit.
