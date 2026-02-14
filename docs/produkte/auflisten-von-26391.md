---
title: "Auflisten von Dokumenten"
topic_id: "26391"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Auflisten von Dokumenten"
---

# Auflisten von Dokumenten

Die Funktion listAttachments() ermöglicht die Auflistung der Dokumente für einen bestimmten Vorgang.

Parameter

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| contractID | Long, Pflicht | Vorgangsnummer |

Rückgabe

| Element | Typ | Beschreibung |
| --- | --- | --- |
| <Attachments> | Attachment[] | Enthält eine Liste der Anhänge, die für die entsprechende Vorgangsnummer hinterlegt sind. |

Attachment

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| AttachmentId | Integer | Die ID eines vorhandenen oder gerade erstellten Dokuments |
| Filename | String | Dateiname |
| Suffix | String | Dateiendung |
| B64Data | String | b64 formatierter String des Dokuments |
