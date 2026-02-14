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
| [getRentalCarClassbyVIN](#showid/7681 "Mietwagenklasse anhand der VIN ermitteln") | Mietwagenklasse anhand der Fahrzeug-Identifizierungsnummer ermitteln. |
| [getRentalCarClassbyDATECode](#showid/7711 "Mietwagenklasse anhand des DAT €uropa-Code® ermitteln") | Mietwagenklasse anhand des DAT €uropa-Code® ermitteln. |
| [getLossOfUseDatabyVIN](#showid/7723 "Nutzungsausfalldaten anhand der VIN ermitteln") | Nutzungsausfalldaten anhand der Fahrzeug-Identifizierungsnummer ermitteln. |
| [getLossOfUseDatabyDATECode](#showid/7727 "Nutzungsausfalldaten anhand DAT €uropa-Code® ermitteln") | Nutzungsausfalldaten anhand des DAT €uropa-Code® ermitteln. |
| [getRentalOffersbyVIN](#showid/7731 "Mietwagenpreise anhand der VIN und PLZ ermitteln") | Mietwagenpreise anhand der Fahrzeug-Identifizierungsnummer und der Postleitzahl ermitteln. |
| [getRentalOffersbyDATECode](#showid/7732 "Mietwagenpreise anhand des DAT €uropa-Code® und PLZ ermitteln") | Mietwagenpreise anhand des DAT €uropa-Code® und Postleitzahl ermitteln. |
| [getRentalOffersbyCarClass](#showid/7739 "Mietwagenpreise anhand der Mietwagenklasse und PLZ ermitteln") | Mietwagenpreise anhand der Mietwagenklasse und Postleitzahl ermitteln. |
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
