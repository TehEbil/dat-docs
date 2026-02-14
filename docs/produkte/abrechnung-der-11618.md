---
title: "Abrechnung der Transaktionen"
topic_id: "11618"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > interaktive Fahrzeugauswahl > Abrechnung der Transaktionen"
---

# Abrechnung der Transaktionen

Immer wenn im Ergebnis dieser Schnittstellenfunktion eine Liste von Fahrzeugen enthalten
ist (im Objekt vehicles), entstehen Kosten und es wird dieser Aufruf als Transaktion protokolliert.

Wenn der Funktionsaufruf als Transaktion protokolliert wurde, wird im HTTP-Header
ein zusätzliches Element mit dem Namen X-DAT-VS-TOKEN geliefert mit einem Token als Inhalt. Das Token hat eine begrenzte Gültigkeit.

Beispiel

X-DAT-VS-TOKEN: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJkYXQiLCJ0aW1lc3RhbXAiOjE1NDUyMDIzODkwMTB9.7x5p2CO2xqeDB1ShQxQXv7x7q7dAGfqPaLtOIlrIB9

Bei allen nachfolgenden Aufrufen zur weiteren Verfeinerung der Fahrzeugsuche, z.B.
mit zusätzlichen Filtern, sollte dieses Token im HTTP-Header des Requests verwendet werden. Damit wird vermieden, dass diese Aufrufe ebenfalls
als kostenpflichtige Transaktion protokolliert werden. Von Beginn der interaktiven
Fahrzeugauswahl bis zum Schluss mit einem einzelnen gefundenen Fahrzeug soll möglichst
nur einmalig eine Abrechnung erfolgen.
