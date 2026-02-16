---
title: "Hochladen von Anhängen anhand einer Identifikation"
topic_id: "2579"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Hochladen von Anhängen anhand einer Identifikation"
---

# Hochladen von Anhängen anhand einer Identifikation

Mit der Funktion uploadAttachmentByIdentification können Dokumente in einem bestimmten Ordner hochgeladen werden falls die interne Ordner
Identifikation (documentType) bekannt ist.

Request uploadAttachmentByIdentification

| Name | Datentyp | Beschreibung | Mögliche Werte | Pflicht |
| --- | --- | --- | --- | --- |
| contractId | Long | Identifizierungsnummer des Auftrags |  | X |
| attachmentItem | AttachmentItem | Anhangselement das die eigentlichen Anhänge beinhaltet wie Name, binäre Datei Typ etc. |  | X |

Element vxs:attachmentItem

| Name | Datentyp | Beschreibung | Mögliche Werte | Pflicht |
| --- | --- | --- | --- | --- |
| fileName | String | Name des Anhangs |  | X |
| mimeType | String | Gibt an, welcher Typ der hochgeladenen Datei (z.B. "image/jpeg" oder "application/pdf") für die korrekte Interpretation und Verarbeitung durch den Server und die Anwendung sorgt. | text/html  image/jpeg  image/png  .  .  .  . |  |
| dataSize | Integer | Kann gesetzt werden damit der Empfänger weiß, wie viel Daten erwartet werden und wie viel Speicherplatz bereitgestellt werden muss, um die Daten aufzunehmen. Es ermöglicht z.B. auch Fehlerüberprüfungen, um sicherzustellen, dass alle Daten korrekt übertragen wurden und keine Informationen verloren gegangen sind. |  |  |
| binaryData | Base64 | Base64 encodedierter Inhalt der Datei |  | X |
| published | DateTime | Veröffentlichungsdatum des Anhangs |  |  |
| uploaded | DateTime | Datum des Uploadzeitpunkts |  |  |
| documentType | String | Identifikationsname des Anhangsordners |  | X |
| documentID | Long | ID des Anhangsordners. Bei der Übergabe von 0 werden Anhänge im Ordner "Other documents" hochgeladen. |  |  |
| attachmentType | String | Dieses Element kann benötigt, werden um den Typ des Anhangs (z. B. Bild, Dokument usw.) zu identifizieren und zu verarbeiten. Diese Information kann z.B. wichtig sein, um sicherzustellen, dass der Empfänger in der Lage ist, den Anhang ordnungsgemäß zu öffnen und anzuzeigen, und um eventuelle Fehler oder Inkompatibilitäten zu vermeiden. |  |  |
| uploaderId | Long | Id des Benutzers der den Upload durchgeführt hat |  |  |
| uploaderCustomerNumber | String | Kundennummer die den Upload durchgeführt hat. |  |  |
| uploaderIdentification | String | Identifikation des Uploaders |  |  |
| uploaderRole | String | Rolle des Uploaders |  |  |
| uploaderName | String | Name des Uploaders |  |  |
| uploaderUserId | Long | Benutzer ID des Uploaders |  |  |
| uploaderUserLogin | String | Benutzer Login des Uploaders |  |  |
| uploaderUserName | String | Benutzername des Uploaders |  |  |
| assignedTags | CustomTagItem | Tags zur Kategorisierung von Anhängen |  |  |

Mit dem Element assignedTags, können Anhänge in den Anhangsordnern mit Merkmalen versehen werden, so das diese
bei Bedarf kategorisiert bzw. besser unterschieden werden können.

Element vxs:assignedTags

| Name | Datentyp | Beschreibung | Mögliche Werte | Pflicht |
| --- | --- | --- | --- | --- |
| id | Integer | Identifizierungsnummer des Merkmals |  | Mindestens einer der zwei Parameter id oder identification muss einen Wert enthalten. |
| description | String | Beschreibung des Merkmals |  |  |
| identification | String | Identifikationsname des Merkmals |  | Mindestens einer der zwei Parameter id oder identification muss einen Wert enthalten. |

Rückgabe

Gibt true zurück falls Anhang erfolgreich hochgeladen wurde.
