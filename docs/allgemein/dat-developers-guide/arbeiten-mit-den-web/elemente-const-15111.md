---
title: "Elemente constructionTimeFrom / To"
topic_id: "15111"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > Arbeiten mit den Webservices > Wiederkehrende Parameter > Elemente constructionTimeFrom / To"
---

# Elemente constructionTimeFrom / To

Die Elemente constructionTimeFrom / constructionTimeTo werden in den Webservices der Fahrzeugauswahl und valuateFinance verwendet, um die
Ergebnismenge der Daten einzuschränken. Das Element besteht aus einer Bauzeit in DAT-Notation.
Zur Umrechnung von Datum in eine Bauzeit und umgekehrt können sie aus dem ConversionFunctionsService die Funktionen date2ConstructionTime / constructionTime2Date verwenden.

| Attributname | Codierung | Beschreibung | Beispiel |
| --- | --- | --- | --- |
| constructionTimeFrom | Integer | Bauzeit von (kann leer sein); nur Fahrzeugauswal und SilverDAT valuateFinance | z.B. 5650 |
| constructionTimeTo | Integer | Bauzeit bis (kann leer sein); nur Fahrzeugauswal und SilverDAT valuateFinance | z.B. 5770 |
