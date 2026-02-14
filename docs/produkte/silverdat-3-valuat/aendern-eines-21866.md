---
title: "Aendern eines Vorgangs mit EV-Wertkorrektur"
topic_id: "21866"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Fahrzeugbewertung von Elektroautos > Fahrzeugbewertung von Elektroautos > Aendern eines Vorgangs mit EV-Wertkorrektur"
---

# Aendern eines Vorgangs mit EV-Wertkorrektur

Für die EV-Wertkorrektur muss es sich um ein rein elektrisches Fahrzeug mit fest verbauter
Batterie und eine Bewertung für das Datenland Deutschland handeln.

Übersicht der Voraussetzungen

| Beschreibung | Parameter | notwendiger Wert |
| --- | --- | --- |
| rein elektrisches Fahrzeug | TechInfo.FuelMethod | Elektro |
| Datenland Deutschland | Vehicle.Country | DE |

Sind diese Voraussetzungen erfüllt, haben Sie die Möglichkeit zur erweiterten Berechnung
des Batterie-abhängigen Restwerts des Elektroautos.

Beim Aufruf der Funktion changeDossierN können dazu zusätzliche Parameter zur EV-Wertkorrektur übergeben werden.
