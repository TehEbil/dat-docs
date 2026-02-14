---
title: "Aendern eines Vorgangs"
topic_id: "14989"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Aendern eines Vorgangs"
---

# Aendern eines Vorgangs

Mit der Funktion changeDossierN ändern Sie bestehende Vorgänge.

Übersicht der Funktionalitäten und deren Verfügbarkeit

| Typ | DossierType | ValuationType | SilverDAT 3 valuateFinance | SilverDAT 3 valuateExpert/  PlusPartner |
| --- | --- | --- | --- | --- |
| Bewertung | evaluation | valuation | X |  |
| Restwertprognose für Gebrauchtfahrzeuge | evaluation | residual value used vehicle | X |  |
| Restwertprognose für Neufahrzeuge | evaluation | residual value new vehicle | X |  |
| stichtagsbezogene beziehungsweise historische Bewertung | historic evaluation | valuation | X |  |
| stichtagsbezogene beziehungsweise  historische Bewertung | valuateExpert  valuateExpertPlusPartner | valuation |  | X |

Kurzbeschreibung der Arbeitsweise

1. Der betreffende Vorgang wird mittels der übergebenen DossierId gesucht.
2. Die Eingaben werden validiert.
3. Eine eventuelle Fahrzeugidentifikation erfolgt ausschließlich über den DAT €uropa-Code®.
4. Die Eingabedaten werden übernommen. Dabei gilt grundsätzlich, dass nur übergebene
   Werte geändert werden, fehlende Unterelemente bleiben unverändert. Ausnahme sind diejenigen
   Daten, die explizit löschbar sind: Ausstattungslisten, Zustandsdaten und Restwertprognosedaten.
5. Das Fahrzeug wird bewertet und der Vorgang gespeichert.
6. Die Vorgangsdaten werden als VXS Datenstruktur zurückgegeben.
7. Die Datenausgabemenge wird durch den Parameter [Coverage](#expandblock-14989-d2e410104) begrenzt.

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

Details zur Funktionsweise und der Datenrückgabe

Nur der Parameter DossierId ist immer Pflicht, über diesen wird das Aktenzeichen identifiziert. Parameter, die
nicht angegeben werden, führen normalerweise nicht zu einer Änderung.

Ausnahmen:

1. Um Sonder- oder Zusatzausstattungen (Equipment-Element) zu ändern muss man immer alle Sonder- und Zusatzausstattungen nochmals mit
   allen zugehörigen Details übergeben. Fehlende Elemente löschen zuvor gespeicherte
   Elemente.
2. Wird ein Condition-Element angegeben, dann müssen auch alle zugehörigen Unterelemente angegeben werden.
   Fehlende Unterelemente löschen einen gegebenenfalls gespeicherten Wert.
3. Wird ein Forecasts-Element angegeben, dann muss auch das zugehörige Unterelement komplett angegeben
   werden. Für fehlende Unterelemente werden Standardwerte angenommen.

Falls mindestens einer der Parameter: DAT €uropa-Code®, Marktindex oder Bauzeit geändert
wird, dann muss eine Fahrzeugneuidentifikation durchgeführt werden. Das bedeutet,
dass diese drei Parameter immer zusammengehörig angegeben werden müssen. Eine Fahrzeugneuidentifikation
hat außerdem zur Folge, dass:

1. die gespeicherte Ausstattungsliste gelöscht wird.
2. falls das Fahrzeug ehemals über eine VIN-Abfrage identifiziert wurde, die Ergebnisse
   der VIN-Abfrage gelöscht werden. Die VIN selbst bleibt gespeichert, wird jedoch als
   deaktiviert gekennzeichnet.
3. Fahrzeugidentifikationsdaten und Ausstattung auch in einem eventuellen zweiten vorhandenen
   Datensatz angepasst werden - siehe unten.

Der Vorgangstyp kann nachträglich nicht mehr geändert werden, der Parameter DossierType wird deshalb von changeDossierN nicht unterstützt.

Die Zusammenhänge sind in dem folgenden Bild grafisch dargestellt:

Ist ein Vorgang vom Typ HISTORIC EVALUATION, wird eine Fahrzeugbewertung zum Stichtag durchgeführt (Parameter DeterminatedDate). Alle Werte und Angaben beziehen sich in diesem Fall auf dieses Datum. Zustandsdaten
werden beim Typ HISTORIC EVALUATION ignoriert.
