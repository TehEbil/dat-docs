---
title: "Löschen eines Auftrags"
topic_id: "22542"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Löschen eines Auftrags"
---

# Löschen eines Auftrags

Die deleteContract Funktion ermöglicht es, einen bestehenden Auftrag basierend auf der Auftrags-ID zu
löschen. Ein Grund für das Löschen sowie ein optionaler Kommentar können ebenfalls
angegeben werden.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| DeleteReason | Datentyp | OTHER, CUSTOMER\_REQUEST, PROCEDURE\_CLEANING | Grund für das Löschen des Auftrags | X |
| ContractId | Long |  | ID des zu löschenden Auftrags | X |
| Comment | String |  | Ein optionaler Kommentar zum Löschen des Vertrags. |  |

Rückgabe

True wenn Löschen Erfolgreich.
