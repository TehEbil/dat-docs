---
title: "Fahrzeugauswahl: DAT €uropa-Code® und Container"
topic_id: "1896"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Aufbau einer Fahrzeugauswahl > Fahrzeugauswahl: DAT €uropa-Code® und Container"
---

# Fahrzeugauswahl: DAT €uropa-Code® und Container

Bitte lesen Sie folgende Kapitel und ihre Unterkapitel, bevor Sie hier weiterlesen:  
- das Kapitel [kleiner Exkurs DAT Europa-Code und Marktindex](#showid/1882 "kleiner Exkurs: DAT €uropa-Code® und Marktindex")  
- die Kapitel ab [Fahrzeugauswahl: Der Basistyp](#showid/1885 "Fahrzeugauswahl: Der Basistyp"), Beachten Sie vor allem die Hinweise zu den Abfragen.

Aufbau eines DAT €uropa-Code®, mit Marktindex bestehend aus Container und Bauzeit  
(der Container ist orange dargestellt).

Beispiel einer Fahrzeugauswahl.

Programmier-Beispiel:

```
...
String datECode = sdoClient.compileDatECode(getDatCustomerNo(),
getDatLogin(), getDatPassword(), eCode[0], eCode[1], eCode[2], eCode[3], eqArray);
...
```
