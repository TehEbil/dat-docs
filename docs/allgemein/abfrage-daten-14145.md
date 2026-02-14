---
title: "Abfrage Daten: getData"
topic_id: "14145"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > Authentifizierung der SilverDAT Webservices > Delegated Sign On (DSO) Service > Abfrage Daten: getData"
---

# Abfrage Daten: getData

Die Funktion liefert ein base64-codiertes und asymmetrisch verschlüsseltes JSON-Objekt
zurück.

Bei dem Funktionsaufruf ist der von der DAT dynamisch erzeugte und an den DSO-Partner
übergebene Token als Parameter "dsoToken" zu übergeben.

Der decodierte und entschlüsselte Inhalt ist ein anonymes JSON-Objekt mit DAT-Kunden-
und -Benutzerinformationen.

Der Inhalt des JSON-Objektes wird mit den DSO-Partnern vereinbart.
