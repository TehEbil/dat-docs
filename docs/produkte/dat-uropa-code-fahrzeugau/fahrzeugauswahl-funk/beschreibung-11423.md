---
title: "Beschreibung"
topic_id: "11423"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > interaktive Fahrzeugauswahl > Beschreibung"
---

# Beschreibung

Durch Verwendung der Schnittstellenfunktion executeVehicleSelectionInteractive kann eine interaktive Fahrzeugauswahl implementiert werden. Für eine Fahrzeugauswahl
über den klassischen Suchbaum müssen ca. 15 verschiedene Schnittstellenfunktionen
aufgerufen werden. Für die interaktive Fahrzeugauswahl genügt eine einzige Schnittstellenfunktion.
Diese Funktion muss mehrfach aufgerufen werden, um zu einem Fahrzeug zu gelangen.
Die Komplexität des Schnittstellenaufrufs hat dadurch etwas zugenommen. Aber mit einem
generischen Ansatz kann im Frontend mit wenigen Zeilen Code die Basis für eine interaktive
Fahrzeugauswahl geschaffen werden.

Die Schnittstellenfunktion zur interaktiven Fahrzeugauswahl ist ausschließlich über
REST verfügbar und befindet sich in unserem VehicleSelectionService. Sie ist nur für bewertbare Fahrzeuge verfügbar. Sobald ein DAT €uropa-Code® aus einem Aufruf resultiert, entstehen Kosten (siehe [Abrechnung der Transaktionen](abrechnung-der-11618.md)).

Grundsätzlicher Ablauf

Die Schnittstellenfunktion zur interaktiven Fahrzeugauswahl muss mehrfach aufgerufen
werden. In der Regel verwendet der erste Aufruf lediglich die Parameter locale und restriction. Hiermit wird die Sprache und der Zielmarkt festgelegt. Als Antwort werden dann alle
für den nächsten Schnittstellenaufruf verfügbaren Filteroptionen zurückgeliefert.
Der Anwender übernimmt eine dieser Optionen und ruft die Schnittstellenfunktion erneut
auf. Es werden die für diese Filterung noch verbleibenden Optionen aus Antwort geliefert,
und der Anwender übernimmt eine weitere davon, und so weiter. Letztendlich wird durch
diesen iterativen Prozess, bei dem immer wieder eine eine zusätzliche Filteroption
Verwendung findet, die Menge der zutreffenden Fahrzeuge immer weiter reduziert. Sobald
die Anzahl 20 Fahrzeuge oder weniger ist, kann der Anwender direkt konkrete Fahrzeuge
mit DAT €uropa-Code® und Marktindex auswählen. Ist nicht ersichtlich, welches der Fahrzeuge das richtige
ist, können weitere Filteroptionen gewählt werden, bis nur noch ein Fahrzeug übrig
bleibt.
