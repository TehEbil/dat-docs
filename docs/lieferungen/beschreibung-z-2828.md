---
title: "Beschreibung Zusatzelement 4"
topic_id: "2828"
breadcrumb: "Datenlieferungen > Satzbeschreibung DAT €uropa-Code > Beschreibung Zusatzelement 4"
---

# Beschreibung Zusatzelement 4

Eine ausführlichere Beschreibung der SVG-Dateien inklusive Beispielen zur Verarbeitung
der Grafiken finden Sie im DAT Developers Guide, [SVG in den DAT Anwendungen](#showid/1551 "SVG in den DAT Anwendungen").

Zusatzelement 4 bietet die Möglichkeit, FI-Grafiken als sensitive Grafiken darzustellen,
um z.B. die FI- Teilauswahl für die FI-Kalkulation zu ermöglichen.

Zusatzelement 4 beinhaltet alle in FI vorhandenen Baugruppen, die den Status = ‚PRODUKTION’
besitzen. Die Baugruppen werden als gezippte SVG-Dateien - als Vektor- oder Pixelgrafiken
- ausgeliefert.

Die Auslieferung des Zusatzelement 4 ist unterteilt: Die Dateninformationen werden
in einer xml-Datei ausgeliefert, zu jedem Datensatz in dieser xml-Datei existiert
eine Bilddatei im SVG-Format. Der Name der xml-Datei lautet svgdescription.xml. Der Name der Bilddatei setzt sich aus folgender Syntax zusammen:

FZA\_HST\_HT\_BG.svg

Legende:

FZA = Fahrzeugart

HST = Hersteller

HT = Haupttyp

BG = Baugruppen-ID

Beispiel:

01\_340\_005\_01.svg

Bitte beachten Sie, dass die SVG-Bilder in den bereits gezippten "Zusatzelement4"-Ordner ebenfalls gezippt sind, weshalb
Sie nach dem Download des Ordners folgende Schritte befolgen müssen:  
- Ordner "zusatz4" entzippen  
- SVG-Dateien in .zip umbenennen  
- Die Dateien erneut entzippen  
- Die Dateien wieder in .svg umbenennen

Beispielgrafik:

Copyright 2010 Deutsche Automobil Treuhand GmbH. Alle Rechte vorbehalten. Alle Texte,
Bilder, Grafiken und sonstige Dateien unterliegen dem Urheberrecht und anderen Gesetzen
zum Schutz geistigen Eigentums. Sie dürfen weder für Handelszwecke oder zur Weitergabe
kopiert, noch verändert und veröffentlicht verwendet werden.
