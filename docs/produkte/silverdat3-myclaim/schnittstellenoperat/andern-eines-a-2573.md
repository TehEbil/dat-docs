---
title: "Ändern eines Auftragsstatus"
topic_id: "2573"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Ändern eines Auftragsstatus"
---

# Ändern eines Auftragsstatus

Die Funktion changeContractStatus ändert den Status eines vorhandenen Auftrags. Der Vorgang scheitert falls der zu setzende
statusType im Auftrag nicht anwendbar ist. D.h. aufgrund eines vordefinierten Arbeitsablaufs
kann es vorkommen dass innerhalb eines bestimmten Status nicht jeder beliebige Status
als Nachfolger gesetzt werden kann. Somit würde im Falle eines ungültigen Nachfolgestatus
ein Fehler ausgegeben werden.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| contractId | Long |  | ID des Auftrags | X |
| statusType | String | custom, opened, uploaded, published, reUploaded, closed, checkup, rejected, onHold, approved, deleted, accepted, technicalError, reportCreated, pleaseCorrect, atAttorneyCSP, releasedCsp, sentCsp, received, invoiced, repaired, payed, assigned | Status Typ | X |
| note | String |  | Optionaler Parameter für Kommentare in der Historie bei Statusänderungen |  |
| comments | List<Comment> |  | Kommentare z.B. von einer Versicherung |  |
| status | Status | type, identification | type =  identification = |  |

Rückgabe

Textinformation das der übergebene Status dem bestimmten Auftrag zugeordnet wurde.
