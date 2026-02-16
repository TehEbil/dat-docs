---
title: "Auflisten der Anhänge"
topic_id: "2591"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Auflisten von Informationen innerhalb eines Auftrags > Auflisten der Anhänge"
---

# Auflisten der Anhänge

Die Funktion listAttachmentsOfContract ladet alle Anhänge eines Auftrags herunter. Dabei können durch die optionalen Parameter
documentTypes, attachmentTypes die Art und newerThan die Zeit des Hochladedatums der Anhänge eingeschränkt werden.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| contractID | String |  | ID des Auftrags | X |
| attachmentTypes | String[] Array | Calculation, attachment, graphicalPartSelection | Art eines Anhangs.  Calculation = Anhänge die aus einem SDII import kommen    attachment = Anhänge innerhalb der Kalkulation in myClaim    graphicalPartSelection = Anhänge innerhalb der Teileauswahl in myClaim |  |
| documentTypes | String[] Array | vehicleStatusReport, insuranceDocuments, datNetInvoiceDocument, datNetInspectionReport |  |  |
| newerThan | Date |  | Falls nicht null werden nur die Anhänge angezeigt die neuer als der übergebene „newerThan" Datumswert sind. |  |
| assignedTags | CustomTagItem |  | Tags zur Kategorisierung von Anhängen |  |

Element vxs:assignedTags

| Name | Datentyp | Beschreibung | Mögliche Werte | Pflicht |
| --- | --- | --- | --- | --- |
| id | Integer | Identifizierungsnummer des Merkmals |  | Falls identification nicht übergeben wird, ist die Übergabe der id pflicht. |
| description | String | Beschreibung des Merkmals |  |  |
| identification | String | Identifikationsname des Merkmals |  | Falls id nicht übergeben wird, ist die Übergabe der identification pflicht. |

Rückgabe

Liste der angefragten Anhänge. Dabei besteht jeder zurückgegebene Datensatz aus dem
eigentlichen Anhang (binäre Datei) und dessen Meta-Informationen.
