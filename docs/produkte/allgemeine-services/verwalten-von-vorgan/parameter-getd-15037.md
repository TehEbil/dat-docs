---
title: "Parameter getDossierN"
topic_id: "15037"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Holen eines Vorgangs > Parameter getDossierN"
---

# Parameter getDossierN

Request getDossierN

| Parameter | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| DossierId | Integer | Eindeutige Vorgangskennung | numerisch | X |
| Coverage  Mit dem Parameter Coverage steuern Sie den Datenumfang der zurückgegeben werden soll.    |  |  | | --- | --- | | Wert | Datenumfang | | MARKETPLACEEXPORT | Datenumfang COMPLETE ergänzt um die Daten für den Börsenexport (nur SilverDAT 3 PRO). | | EXTENDEDBYTRADING | Datenumfang COMPLETE ergänzt um die Unterelemente TradingActivity und TradingAdditional mit den Handelsdaten der Methoden setPurchaseData, setAdmissionData und setSalesData (nur SilverDAT 3 PRO). | | COMPLETE | Defaultwert; Standard Datenumfang für die Datenrückgabe | | NOVALUATIONRESULT | Datenrückgabe ohne die Unterelemente Valuation und VAT | | ENRICHED | Benennungen entfallen teilweise, aber mit den Bennennungen der Ausstattungen | | BASE | Datenrückgabe ganz ohne Benennungen | | SIMPLE | Bei diesem Wert entfallen zusätzlich bestimmte Unterelemente, wie zum Beispiel: CustomerAddress, TradingData, RepairCalculation, RepairOrder, RegistratinData, Engine, Equipment oder TechInfo. | | NONE | Datenrückgabe entweder mit leerem Rahmen, nur mit der DossierId oder nur mit DossierType. | | String | optional; definiert die Datenausgabemenge |  |  |
