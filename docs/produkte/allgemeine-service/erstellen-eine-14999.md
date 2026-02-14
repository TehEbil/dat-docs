---
title: "Erstellen eines neuen Vorgangs"
topic_id: "14999"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Erstellen eines neuen Vorgangs"
---

# Erstellen eines neuen Vorgangs

Mit der Funktion createDossierN erstellen Sie neue Vorgänge.

Übersicht der Funktionalitäten und deren Verfügbarkeit

| Typ | DossierType | ValuationType | SilverDAT 3 valuateFinance | SilverDAT 3 valuateExpert/  PlusPartner |
| --- | --- | --- | --- | --- |
| Bewertung | evaluation | valuation | X |  |
| Restwertprognose für Gebrauchtfahrzeuge | evaluation | residual value used vehicle | X |  |
| Restwertprognose für Neufahrzeuge | evaluation | residual value new vehicle | X |  |
| stichtagsbezogene beziehungsweise  historische Bewertung | historic evaluation | valuation | X |  |
| stichtagsbezogene beziehungsweise  historische Bewertung | valuateExpert  valuateExpertPlusPartner | valuation |  | X |

Momentan stehen die Datenländer Bulgarien, China, Deutschland, Frankreich, Griechenland,
Italien, Niederlande, Österreich, Rumänien, Schweiz, Slowakei, Spanien, Tschechische
Republik, Türkei und Ungarn für die Bewertung zur Verfügung. Derzeit können Sie als
Sprache bulgarisch, chinesisch, deutsch, englisch, französisch, griechisch, italienisch,
niederländisch, polnisch, rumänisch, russisch, slowakisch, spanisch, tschechisch,
türkisch und ungarisch auswählen. Bitte beachten Sie, dass gegenwärtig nur bestimmte
Kombinationen aus Datenland und Sprache möglich sind.

Kurzbeschreibung der Arbeitsweise

1. Die Eingaben werden validiert.
2. Das Fahrzeug wird ausschließlich über den DAT €uropa-Code® identifiziert.
3. Der Vorgang wird angelegt, falls die Abfrage nicht mit einer benötigten Freigabe wiederholt
   werden muss.
4. Das Fahrzeug wird bewertet und der Vorgang wird gespeichert, sofern dies nicht mittels
   des Speicherkennzeichens verhindert wird.
5. Die Vorgangsdaten werden als VXS Datenstruktur zurückgegeben.
6. Die Datenausgabemenge wird durch den Parameter Coverage begrenzt.

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

Es werden nur die nachfolgend beschriebenen Parameter unterstützt, alle anderen werden
ignoriert.

Für die Parameter wurden folgende Namespace-Definitionen festgelegt:

xmlns:dos="http://sphinx.dat.de/services/DossierN" für SilverDAT 3 valuateFinance

xmlns:dos="http://www.dat.de/services/Dossier1N" für SilverDAT 3 valuateExpert/PlusPartner

xmlns:vxs="http://www.dat.de/vxs"

Rückgabe

Im Erfolgsfall wird der Vorgang als VXS zurückgeliefert, ansonsten wird eine Fehlermeldung zurückgegeben. Die Beschreibung
der Response-Elemente finden Sie im Kapitel VXS.
