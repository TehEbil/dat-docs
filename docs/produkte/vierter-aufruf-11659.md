---
title: "vierter Aufruf"
topic_id: "11659"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > interaktive Fahrzeugauswahl > Beispiel einer Fahrzeugauswahl > vierter Aufruf"
---

# vierter Aufruf

Durch die Auswahl des Modells wurden die gefundenen Fahrzeuge auf 99 reduziert. Zur
weiteren Reduktion der Treffermenge wird erneut eine Filteroption hinzugewählt.

- Auswahl der Kraftstoffart Hybrid.  
  ( key: "fuelMethod", value "25" )
- Optionale Aktivierung der Ausgabe der Ausstattungsmatrix.  
  ( "withEquipmentMatrix": true )

Die fortschreitende Filterung schränkt die Trefferanzahl der Fahrzeuge weiter ein.
Sobald diese höchstens 30 beträgt, enthält das Ergebnis zusätzlich die Struktur "vehicles".

Mit diesem Aufruf wird zum ersten Mal das Element "vehicles" ausgegeben. Im Response Header erhalten Sie dann, das ab diesem Zeitpunkt für fünf Minuten gültige Transaktions-Token
"X-DAT-VS-TOKEN". Bitte verwenden Sie dieses Token im Header der nachfolgenden Request! Bitte lesen Sie hierzu auch das Topic [Abrechnung der Transaktionen](#showid/11618 "Abrechnung der Transaktionen").
