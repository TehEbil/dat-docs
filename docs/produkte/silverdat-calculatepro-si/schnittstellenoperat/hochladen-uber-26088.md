---
title: "Hochladen, Überschreiben und Löschen von Dokumenten"
topic_id: "26088"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Hochladen, Überschreiben und Löschen von Dokumenten"
---

# Hochladen, Überschreiben und Löschen von Dokumenten

Die Funktion manageAttachments() ermöglicht das Hochladen, Überschreiben und Löschen von Dokumenten in einem bestimmten
Vorgang.

Parameter

| Name / Elternelement | Datentyp | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| contractID | Long, Pflicht |  | Vorgangsnummer |
| crud | String, Pflicht | "UPLOAD", "OVERWRITE", "DELETE" | "UPLOAD": importiert Dokumente in ein existierendes Dossier.    "OVERWRITE": ersetzt bzw. überschreibt Dokumente innerhalb eines Dossiers.    "DELETE": löscht einzelne Dokumente innerhalb eines Dossiers. |
| attachments | Attachment[] |  | Anhänge. Mehrfach Übergabe möglich |

Attachment

| Name / Elternelement | Datentyp | Beschreibung |
| --- | --- | --- |
| Filename | String | Dateiname |
| Suffix | String | Dateiendung |
| B64Data | String | b64 formatierter String des Dokuments |
| AttachmentId | Integer | Die ID eines vorhandenen oder gerade erstellten Dokuments |

Rückgabe

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| uploadStatusList | uploadStatus[] | Enthält eine Liste mit dem jeweiligen Status der Aktion, die für den entsprechenden Anhang durchgeführt worden ist(Hochladen, Überschreiben oder Löschen) |

uploadStatus

| Name / Elternelement | Datentyp | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| Attachment | Attachment |  | Vorgangsnummer |
| message | String | Upload successful | Upload failed | Deletion successful | Deletion failed | Gibt an, ob das Dokument hochgeladen/gelöscht wurde oder nicht. |
| status | String | 200 | 400 | HTTP-Statuscode, der anzeigt, ob der Upload/Löschvorgang erfolgreich war oder nicht. |
