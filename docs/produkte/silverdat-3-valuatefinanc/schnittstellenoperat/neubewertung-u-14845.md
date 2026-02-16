---
title: "Neubewertung und Nachbewertung der Dossiers"
topic_id: "14845"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Neubewertung und Nachbewertung der Dossiers"
---

# Neubewertung und Nachbewertung der Dossiers

Mithilfe der nachfolgend beschriebenen Funktionen können Sie einen Auftrag starten,
der für eine Liste von Dossiers eine Neubewertung oder eine Nachbewertung durchführt.
Die zugehörigen Funktionen finden Sie unter dem Service BatchValuation in SilverDAT 3 FinanceLine. Ein Task ist hierbei ein Auftrag.

Ein Auftrag kann folgende Status besitzen:

- WAITING = wartet bis der erste Auftrag abgearbeitet ist
- INWORK = Auftrag ist in Arbeit
- DONE = Auftrag ist abgearbeitet
- CANCEL = Auftrag wurde abgebrochen

Übersicht der Funktionen

| Bezeichnung | Funktion | Beschreibung |
| --- | --- | --- |
| Auftrag starten | startTask | Zusammenfassung der Dossiers zu einem Auftrag, der nachbewertet oder neubewertet werden soll. |
| Auftrag holen | getTask | Holen der Auftragsinformationen |
| Hole Dokumentenergebnis des Auftrags | getDocument | Holen eines  Auftragsdokuments |
| Alle Aufträge holen | getAllTask | Holen aller Aufträge |
| Abbrechen eines Auftrags | cancelTask | Abbruch eines Auftrags |

WSDL

<https://www.datgroup.com/FinanceLine/soap/BatchValuation?wsdl>

Service request

https://www.datgroup.com/FinanceLine/soap/BatchValuation
