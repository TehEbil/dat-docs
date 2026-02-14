---
title: "Holen einer Bewertung"
topic_id: "15180"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Verwalten von Vorgängen > Holen einer Bewertung"
---

# Holen einer Bewertung

Mit der Funktion getValuationN rufen Sie einen gespeicherten Vorgang ab.

Um einen Vorgang abzurufen, benötigen Sie mindestens die Identifikationsnummer des
Auftrags contractID. Die Identifikationsnummer entspricht der DossierId im Response der Funktion createValuationN.

Variante mit unvollständiger Fahrzeugidentifikation

Die Funktion getValuationN können Sie in der Variante mit unvollständiger Fahrzeugidentifikation einsetzen.
In diesem Fall holen Sie einen Vorgang ohne Fahrzeugidentifikation oder nur mit unvollständiger
Fahrzeugidentifikation.

Voraussetzungen:

- Der zu holende Vorgang muss sich im Mode Variante mit unvollständiger Fahrzeugidentifikation
  befinden.
- Das Element Coverage muss gesetzt sein und den Wert NOVALUATIONRESULT oder NONE enthalten.

Rückgabe

Im Erfolgsfall wird der Vorgang als VXS zurückgegeben, andernfalls wird eine Fehlermeldung zurückgegeben. Die Beschreibung
der Response-Elemente finden Sie im Kapitel VXS. In der Rückgabe finden Sie den Parameter DossierId den Sie nachfolgend für die weitere Funktionen benötigen. Die Identifikationsnummer
DossierId ist identisch mit der contractID die Sie zum Beispiel in der Funktion changeValuationN benötigen. Ob es sich um einen Response der Variante mit unvollständiger Fahrzeugidentifikation
handelt können Sie anhand des Werts incompleteValuation im Attribut type des Elements VXS erkennen. Es werden keine Halterdaten in dieser Funktion ausgegeben.

Parameter

Es werden nur die nachfolgend beschriebenen Parameter unterstützt, nicht aufgeführte
Parameter führen zu Fehlern oder werden ignoriert.

Standardfall

Request getValuationN

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| contractID | Long | Eindeutige Identifikationsnummer des Auftrags. Die Identifikationsnummer contractID ist identisch mit der DossierId aus createValuation. | numerisch | X |
| [Coverage](#expandblock-15180-d2e768822)  Mit dem Parameter Coverage steuern Sie den Datenumfang der zurückgegeben werden soll.    |  |  | | --- | --- | | Wert | Datenumfang | | MARKETPLACEEXPORT | Datenumfang COMPLETE ergänzt um die Daten für den Börsenexport (nur SilverDAT 3 PRO). | | EXTENDEDBYTRADING | Datenumfang COMPLETE ergänzt um die Unterelemente TradingActivity und TradingAdditional mit den Handelsdaten der Methoden setPurchaseData, setAdmissionData und setSalesData (nur SilverDAT 3 PRO). | | COMPLETE | Defaultwert; Standard Datenumfang für die Datenrückgabe | | NOVALUATIONRESULT | Datenrückgabe ohne die Unterelemente Valuation und VAT | | ENRICHED | Benennungen entfallen teilweise, aber mit den Bennennungen der Ausstattungen | | BASE | Datenrückgabe ganz ohne Benennungen | | SIMPLE | Bei diesem Wert entfallen zusätzlich bestimmte Unterelemente, wie zum Beispiel: CustomerAddress, TradingData, RepairCalculation, RepairOrder, RegistratinData, Engine, Equipment oder TechInfo. | | NONE | Datenrückgabe entweder mit leerem Rahmen, nur mit der DossierId oder nur mit DossierType. | | String | definiert den Umfang der Datenausgabe; Default ist COMPLETE | [Coverage](#expandblock-15180-d2e768836)  Mit dem Parameter Coverage steuern Sie den Datenumfang der zurückgegeben werden soll.    |  |  | | --- | --- | | Wert | Datenumfang | | MARKETPLACEEXPORT | Datenumfang COMPLETE ergänzt um die Daten für den Börsenexport (nur SilverDAT 3 PRO). | | EXTENDEDBYTRADING | Datenumfang COMPLETE ergänzt um die Unterelemente TradingActivity und TradingAdditional mit den Handelsdaten der Methoden setPurchaseData, setAdmissionData und setSalesData (nur SilverDAT 3 PRO). | | COMPLETE | Defaultwert; Standard Datenumfang für die Datenrückgabe | | NOVALUATIONRESULT | Datenrückgabe ohne die Unterelemente Valuation und VAT | | ENRICHED | Benennungen entfallen teilweise, aber mit den Bennennungen der Ausstattungen | | BASE | Datenrückgabe ganz ohne Benennungen | | SIMPLE | Bei diesem Wert entfallen zusätzlich bestimmte Unterelemente, wie zum Beispiel: CustomerAddress, TradingData, RepairCalculation, RepairOrder, RegistratinData, Engine, Equipment oder TechInfo. | | NONE | Datenrückgabe entweder mit leerem Rahmen, nur mit der DossierId oder nur mit DossierType. | |  |

Variante mit unvollständiger Fahrzeugidentifikation

Request getValuationN

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| contractID | Long | Eindeutige Identifikationsnummer des Auftrags. Die Identifikationsnummer contractID ist identisch mit der DossierId aus createValuation. | numerisch | X |
| Coverage | String | Steuerung für Variante mit unvollständiger Fahrzeugidentifikation | NOVALUATIONRESULT NONE | X |

¹ weitere Infos siehe Popup-Fenster
