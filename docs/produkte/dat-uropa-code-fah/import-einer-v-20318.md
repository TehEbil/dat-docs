---
title: "Import einer VIN-Abfrage"
topic_id: "20318"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Fahrzeugidentifikation anhand VIN (VIN-Abfrage) > Import einer VIN-Abfrage"
---

# Import einer VIN-Abfrage

Seit geraumer Zeit ist es möglich, das Ergebnis einer VIN-Abfrage zu importieren ohne
das dabei in der Weboberfläche das VIN-Abfrage Buch-Symbol und die damit verbundenen
Daten verloren gehen.

Die Herstellercodes aus der VIN-Abfrage gewinnen mehr und mehr Bedeutung bei der Ersatzteilbestimmung
in unseren Anwendungen der Schadenskalkulation!

Eine entscheidende Rolle beim Import spielt dabei das TokenOfVinResult. Dieses Token verhindert eine missbräuchliche Verwendung und die Manipulation des
Ergebnisses aus der VIN-Abfrage.

Voraussetzungen:

- Das TokenOfVinResult darf nicht älter als 7 Tage sein
- Im Element <VINResult> dürfen keinerlei Veränderungen stattgefunden haben
- Die Kundennummer und die InterfacePartnerNummer müssen übereinstimmen
- Der €uropa-Code, Container und Bauzeit in <Vehicle> muss mit den Daten in <VINResult> übereinstimmen.
- Im Umfeld myClaim muss zusätzlich der Wert von VinActive auf true gesetzt und das Element SubModelVariant vorhanden sein.

Mit dem Release 2025-001 wird das VXS-Element VinActive entfernt. Die Funktion übernimmt
das Element TokenOfVinResult.

Szenarien:

1. Webanwendung Export -> Webanwendung Import  
   Kundennummer muss übereinstimmen
2. Schnittstelle Export -> Webanwendung Import  
   Kundennummer muss übereinstimmen
3. Schnittstelle Export -> Schnittstelle Import  
   Kundennummer und InterfacePartnerNummer müssen übereinstimmen
4. Webanwendung Export -> Schnittstelle Import  
   Dieses ist aus technischen Gründen aktuell leider nicht möglich!

Produkte und Funktionen die den Import unterstützen

| Produkt | Funktion |
| --- | --- |
| CalculatePro / CalculateExpert | importDossier |
| valuateFinance | createDossierN changeDossierN |
| valuateExpert / PlusPartner | createDossierN changeDossierN |
| SD3 PRO | createValuationN changeValuationN  doValuationInMemoryN |
| myClaim | createOrUpdateContractN |

Hinweis: Beim Export einer VIN-Abfrage sollte in jedem Fall das TokenOfVinResult enthalten sein. Sollten Sie Probleme bein Import einer VIN-Abfrage haben, wenden
Sie sich bitte an unsere DAT Hotline interfaces@dat.eu
