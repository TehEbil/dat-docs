---
title: "erster Aufruf"
topic_id: "11430"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > interaktive Fahrzeugauswahl > Beispiel einer Fahrzeugauswahl > erster Aufruf"
---

# erster Aufruf

Begonnen wird in der Regel mit einem Aufruf lediglich mit den Pflichtfeldern. Dazu
gehört der Parameter locale und restriction. Da die interaktive Fahrzeugauswahl nur für bewertbare Fahrzeuge funktioniert, ist
die restriction immer APPRAISAL.

- Suche nach Fahrzeugen im Markt Deutschland, Ausgabe der Daten in deutsch.  
  ( "locale": ... )

Es werden nur Fahrzeuge der Fahrzeugart 1 (PKW, SUV, Transporter) zur Auswahl berücksichtigt.  
( "allowedVehicleTypes": [1] )

Die Ausgabe (Response) enthält alle möglichen Auswahlfelder mit den möglichen Auswahlen. Mit den jetzigen
Aufrufparametern gibt es nur für die Hersteller Vorschläge für die Auswahl.

Es kann nun dem Anwender diese Liste der Hersteller zur Auswahl angeboten werden.
