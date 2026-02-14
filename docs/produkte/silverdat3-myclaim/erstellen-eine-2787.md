---
title: "Erstellen eines neuen Auftrags für externe ID"
topic_id: "2787"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Erstellen eines neuen Auftrags für externe ID"
---

# Erstellen eines neuen Auftrags für externe ID

Mit der Funktion createContractForExternalID kann ein neuer Auftrag erstellt werden und dieser gleichzeitig einem Kunden basierend
auf seiner externen ID zugewiesen werden.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| contractId | Long |  | Identifikationsnummer des Auftrags. |  |
| contractType | String | eneral, glass, ania, vro\_calculation, temporary, vsr\_order, vro\_domus\_calculation | Mögliche Auftragstypen  (Stand 12.2014) | x |
| networkType | String | OPEN, VW, HUK, NISSAN, MOBILE, IFERT, AUDI, POSTFLEET, DUERKOP,... | Mögliche Netzwerktypen | x |
| Dossier | Dossier |  | Element das die Vehicle eXchange Struktur (VXS) beinhaltet | x |
| externalId | String |  | Externe ID für die identifizierung einer Werkstatt | x |

Rückgabe

ID (Auftrags ID) des neu erstellten Auftrags.
