---
title: "Mietwagenspiegel-Funktionen"
topic_id: "7685"
breadcrumb: "SilverDAT Produkte > SilverDAT Mietwagenspiegel > Schnittstellenoperationen > Mietwagenspiegel-Funktionen"
---

# Mietwagenspiegel-Funktionen

Mit Hilfe der Funktionen des Mietwagenspiegels ermitteln Sie die Mietwagenklasse,
den Nutzungsausfall und die Mietwagenpreise.

Übersicht der verfügbaren Funktionen

| Funktion | Beschreibung |
| --- | --- |
| [getRentalCarClassbyVIN](mietwagenklass-7681.md) | Mietwagenklasse anhand der Fahrzeug-Identifizierungsnummer ermitteln. |
| [getRentalCarClassbyDATECode](mietwagenklass-7711.md) | Mietwagenklasse anhand des DAT €uropa-Code® ermitteln. |
| [getLossOfUseDatabyVIN](nutzungsausfal-7723.md) | Nutzungsausfalldaten anhand der Fahrzeug-Identifizierungsnummer ermitteln. |
| [getLossOfUseDatabyDATECode](nutzungsausfal-7727.md) | Nutzungsausfalldaten anhand des DAT €uropa-Code® ermitteln. |
| [getRentalOffersbyVIN](mietwagenpreis-7731.md) | Mietwagenpreise anhand der Fahrzeug-Identifizierungsnummer und der Postleitzahl ermitteln. |
| [getRentalOffersbyDATECode](mietwagenpreis-7732.md) | Mietwagenpreise anhand des DAT €uropa-Code® und Postleitzahl ermitteln. |
| [getRentalOffersbyCarClass](mietwagenpreis-7739.md) | Mietwagenpreise anhand der Mietwagenklasse und Postleitzahl ermitteln. |
| exportRentalOffers | Mietwagenprotokoll erstellen |

Mietwagenklassen

Die Fahrzeuge wurden im DAT Fahrzeugbestand in 11 verschiedene Mietwagenklassen eingestuft.
Die Mietwagenklassen wurden dabei definiert durch Fahrzeugkosten und Motorisierung.
Die Mietwagenklassen gehen bei PKW von 1 – 11, bei Transportern von 21 – 31, wobei
in der Praxis bei Transportern aufgrund der Preisstrukturen die Klassen 24 – 31 Verwendung
finden. Für jedes Modelljahr, beginnend mit dem Jahr 2003, werden die Klassen anhand
der aktuellen Fahrzeugangebote, Preise und Ausstattungskriterien ergänzt, überarbeitet
und ggf. angepasst

Nutzungsausfallklasse

Gängige Praxis ist es, das Fahrzeugalter dahingehend zu berücksichtigten, dass ab
einem Alter von 5 Jahren eine Gruppe niedriger eingestuft wird. Ab 10 Jahren wird
die Einstufung 2 Klassen niedriger vorgenommen. Niedrigste Klasse ist aber die Klasse
A.
