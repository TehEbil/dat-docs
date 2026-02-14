---
title: "Übersicht"
topic_id: "27900"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) 2026 - Schnittstelle zum Datenabruf > Übersicht"
---

# Übersicht

Dieses Dokument spezifiziert die Datenabruf-REST-Schnittstelle des Data Entry Tool
(DET).

Der DET-Datenabrufdienst bietet Funktionen zur Abfrage von Fahrzeugdaten aus der DET-Datenbank.
Es werden nur Lesevorgänge unterstützt.

Die URL für die Datenabfragefunktionen auf der Produktionsplattform lautet:

https://det.dat.de/rest/<function\_name>

Die URL für die Datenabfragefunktionen auf der Testplattform lautet:

https://det.gold.dat.de/rest/<function\_name>

Bei jedem Aufruf der REST-Schnittstelle muss ein Berechtigungsschlüssel im HTTP-Header
DAT-AuthorizationToken übergeben werden. Dieser Schlüssel muss vorher aus der login-Funktion erfragt werden (siehe Abschnitt [Anmeldung (Funktionen)](anmeldung-27906.md)). Beachten Sie, dass die Anmeldefunktionen einen anderen Pfad benutzen als die Datenabfragefunktionen
(/admin/login und /admin/refreshToken)

Der Benutzer der Schnittstelle ist für die Lokalisierung der ausgegebenen Schlüssel
für die als lokalisierbar definierten Werte verantwortlich.

Es gibt keine Schnittstellenfunktionen für die Abfrage der Listen von Ländern und
Fahrzeugtypen, da der Zugriff in der Regel pro Kunde eingeschränkt ist. Land und Fahrzeugart
sind jedoch Teil der Parameterlisten von Funktionen, die von diesen Informationen
abhängen.
