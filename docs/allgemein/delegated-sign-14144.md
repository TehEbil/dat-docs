---
title: "Delegated Sign On (DSO) Service"
topic_id: "14144"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > Authentifizierung der SilverDAT Webservices > Delegated Sign On (DSO) Service"
---

# Delegated Sign On (DSO) Service

Die Nutzung des Delegated Sign On (DSO) Service steht ausschließlich DSO-Partnern zur Verfügung.

Der Service bietet die Möglichkeit, DSO-Partner-spezifische Hashwerte der DAT-Kundennummer
und -Benutzer-ID DSO-Partnern zur Verfügung zu stellen. Hierbei wird das DAT-Benutzerpasswort
nicht an den DSO-Partner weitergegeben.

DSO-Partner können die Informationen verwenden, um zum Beispiel eine automatische
Benutzeranmeldung umzusetzen.

Die DSO-Partnerspezifischen Hash-Werte können vom DSO-Partner in selbst entwickelten
Funktionen verwendet werden, z.B. zur Zuordnung von DAT-Benutzern zu vorhandenen DSO-eigenen
Benutzern sowie zur automatischen Anmeldung.

Generelle Funktionsweise:

- DAT übermittelt den dsoToken an die vereinbarte URL des DSO-Partners
- DSO-Partner ruft den DSO-Webservice-Funktion getData auf und übergibt den dsoToken
- DAT prüft die Gültigkeit des dsoTokens

  - Falls der dsoToken ungültig ist: Fehler
  - Sonst:

    - Erzeugung JSON-Objekt mit den Daten, die mit dem DSO-Partner vereinbart wurden
    - Verschlüsselung des JSON-Objektes mit einem DSO-Partner- und umgebungsspezifischen
      publicKey
    - Base64-Codierung des verschlüsselten JSON-Objektes
    - Rückgabe des Base64-codierten und verschlüsselten JSON-Objektes an den DSO-Partner
- DSO-Partner

  - Falls Fehler: DSO-Partnerspezifische Fehlerbehandlung, z.B.

    - Fehlermeldung
    - Redirect auf DAT-Startseite
  - Sonst: Decodierung des Base64-codierte und verschlüsselten JSON-Objektes mit einem
    DSO-Partner- und umgebungsspezifischen privateKey

Seitens des DSO-Partners sind gegebenenfalls eigene Funktionen umzusetzen, beispielsweise:

- Prüfung, ob Benutzer mit DAT-Kunden-Hashwert und DAT-Benutzer-Hashwert in eigener
  Anwendung und Umgebung bereits vorhanden

  - Falls vorhanden: automatische Anmeldung
  - Sonst:

    - Zuordnung zu bereits vorhandenem DSO-Benutzer (sofern vorhanden)
    - oder Neuanlage mit Speicherung der DAT-Kunden-Hashwert und DAT-Benutzer-Hashwert
    - Anmeldung

Wichtige Hinweise:

- Nur der DSO-Partner verfügt über die privateKeys zur Entschlüsselung der Daten
- Die DAT erhält ausschließlich die publicKeys zur Verschlüsselung der Daten
- Gültigkeit des dsoTokens:

  - 30 Minuten
  - Einmal verwendbar

DSO-Webservice-URL: https://www.dat.de/AuthorizationManager/dso
