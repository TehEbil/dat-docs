---
title: "Aktualisieren eines Vorgangs ohne Wertänderung"
topic_id: "14991"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Aktualisieren eines Vorgangs ohne Wertänderung"
---

# Aktualisieren eines Vorgangs ohne Wertänderung

Mit der Funktion updateDossierN aktualisieren Sie die Bewertung eines bestehenden Vorgangs.

Um die Änderungen der Bewertung von setConditionDetails im Dossier zu übernehmen, muss updateDossierN aufgerufen werden.

Übersicht der Funktionalitäten und deren Verfügbarkeit

| Typ | DossierType | SilverDAT 3 valuateFinance | SilverDAT 3 valuateExpert/  PlusPartner |
| --- | --- | --- | --- |
| Bewertung | evaluation | X |  |
| stichtagsbezogene beziehungsweise  historische Bewertung | historic evaluation | X |  |
| stichtagsbezogene beziehungsweise  historische Bewertung | valuateExpert  valuateExpertPlusPartner |  | X |

Arbeitsweise

1. Der betreffende Vorgang wird mittels der übergebenen DossierId gesucht.
2. Falls der Vorgang gefunden wurde, wird er nachbewertet. Wenn es sich um einen Vorgang
   vom Typ: historische Bewertung handelt, wird eine Stichtagsbewertung durchgeführt.
3. Die Vorgangsdaten werden als VXS Datenstruktur zurückgegeben.
4. Die Datenausgabemenge wird durch den Parameter [Coverage](#expandblock-14991-d2e410491) begrenzt.

   Mit dem Parameter Coverage steuern Sie den Datenumfang der zurückgegeben werden soll.

   |  |  |
   | --- | --- |
   | Wert | Datenumfang |
   | MARKETPLACEEXPORT | Datenumfang COMPLETE ergänzt um die Daten für den Börsenexport (nur SilverDAT 3 PRO). |
   | EXTENDEDBYTRADING | Datenumfang COMPLETE ergänzt um die Unterelemente TradingActivity und TradingAdditional mit den Handelsdaten der Methoden setPurchaseData, setAdmissionData und setSalesData (nur SilverDAT 3 PRO). |
   | COMPLETE | Defaultwert; Standard Datenumfang für die Datenrückgabe |
   | NOVALUATIONRESULT | Datenrückgabe ohne die Unterelemente Valuation und VAT |
   | ENRICHED | Benennungen entfallen teilweise, aber mit den Bennennungen der Ausstattungen |
   | BASE | Datenrückgabe ganz ohne Benennungen |
   | SIMPLE | Bei diesem Wert entfallen zusätzlich bestimmte Unterelemente, wie zum Beispiel: CustomerAddress, TradingData, RepairCalculation, RepairOrder, RegistratinData, Engine, Equipment oder TechInfo. |
   | NONE | Datenrückgabe entweder mit leerem Rahmen, nur mit der DossierId oder nur mit DossierType. |

Eingabedaten

Es werden nur die Parameter DossierId und [Coverage](#expandblock-14991-d2e410502) unterstützt.

Mit dem Parameter Coverage steuern Sie den Datenumfang der zurückgegeben werden soll.

|  |  |
| --- | --- |
| Wert | Datenumfang |
| MARKETPLACEEXPORT | Datenumfang COMPLETE ergänzt um die Daten für den Börsenexport (nur SilverDAT 3 PRO). |
| EXTENDEDBYTRADING | Datenumfang COMPLETE ergänzt um die Unterelemente TradingActivity und TradingAdditional mit den Handelsdaten der Methoden setPurchaseData, setAdmissionData und setSalesData (nur SilverDAT 3 PRO). |
| COMPLETE | Defaultwert; Standard Datenumfang für die Datenrückgabe |
| NOVALUATIONRESULT | Datenrückgabe ohne die Unterelemente Valuation und VAT |
| ENRICHED | Benennungen entfallen teilweise, aber mit den Bennennungen der Ausstattungen |
| BASE | Datenrückgabe ganz ohne Benennungen |
| SIMPLE | Bei diesem Wert entfallen zusätzlich bestimmte Unterelemente, wie zum Beispiel: CustomerAddress, TradingData, RepairCalculation, RepairOrder, RegistratinData, Engine, Equipment oder TechInfo. |
| NONE | Datenrückgabe entweder mit leerem Rahmen, nur mit der DossierId oder nur mit DossierType. |

Für die Parameter wurden folgende Namespace-Definitionen festgelegt:

xmlns:dos="http://sphinx.dat.de/services/DossierN" für SilverDAT 3 valuateFinance

xmlns:dos="http://www.dat.de/services/Dossier1N" für SilverDAT 3 valuateExpert/PlusPartner

xmlns:vxs="http://www.dat.de/vxs"

Rückgabe

Im Erfolgsfall wird der Vorgang als VXS zurückgeliefert, ansonsten wird eine Fehlermeldung zurückgegeben. Die Beschreibung
der Response-Elemente finden Sie im Kapitel VXS.
