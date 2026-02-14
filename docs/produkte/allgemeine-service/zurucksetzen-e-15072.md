---
title: "Zurücksetzen eines Vorgangs auf die DAT-Vorgaben"
topic_id: "15072"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Zurücksetzen eines Vorgangs auf die DAT-Vorgaben"
---

# Zurücksetzen eines Vorgangs auf die DAT-Vorgaben

Mit der Funktion resetDossier2DefaultN führen Sie eine Neubewertung des Vorgangs durch. Hierbei werden alle bewertungsrelevanten
Parameter auf die DAT-Standardwerte zurückgesetzt.

Übersicht der Funktionalitäten und deren Verfügbarkeit

| Typ | DossierType | SilverDAT 3 valuateFinance | SilverDAT 3 valuateExpert/PlusPartner |
| --- | --- | --- | --- |
| Bewertung | evaluation | X |  |
| Stichtagsbezogene beziehungsweise historische Bewertung | historic evaluation | X |  |
| Stichtagsbezogene beziehungsweise historische Bewertung | valuateExpert valuateExpertPlusPartner |  | X |

Arbeitsweise

1. Der betreffende Vorgang wird mittels der übergebenen DossierId gesucht.
2. Falls der Vorgang gefunden wurde, wird er auf die DAT Standardwerte zurückgesetzt.
   Hierbei werden die nachfolgenden Parameter überschrieben:

   1. Alle Parameter der Zustandsbewertung
   2. Alle Benutzer-Wertangaben (auch brutto) mit Ausnahme von Neupreisen für Zusatzausstattungen
   3. Alle Benutzer-Korrekturbeträge
   4. Pauschaler Korrekturfaktor
   5. Beschreibende Benutzer-Fahrzeugdaten (zum Beispiel: Baujahr, Benennungen von Aufbauten)
3. Der Vorgang wird nachbewertet. Wenn es sich um einen Vorgang vom Vorgangstyp: historische Bewertung handelt, wird eine Stichtagsbewertung durchgeführt.
4. Die Vorgangsdaten werden als VXS Datenstruktur zurückgegeben. Die Datenausgabemenge wird durch den Parameter [Coverage](#expandblock-15072-d2e431692) begrenzt.

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

Es werden nur die Parameter DossierId und Coverage unterstützt.

Für die Parameter wurden folgende Namespace-Definitionen festgelegt:

xmlns:dos="http://sphinx.dat.de/services/DossierN" für SilverDAT 3 valuateFinance

xmlns:dos="http://www.dat.de/services/Dossier1N" für SilverDAT 3 valuateExpert/PlusPartner

xmlns:vxs="http://www.dat.de/vxs"

Rückgabe

Als Antwort wird im Erfolgsfall der Vorgang als VXS, ansonsten wird eine Fehlermeldung zurückgegeben. Die Beschreibung der Response-Elemente
finden Sie im Kapitel VXS.
