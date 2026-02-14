---
title: "Prognosen (Forecasts)"
topic_id: "1754"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Bewertungsdaten (Valuation) > Prognosen (Forecasts)"
---

# Prognosen (Forecasts)

Forecasts enthält ein Element: Forecast. Forecast enthält weitere Elemente, darunter
auch ForecastItems. ForecastItems enthält das Element ForecastItem, das wiederum weitere
Elemente enthält:

Forecast

| Element | Typ | Beschreibung |
| --- | --- | --- |
| ForecastType | String | Art der Restwertprognose  new car - Neufahrzeug  used car - Gebrauchtfahrzeug |
| PriceType | String | PriceType (Preisart EK/ VK):  SALES - VK  PURCHASE - EK |
| IncludeVat | Boolean | Mit oder ohne Mehrwertsteuerangabe  true - mit Mehrwertsteuer  false - ohne Mehrwertsteuer |
| CurveType | String | Kurvenart  MINIMUM - minimal  DAT - nach DAT  MAXIMUM - maximal |
| DecreaseType | String | Abwertungsart |
| StartType | String | Kennzeichen für die Angabe des Fahrzeugalters (Gesamt oder ab Bewertungsmonat); Standardwert ist INITIAL REGISTRATION  INITIAL REGISTRATION - Erstzulassungsdatum  RECENT EVALUATION |
| ValueType | String | Form der Wertrückgabe  MONETARY - Beträge in Euro  MILEAGE - Kilometer-Laufleistung  PERCENTAGE -in Prozent |
| MileageType | String | Kennzeichen für die Laufleistungsangabe  YEAR - Laufleistung pro Jahr  TOTAL - Gesamtlaufleistung |
| ConsiderCurrentCondition | Boolean | Berücksichtigung des aktuellen Fahrzeugzustands  true - Fahrzeugzustand wird berücksichtigt  false - Fahrzeugzustand wird nicht berücksichtigt |
| ForecastItems |  | s. ForecastItem |

ForecastItem

| Element | Typ | Beschreibung |
| --- | --- | --- |
| Months | Integer | Bewertungszeitpunkt in Monaten entsprechend der Vorgabe im Request |
| MileagePerYear | Integer | Jahresfahrleistung |
| MileageTotal | Integer | Kilometer-Gesamtlaufleistung |
| Value | Decimal | Absolutwert der Restwertprognose (Nettowert) |
| ValueGross | Decimal | Absolutwert der Restwertprognose (Bruttowert) |
| Percentage | Decimal | Prozentwert der Restwertprognose (Nettowert) |
| PercentageNet | Decimal | nicht aktiv |
| PercentageGross | Decimal | nicht aktiv |
| Error | String | Fehlertext |
| Row | Integer | nicht aktiv |
