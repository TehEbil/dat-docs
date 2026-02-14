---
title: "Standard Restwertprognose Gebrauchtfahrzeuge"
topic_id: "2187"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Standardbewertung und Standard Restwertprognose > Standard Restwertprognose Gebrauchtfahrzeuge"
---

# Standard Restwertprognose Gebrauchtfahrzeuge

Mit der Funktion getUsedVehicleForecast kann eine Restwertprognose durchgeführt werden. Notwendig ist ein vollständig identifiziertes
Fahrzeug mit minimal notwendigen Angaben. Restwertprognosen erfolgen immer auf Basis
der Regelbesteuerung. Bitte lesen Sie das Unterkapitel [Parameter](#showid/2165 "Parameter getUsedVehicleForecast ") für alle weiteren Pflichtparameter.

Bei den Monatsangaben gehen wir IMMER von Angaben ab Erstzulassung aus. Die Angabe
ab Bewertungsmonat kann über Schnittstelle NICHT eingestellt werden.

Für folgende Fahrzeugarten können Sie Restwertprognosen durchführen:

- Pkw
- Geländewagen/SUV
- Transporter

Rückgabe

Es gibt ein Fehlerfeld in den Zellen für die Restwertprognose. Wenn ein Fehler aufgetreten
ist, wird dieses Feld gefüllt und ausgegeben. Die Ergebniswerte der Zelle sind im
Fehlerfall leer. Zurückgegeben wird ein vollständiges Fahrzeug samt Ausstattung und
der Restwertprognose nach Vorgabe. Im Erfolgsfall wird das Ergebnis als VXS zurückgeliefert, ansonsten wird eine Fehlermeldung zurückgegeben. Die Beschreibung
der Response-Elemente finden Sie im Kapitel VXS.
