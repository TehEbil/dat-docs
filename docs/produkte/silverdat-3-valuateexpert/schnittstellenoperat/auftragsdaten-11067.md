---
title: "Auftragsdaten anlegen"
topic_id: "11067"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Funktionen für Sachverständige > Funktionsumfang > Auftragsdaten anlegen"
---

# Auftragsdaten anlegen

Mit der Funktion setOrderOpeningDetails legen oder ändern Sie die Auftragsdaten zu einem bestehenden Vorgang.

Parameter setOrderOpeningDetails

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| DossierId | Long | Eindeutige Vorgangskennung | numerisch | X |
| ContractNumber | String | Vertragsnummer |  |  |
| CustomerKind | String | Kundenart | RQSTR=Auftraggeber  DVR=Halter  WSHP=Autohaus Werkstatt  LCUST=Leasing Kunde |  |
| DateOfVisit | dateTime | Datum | JJJJ-MM-DD |  |
| LicensePlateNumber | String | Amtliches Kennzeichen |  |  |
| LocationOfVisit | String | Ort der Besichtigung |  |  |
| OrderNumber | String | Auftragsnummer |  |  |
| ProcedureName | String | Vorgangsname |  |  |
| VisitedBy | String | Kundennummer des Besichtigers und optional kann ein String angegeben werden, dass in den Ausdruck (über die Methode exportDossierN) angezeigt wird | numerisch |  |
