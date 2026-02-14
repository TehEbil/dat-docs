---
title: "Notwendige Schritte"
topic_id: "2237"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Integration der Oberfläche > Notwendige Schritte"
---

# Notwendige Schritte

Für den Aufruf wird eine neue oder bestehende HTML-Seite mit JavaScript-Code benötigt.
Diese HTML-Seite stellt die grundlegende und zwingend benötigte HTML-Struktur bereit.
Es ist unerheblich, ob es sich um eine statische HTML-Seite oder um ein dynamisch
erzeugtes HTML-Konstrukt (beispielsweise bei Einsatz von ASP.Net, PHP, JSP, JSF etc.) handelt.

Zur Integration wird im Detail benötigt:

- Bereitstellung des typischen HTML-Grundgerüsts

  - Head
  - Body
  - gegebenenfalls eigene Inhalte und Steuerelemente
- Inkludierung der JavaScript-Datei von www.datgroup.com

  https://www.datgroup.com/FinanceLine/financeline/js/externalSphinxFL.js
- Implementierung der JavaScript Methoden:

  - Initialisierung

    - Einstellen der DAT-Ziel-Umgebung
    - Vorgabe der Host-URL
    - Übergabe der Authentifizierungsinformationen
    - Aufbereitung der Eingabeparameter
  - Fehlerbehandlung
  - Verarbeitung einer abgeschlossenen Bewertung
  - Export der Dossierdaten VXS
  - Aktion nach dem Export der Dossierdaten VXS
  - Aufruf der SilverDAT 3 valuateFinance Oberfläche

Das gewünschte Design können Sie im Head-Tag zum Beispiel mittels eines Bereichs für Stylesheet-Formatdefinitionen festlegen.
Im Anschluss muss zwingend die JavaScript-Datei externalSphinxFL.js inkludiert werden. Die Datei externalSphinxFL.js stellt dabei ein globales JavaScript-Objekt namens sphinx zur Verfügung. Dieses Objekt wird nachfolgend für alle Interaktionen mit SilverDAT 3 valuateFinance benutzt.
