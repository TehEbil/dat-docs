---
title: "Kopieren eines Auftrags"
topic_id: "9346"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Kopieren eines Auftrags"
---

# Kopieren eines Auftrags

Die CopyClaim-Funktion wird verwendet, um Daten aus einem bestehenden Auftrag zu kopieren
und basierend auf den bereitgestellten Einstellungen einen neuen Auftrag zu erstellen.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| claimId | Long |  | Auftrags ID des zu kopierenden Auftrags | X |
| templateId | Long |  | Ziel Template Id | X |
| referenceNumber | String |  | Name der neu angelegten Auftragskopie | X |
| copySettings | List<String> | CLAIM\_DATA  VEHICLE\_DATA  ADDRESS\_DATA  CALCULATION\_DATA  INSURANCE\_DATA  PARTNERS  PARTS\_SELECTION  PROCESS\_RELATED\_DATA  ATTACHMENTS | Liste der Einstellungen, die angeben, welche Daten kopiert werden sollen | X |

Rückgabe

Claim ID des neuen Auftrags
