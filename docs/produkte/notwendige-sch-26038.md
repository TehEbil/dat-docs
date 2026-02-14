---
title: "Notwendige Schritte SilverDAT 3 Mietwagenspiegel Oberflächenintegration"
topic_id: "26038"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Integration der Oberfläche > Notwendige Schritte SilverDAT 3 Mietwagenspiegel Oberflächenintegration"
---

# Notwendige Schritte SilverDAT 3 Mietwagenspiegel Oberflächenintegration

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

  - https://www.datgroup.com/rentalPrices/app/js/external.js
- Implementierung der JavaScript Methoden:

  - Initialisierung

    - Vorgabe der Host-URL
    - Übergabe der Authentifizierungsinformationen
    - Aufbereitung der Eingabeparameter
  - Fehlerbehandlung
  - Aufruf des Produkts SilverDAT 3 Mietwagenspiegel Oberfläche

Das gewünschte Design können Sie im Head-Tag zum Beispiel mittels eines Bereichs für Stylesheet-Formatdefinitionen festlegen.
Im Anschluss muss zwingend die JavaScript-Datei external.js inkludiert werden. Die Datei external.js stellt ein globales JavaScript-Objekt namens rentalPricesExternal zur Verfügung. Dieses Objekt wird nachfolgend für alle Interaktionen mit SilverDAT 3 Mietwagenspiegel benutzt.
