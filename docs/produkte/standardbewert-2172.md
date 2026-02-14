---
title: "Standardbewertung"
topic_id: "2172"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Standardbewertung und Standard Restwertprognose > Standardbewertung"
---

# Standardbewertung

Die Schnittstellenfunktion getVehicleEvaluation benötigt nur minimale Angaben, um eine Bewertung für ein vollständig identifiziertes
Fahrzeug durchzuführen.

Übergeben werden MUSS

- der 15stelligen DAT €uropa-Code® inklusive dem 9stelligen Marktindex. Dadurch entfällt die nochmalige Übergabe Serienausstattung.
  Sie wird automatisch ermittelt.

Übergeben werden KANN

- die Sonderausstattung inklusive Abwertungsart, beides fließt in die Bewertung ein.

Übergeben werden kann NICHT

- Zusatzausstattung

Bitte lesen Sie das Unterkapitel [Parameter](#showid/2169 "Parameter getVehicleEvaluation ") für weitere Pflichtparameter.

Auch wenn Sie [Annäherungsbewertung](#showid/2174 "Annäherungsbewertung") und [Standardbewertung](#showid/2172 "Standardbewertung") gleiche Werte übergeben, erhalten Sie nicht unbedingt die gleichen Ergebnisse.

Rückgabe

Die Anwendung liefert anhand der übergebenen Werte eine Zustandsbewertung zurück,
sofern das optionale Element condition inklusive seiner Unterelemente mitgegeben werden. Wird condition nicht mitgegeben, wird eine Bewertung zurückgegeben, die den Zustand nur anhand des
übergebenen Korrekturfaktors berücksichtigt (siehe [Parameter](#showid/2169 "Parameter getVehicleEvaluation ")). Im Erfolgsfall wird das Ergebnis als VXS zurückgeliefert, ansonsten wird eine Fehlermeldung zurückgegeben. Die Beschreibung
der Response-Elemente finden Sie im Kapitel VXS.
