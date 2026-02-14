---
title: "Auflisten der Historie eines Vorgangs-Ereignisses"
topic_id: "10937"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Auflisten der Historie eines Vorgangs-Ereignisses"
---

# Auflisten der Historie eines Vorgangs-Ereignisses

Diese Funktion listet historisch die gängigsten Ereignisse wie z.B. die Kommentare,
Statusänderungen usw. zu einem Vorgang auf.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| contractId | long |  | Auftrags ID | X |
| producedFrom | Date |  | Datum des Ereignisses |  |
| historyEvent | HistoryEvent | statusChange  comment  assignedUser  assignedPartner  resignedUser  documentsUploaded  documentDeleted  settlementsChosen  dataEdited  unAssignedPartner  GDVSent  dirtyClaim  GDVIncoming  emailSent  audatexImport  changedAdditionalCosts  valuation  purchaseOffer  purchase  admission  salesOffer  sales  reservation  claimUpdated  emailRequestAssigned  GDVGeneral  valuation\_vehicle\_changed  valuation\_equipment\_changed  repair\_vehicle\_changed  repair\_equipment\_changed  assignedPartner\_role\_REPAIRER  assignedPartner\_role\_INSURANCE  assignedPartner\_role\_EXPERT  assignedPartner\_role\_MANUFACTURER  assignedPartner\_role\_GUEST  assignedPartner\_role\_LAWYER  assignedPartner\_role\_FLEET  assignedPartner\_role\_OTHER\_PARTNER  fastTrackCalculated  repair\_calculation  assignedPartner\_role\_CG\_REPAIRER  assignedPartner\_role\_CG\_EXPERT  fastTrackInputChanged  assignedPartner\_role\_PAINT\_SHOP  assignedPartner\_role\_TOWING\_SERVICE  assignedPartner\_role\_BANK  assignedPartner\_role\_LEASING\_COMPANY  infoekspertValuation | Ereignis Typ der Historie |  |
| senderRoles | List<CustomerRole> | REPAIRER  INSURANCE  EXPERT  MANUFACTURER  GUEST  LAWYER  FLEET  OTHER\_PARTNER  SERVICE\_PROVIDER  CG\_REPAIRER  CG\_EXPERT  PAINT\_SHOP  TOWING\_SERVICE  BANK  LEASING\_COMPANY | Liste der Rollen die das Ereignis erstellt haben |  |

Rückgabe

Verlaufsergebnisse eines Auftrags (Kommentare, Statusänderungen etc.)
