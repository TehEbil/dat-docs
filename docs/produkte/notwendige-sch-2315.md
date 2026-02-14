---
title: "Notwendige Schritte SilverDAT 3 valuateExpert Oberflächenintegration"
topic_id: "2315"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Integration der Oberfläche > Notwendige Schritte SilverDAT 3 valuateExpert Oberflächenintegration"
---

# Notwendige Schritte SilverDAT 3 valuateExpert Oberflächenintegration

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

  - https://www.datgroup.com/valuateNG/app/js/external.js
- Implementierung der JavaScript Methoden:

  - Initialisierung

    - Vorgabe der Host-URL
    - Übergabe der Authentifizierungsinformationen
    - Aufbereitung der Eingabeparameter
  - Fehlerbehandlung
  - Verarbeitung eines abgeschlossenen Vorgangs
  - Export der Dossierdaten VXS
  - Aktion nach dem Export der Dossierdaten VXS
  - Aufruf der SilverDAT 3 valuateExpert/PlusPartner Oberfläche

Das gewünschte Design können Sie im Head-Tag zum Beispiel mittels eines Bereichs für Stylesheet-Formatdefinitionen festlegen.
Im Anschluss muss zwingend die JavaScript-Datei external.js inkludiert werden. Die Datei external.js stellt ein globales JavaScript-Objekt namens valuateNGExternal zur Verfügung. Dieses Objekt wird nachfolgend für alle Interaktionen mit SilverDAT 3 valuateExpert/PlusPartner benutzt.
