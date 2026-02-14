---
title: "Beschreibung Zusatzelement 2"
topic_id: "2834"
breadcrumb: "Datenlieferungen > Satzbeschreibung DAT €uropa-Code > Beschreibung Zusatzelement 2"
---

# Beschreibung Zusatzelement 2

Spezifische Ersatzteilbenennung über DVN

Das Zusatzelement 2 liefert die Datenverarbeitungsnummern (DVN) der DAT-spezifischen
Ersatzteilbenennung zu einem Haupttyp.

Bei den DVNs wird ein Satz pro Haupttyp – DVN ausgegeben.

DVN-Benennungen aus dem Typenheft und der Wartung haben, da sie spezifischer sind,
Vorrang vor denen aus der DVN-Stammtabelle.

Der Name des XML-Root-Elements lautet „zusatz2" und der Name eines Satz-Elements lautet
„zusatz2\_s".

Damit Informationen, die vom Haupttyp (HT) abhängig sind, nicht wiederholt werden
müssen, gibt es zusätzlich eine Haupttyp-Stammdatendatei. Der Name des entsprechenden
XML-Root-Elements lautet „zusatz2\_ht" und der Name eines Satz-Elements lautet „zusatz2\_ht\_s".

Als Voraussetzung für die Nutzung des Zusatzelements 2 gilt, dass zuvor eine Fahrzeugidentifikation
auf Basis des DAT €uropa-Codes® im Kombination mit dem Zusatzelement 1 durchgeführt
wurde.
