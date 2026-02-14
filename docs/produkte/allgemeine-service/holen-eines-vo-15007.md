---
title: "Holen eines Vorgangs"
topic_id: "15007"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Holen eines Vorgangs"
---

# Holen eines Vorgangs

Mit getDossierN holen Sie bestehende Vorgänge ab.

Übersicht der Funktionalitäten und deren Verfügbarkeit

| Typ | DossierType | SilverDAT 3 valuateFinance | SilverDAT 3 valuateExpert/  PlusPartner |
| --- | --- | --- | --- |
| Bewertung | evaluation | X |  |
| stichtagsbezogene beziehungsweise  historische Bewertung | historic evaluation | X |  |
| stichtagsbezogene beziehungsweise  historische Bewertung | valuateExpert  valuateExpertPlusPartner |  | X |

Arbeitsweise

1. Der betroffene Vorgang wird mittels der übergebenen DossierId gesucht.
2. Die Vorgangsdaten werden als VXS Datenstruktur zurückgegeben.
3. Die Datenausgabemenge wird durch den Parameter [Coverage](#expandblock-15007-d2e411815) begrenzt.

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

Es werden nur die nachfolgend beschriebenen Parameter unterstützt, nicht erwähnte
Parameter werden ignoriert.

Für die Parameter wurden folgende Namespace-Definitionen festgelegt:

xmlns:dos="http://sphinx.dat.de/services/DossierN" für SilverDAT 3 valuateFinance

xmlns:dos="http://www.dat.de/services/Dossier1N" für SilverDAT 3 valuateExpert/PlusPartner

xmlns:vxs="http://www.dat.de/vxs"

Rückgabe

Im Erfolgsfall wird der Vorgang als VXS zurückgeliefert, ansonsten wird eine Fehlermeldung zurückgegeben. Die Beschreibung
der Response-Elemente finden Sie im Kapitel VXS.
