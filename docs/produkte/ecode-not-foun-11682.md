---
title: "ECode not found  - Datenkarte"
topic_id: "11682"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Fahrzeugidentifikation anhand VIN (VIN-Abfrage) > ECode not found  - Datenkarte"
---

# ECode not found  - Datenkarte

##### ECode not found - Datenkarte

Fehlermeldungen können unter Umständen wichtige Informationen enthalten. Im Ergebnis
einer VIN-Abfrage ist die Fehlermeldung "ECode not found" ein solcher Fall, darin ist die sogenannte Datenkarte enthalten. Es lohnt sich diese
genauer zu betrachten und die darin enthaltenen Informationen gegebenenfalls weiterzuverarbeiten.

Ursache

Immer wenn anhand der Daten vom Hersteller in den DAT Fahrzeugdaten kein vollständiger
DAT €uropa-Code® zugeordnet werden kann, erfolgt diese Fehlermeldung.

Fehlermeldung

```
<S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <S:Fault>
         <faultcode xmlns:dat="http://www.dat.de">dat:dat:Server.valueNotFound</faultcode>
         <faultstring><![CDATA[ECode not found <additionalInformation><ns2:Vehicle> ... </ns2:Vehicle></additionalInformation>]]></faultstring>
         <faultactor>de.dat.sphinx.vehicleselection.ws.n.VehicleIdentificationService</faultactor>
      </S:Fault>
   </S:Body>
</S:Envelope>
```

Hinter der Meldung "ECode not found" steckt in <additionalInformation> ein Vehicle Objekt im bekannten VXS-Format. Darin sind alle Informationen vom Hersteller sowie alle zugeordneten DAT Schlüssel
enthalten.

In den Folgenden Abschnitten zwei Beispiele für Situationen in denen die Informationen
in der Fehlermeldung durchaus wertvoll sein können.
