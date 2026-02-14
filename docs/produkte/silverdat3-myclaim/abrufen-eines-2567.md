---
title: "Abrufen eines Auftragsstatus"
topic_id: "2567"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Abrufen eines Auftragsstatus"
---

# Abrufen eines Auftragsstatus

Die Funktion getContractStatus ermöglicht es alle Informationen eines Auftragsstatus abzurufen wie z.B Versendet,
Freigegeben etc.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| contractId | Long |  | Identifikationsnummer des Auftrags | X |

Rückgabe

Zurückgegeben werden folgende Statusinformationen eines Auftrags

- Symbolname des Status
- Anzeigename des Status
- Netzwerktyp
- Status ID
- Statustyp
