---
title: "Erstellen eines neuen Vorgangs/einer neuen Bewertung mit EV-Wertkorrektur"
topic_id: "21882"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Fahrzeugbewertung von Elektroautos > Fahrzeugbewertung von Elektroautos > Erstellen eines neuen Vorgangs/einer neuen Bewertung mit EV-Wertkorrektur"
---

# Erstellen eines neuen Vorgangs/einer neuen Bewertung mit EV-Wertkorrektur

###### Erstellen eines neuen Vorgangs/einer neuen Bewertung mit EV-Wertkorrektur Für die EV-Wertkorrektur muss es sich um ein rein elektrisches Fahrzeug mit fest verbauter Batterie und eine Bewertung für das Datenland Deutschland handeln. Übersicht der Voraussetzungen | Beschreibung | Parameter | notwendiger Wert | | --- | --- | --- | | rein elektrisches Fahrzeug | TechInfo.FuelMethod | Elektro | | Datenland Deutschland | Vehicle.Country | DE | Sind diese Voraussetzungen erfüllt, haben Sie die Möglichkeit zur erweiterten Berechnung des Batterie-abhängigen Restwerts des Elektroautos. Beim Aufruf der Funktionen createValuationN und doValuationInMemoryN können dazu zusätzliche Parameter zur EV-Wertkorrektur übergeben werden.
