---
title: "Löschen eines Vorgangs"
topic_id: "15009"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Löschen eines Vorgangs"
---

# Löschen eines Vorgangs

Mit der Funktion deleteDossierN löschen Sie einen bestehenden Vorgang.

Übersicht der Funktionalitäten und deren Verfügbarkeit

| Typ | DossierType | SilverDAT 3 valuateFinance | SilverDAT 3 valuateExpert/  PlusPartner |
| --- | --- | --- | --- |
| Bewertung | evaluation | X |  |
| stichtagsbezogene beziehungsweise  historische Bewertung | historic evaluation | X |  |
| stichtagsbezogene beziehungsweise  historische Bewertung | valuateExpert  valuateExpertPlusPartner |  | X |

Arbeitsweise

1. Der betreffende Vorgang wird mittels der übergebenen DossierId gesucht.
2. Der Vorgang wird gelöscht, falls er gefunden werden konnte.
3. Im Erfolgsfall wird true im Tag Success zurückgegeben, andernfalls eine Fehlermeldung.

Eingabedaten

Als Parameter kann nur die DossierId angegeben werden.

Für die Parameter wurden folgende Namespace-Definitionen festgelegt:

xmlns:dos="http://sphinx.dat.de/services/DossierN" für SilverDAT 3 valuateFinance

xmlns:dos="http://www.dat.de/services/Dossier1N" für SilverDAT 3 valuateExpert/PlusPartner

xmlns:vxs="http://www.dat.de/vxs"

Rückgabe

Im Erfolgsfall wird im Tag Success der Wert true zurückgeliefert, ansonsten wird eine Fehlermeldung zurückgegeben.
