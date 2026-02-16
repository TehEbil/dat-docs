---
title: "Notwendige Schritte"
topic_id: "1852"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Oberflächen-Schnittstelle > Integration der Oberfläche > Notwendige Schritte"
---

# Notwendige Schritte

Es wird eine neue oder bestehende HTML-Seite mit etwas JavaScript-Code benötigt, die
die grundlegende, zwingend benötigte HTML-Struktur bereitstellt. Es ist dabei unerheblich,
ob es sich um eine statische HTML-Seite oder ein dynamisch erzeugtes HTML-Konstrukt
(bspw. bei Einsatz von ASP.Net, PHP, JSP, JSF etc.) handelt.

Zur Integration wird im Detail benötigt:

- Bereitstellung des typischen HTML-Grundgerüsts

  - Head
  - Body
  - (ggfs. eigene Inhalte und Steuerelemente)
- Inkludierung von 2 JavaScript-Dateien von www.dat.de

  - https://www.dat.de/sphinx/js/lazyload.js
  - https://www.dat.de/sphinx/js/externalSphinx.js
- Inkludierung von JavaScript-Datei für Generierung des DAT-AuthorizationToken über
  AJAX

  - https://code.jquery.com/jquery-2.2.4.min.js
- Implementierung von 3 JavaScript Methoden:

  - Sphinx Initialisierung

    - Aufbereitung der Eingabeparameter (optional)
    - Aufbereitung der Authentifizierungsinformationen
    - Initialisierung und Aufruf des JavaScript-Objekts für die Fahrzeugauswahl
  - Callback-Methode für die Verarbeitung einer abgeschlossenen Fahrzeugauswahl
  - Callback-Methode für Fehlerbehandlungen
