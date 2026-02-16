---
title: "Neubewertung und Nachbewertung der Dossiers"
topic_id: "12671"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Neubewertung und Nachbewertung der Dossiers"
---

# Neubewertung und Nachbewertung der Dossiers

Mithilfe der beschriebenen Funktionen können Sie eine Liste von Dossiers oder alle
Dossiers neu- oder nachbewerten. Die zugehörigen Funktionen finden Sie unter dem Service
BatchValuationService in SilverDAT 3 PRO. In BatchValuationService können Sie Tasks verwalten. Ein Task ist ein Auftrag. Diese Methoden können nicht für Kalkulations-Dossiers verwendet werden.

Ein Auftrag kann folgende Status besitzen:

- WAITING = wartet bis der vorherige Auftrag abgearbeitet ist
- INWORK = Auftrag ist in Arbeit
- DONE = Auftrag ist abgearbeitet
- CANCELED = Auftrag wurde abgebrochen

Übersicht der Funktionen

| Bezeichnung | Funktion | Beschreibung |
| --- | --- | --- |
| Auftrag starten | startTaskN | Zusammenfassung der Dossiers zu einem Auftrag, der nachbewertet oder neubewertet werden soll. |
| Auftrag holen | getTask | Holen der Auftragsinformationen |
| Hole Dokumentenergebnis des Auftrags | getDocument | Holen eines  Auftragsdokuments |
| Alle Aufträge holen | getAllTask | Holen aller Aufträge |
| Abbrechen eines Auftrags | cancelTaskN | Abbruch eines Auftrags |

WSDL

[https://www.datgroup.com/myClaim/soap/v2/BatchValuationService?wsdl](https://www.dat.de/myClaim/soap/v2/BatchValuationService?wsdl)

Serviceaufruf

https://www.datgroup.com/myClaim/soap/v2/BatchValuationService
