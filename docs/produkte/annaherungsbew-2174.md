---
title: "Annäherungsbewertung"
topic_id: "2174"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Annäherungsbewertung"
---

# Annäherungsbewertung

Mit der Funktion getVehicleApproximateValue können Sie eine Bewertung durchführen, selbst wenn nur eine ungenaue Fahrzeugidentifikation
zur Verfügung steht. Das Ergebnis ist entsprechend unsicherer als eine Bewertung mit
exakter Identifizierung. Die Funktion getVehicleApproximateValue ist die einzige Bewertungsfunktion die sowohl die Identifikation als auch die Bewertung
beinhaltet.

Ungenaue Schlüssel zur Fahrzeugidentifikation

Als ungenaue Schlüssel zur Fahrzeugidentifikation gelten in der Datenwelt der DAT
alle Schlüssel, die nicht zu einem eindeutig identifizierten Fahrzeug führen:

- KBA-Schlüssel - Deutschland
- Nationalcode - Österreich
- DAT €uropa-Code®, 15-stellig
- Modellcode, 11-stellig

Näheres zum Modellcode

Der Modellcode ist eine Kombination aus Fahrzeugart-, Hersteller-, Haupttyp- und Untertypschlüssel
und damit 11stellig. Er dient zur Vereinfachung für den Kunden. Der hypothetische
Workflow sieht dabei wie folgt aus:

Der Schnittstellenpartner programmiert mithilfe der Schnittstellenfunktionen der neuen
Fahrzeugauswahl einen Fahrzeug-Suchbaum, den er vom Kunden ausfüllen lässt. Um dem
Kunden die Arbeit zu erleichtern und das Ziel - nämlich die Bewertung - schneller
zu erreichen, wird die Fahrzeugauswahl nur bis zum Untertypen ausgewählt. Optional
kann der Kunde auswählen, welchen Motor das Fahrzeug verbaut hat, welche Karosserie
eingebaut ist. Diese gehören zu den klassifizierenden Ausstattungen.

Mit diesen rudimentären Fahrzeuginformationen kann nun eine Annäherungsbewertung durchgeführt
werden.

Der exakte Bewertungsschlüssel

Als exakter Bewertungsschlüssel gilt der 15-stelligen DAT €uropa-Code® inklusive dem 9-stelligen Marktindex. Lesen Sie mehr über den DAT €uropa-Code® und seine Zusammensetzung in unserem [kleiner Exkurs: DAT €uropa-Code und Marktindex](#showid/1882 "kleiner Exkurs: DAT €uropa-Code® und Marktindex").

Mit dieser Bewertungsfunktion haben Sie die Möglichkeit:

- Eine Annäherungsbewertung mit einem ungenauen Schlüssel durchzuführen
- Ein Kennzeichen zu setzen, mit dem Sie markieren, welche Fahrzeugidentifikation benutzt
  werden soll (bitte lesen Sie hierzu auch die [Parameter](#showid/1818 "Parameter getVehicleApproximateValue ") mit zusätzlichen Erläuterungen).
- Den 15-stelligen DAT €uropa-Code® und den 9-stelligen Marktindex zu übergeben.

Hinweise:

- Bitte verwenden Sie eine exakte Bewertungsfunktion , falls Ihnen der 15-stellige DAT €uropa-Code® und der 9-stelligen Marktindex zur Verfügung steht.
- Die exakte Bewertung führen Sie mit den Methoden createDossierN oder getVehicleEvaluation durch.
- Die Funktion getVehicleApproximateValue speichert die Ergebnisse NICHT im System ab.
- Auch wenn Sie bei der [Annäherungsbewertung](#showid/2174 "Annäherungsbewertung") und der [Standardbewertung](#showid/2172 "Standardbewertung") gleiche Werte übergeben, erhalten Sie nicht unbedingt die gleichen Ergebnisse.

Rückgabe

Die Anwendung sucht den zugehörigen DAT €uropa-Code® heraus und liefert anhand der übergebenen Werte eine Bewertung zurück, die den Fahrzeugzustand
unberücksichtigt lässt. Im Erfolgsfall wird das Ergebnis als VXS zurückgeliefert, ansonsten wird eine Fehlermeldung zurückgegeben. Die Beschreibung
der Response-Elemente finden Sie im Kapitel VXS.

Über das Rückgabefeld IdentificationSource kann ausgelesen werden, mit welchem Schlüssel die Bewertung vorgenommen worden ist.
Die möglichen Werte sind hier KBA, NATIONALCODE, DATECODE oder MODEL.
