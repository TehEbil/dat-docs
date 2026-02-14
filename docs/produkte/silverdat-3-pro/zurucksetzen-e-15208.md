---
title: "Zurücksetzen einer Bewertung auf die DAT Standardeinstellungen"
topic_id: "15208"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Verwalten von Vorgängen > Zurücksetzen einer Bewertung auf die DAT Standardeinstellungen"
---

# Zurücksetzen einer Bewertung auf die DAT Standardeinstellungen

Mit der Funktion resetValuation2defaultN führen Sie eine Neubewertung des Vorgangs durch. Hierbei werden alle bewertungsrelevanten
Parameter auf die DAT-Standardwerte zurückgesetzt. Die Funktion resetValuation2defaultN unterstützt nicht die Variante mit unvollständiger Fahrzeugidentifikation.

Um eine Bewertung auf die DAT-Standardwerte zurückzusetzen, benötigen Sie die Identifikationsnummer
des Auftrags contractID.

Arbeitsweise

1. Die betreffende Bewertung wird anhand der contractID ermittelt.
2. Falls die betreffende Bewertung gefunden wurde, wird sie auf die DAT Standardwerte
   zurückgesetzt. Hierbei werden die nachfolgenden Parameter überschrieben:

   1. Alle Parameter der Zustandsbewertung
   2. Alle Benutzer-Wertangaben (auch brutto) mit Ausnahme von Neupreisen für Zusatzausstattungen
   3. Alle Benutzer-Korrekturbeträge
   4. Pauschaler Korrekturfaktor
   5. Beschreibende Benutzer-Fahrzeugdaten (zum Beispiel: Baujahr, Benennungen von Aufbauten)
3. Der Vorgang wird nachbewertet.
4. Die Vorgangsdaten werden als VXS Datenstruktur zurückgegeben. Der Datenumfang wird durch den Parameter Coverage bestimmt.

Rückgabe

Im Erfolgsfall wird der Vorgang als VXS zurückgegeben, andernfalls wird eine Fehlermeldung zurückgegeben. Die Beschreibung
der Response-Elemente finden Sie im Kapitel VXS. In der Rückgabe finden Sie den Parameter DossierId den Sie nachfolgend für die weitere Funktionen benötigen. Die Identifikationsnummer
DossierId ist identisch mit der contractID die Sie zum Beispiel in der Funktion getValuationN benötigen.

Parameter

Request resetValuation2defaultN

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| contractID | Long | Eindeutige Identifikationsnummer des Auftrags. Die Identifikationsnummer contractID ist identisch mit der DossierId aus createValuationN | numerisch | X |
| Coverage  Mit dem Parameter Coverage steuern Sie den Datenumfang der zurückgegeben werden soll.    |  |  | | --- | --- | | Wert | Datenumfang | | MARKETPLACEEXPORT | Datenumfang COMPLETE ergänzt um die Daten für den Börsenexport (nur SilverDAT 3 PRO). | | EXTENDEDBYTRADING | Datenumfang COMPLETE ergänzt um die Unterelemente TradingActivity und TradingAdditional mit den Handelsdaten der Methoden setPurchaseData, setAdmissionData und setSalesData (nur SilverDAT 3 PRO). | | COMPLETE | Defaultwert; Standard Datenumfang für die Datenrückgabe | | NOVALUATIONRESULT | Datenrückgabe ohne die Unterelemente Valuation und VAT | | ENRICHED | Benennungen entfallen teilweise, aber mit den Bennennungen der Ausstattungen | | BASE | Datenrückgabe ganz ohne Benennungen | | SIMPLE | Bei diesem Wert entfallen zusätzlich bestimmte Unterelemente, wie zum Beispiel: CustomerAddress, TradingData, RepairCalculation, RepairOrder, RegistratinData, Engine, Equipment oder TechInfo. | | NONE | Datenrückgabe entweder mit leerem Rahmen, nur mit der DossierId oder nur mit DossierType. | | String | Definiert den Datenumfang | Coverage  Mit dem Parameter Coverage steuern Sie den Datenumfang der zurückgegeben werden soll.    |  |  | | --- | --- | | Wert | Datenumfang | | MARKETPLACEEXPORT | Datenumfang COMPLETE ergänzt um die Daten für den Börsenexport (nur SilverDAT 3 PRO). | | EXTENDEDBYTRADING | Datenumfang COMPLETE ergänzt um die Unterelemente TradingActivity und TradingAdditional mit den Handelsdaten der Methoden setPurchaseData, setAdmissionData und setSalesData (nur SilverDAT 3 PRO). | | COMPLETE | Defaultwert; Standard Datenumfang für die Datenrückgabe | | NOVALUATIONRESULT | Datenrückgabe ohne die Unterelemente Valuation und VAT | | ENRICHED | Benennungen entfallen teilweise, aber mit den Bennennungen der Ausstattungen | | BASE | Datenrückgabe ganz ohne Benennungen | | SIMPLE | Bei diesem Wert entfallen zusätzlich bestimmte Unterelemente, wie zum Beispiel: CustomerAddress, TradingData, RepairCalculation, RepairOrder, RegistratinData, Engine, Equipment oder TechInfo. | | NONE | Datenrückgabe entweder mit leerem Rahmen, nur mit der DossierId oder nur mit DossierType. | |  |

¹ weitere Infos siehe Popup-Fenster
