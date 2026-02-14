---
title: "Auflisten der Anhangsordner"
topic_id: "2603"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Auflisten von Informationen innerhalb eines Auftrags > Auflisten der Anhangsordner"
---

# Auflisten der Anhangsordner

Die Funktion listAttachmentFolders liefert Informationen, welcher Anhangsordner einem Auftrag (Claim) zugeordnet ist.

Die Anhangsordner-Struktur entspricht der Konfiguration ders Ordnerstruktur in der
Dokumentenverwaltung in myClaim.

```
<folderID> - is internal unique folder ID:
<folderIdentification> - is internal ID
<folderName> - is Document
<isOnlySingleAttachmentEnabled> - is single File
<enabledFileExtensions> - file extensions
```

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| contractId | Long |  | Identifizierungsnummer des Auftrags | x |

Rückgabe

Liste der Anhangsordner-Struktur mit der Information der Ordner, die dem Auftrag (Claim) zugeordnet sind.
