---
title: "Auflisten der Auftragshistorie"
topic_id: "11889"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Auflisten von Informationen innerhalb eines Auftrags > Auflisten der Auftragshistorie"
---

# Auflisten der Auftragshistorie

Die Funktion listContractHistory listet alle Ereignisse innerhalb derAuftragshistorie auf wie z.B. Statusänderungen,
Kommentare, Benutzerzuweisungen usw.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| contractID | String |  | ID des Auftrags | X |
| historyEvent | HistoryEvent | statusChange  comment  assignedUser  assignedPartner  resignedUser  documentsUploaded  documentDeleted  settlementsChosen  dataEdited  unAssignedPartner  GDVSent  dirtyClaim  GDVIncoming  emailSent  audatexImport  changedAdditionalCosts    valuation  purchaseOffer  purchase  admission  salesOffer  sales  reservation    claimUpdated    emailRequestAssigned  GDVGeneral  valuation\_vehicle\_changed  valuation\_equipment\_changed  repair\_vehicle\_changed  repair\_equipment\_changed    assignedPartner\_role\_REPAIRER  assignedPartner\_role\_INSURANCE  assignedPartner\_role\_EXPERT  assignedPartner\_role\_MANUFACTURER  assignedPartner\_role\_GUEST  assignedPartner\_role\_LAWYER  assignedPartner\_role\_FLEET  assignedPartner\_role\_OTHER\_PARTNER  fastTrackCalculated  repair\_calculation  assignedPartner\_role\_CG\_REPAIRER  assignedPartner\_role\_CG\_EXPERT  fastTrackInputChanged    assignedPartner\_role\_PAINT\_SHOP  assignedPartner\_role\_TOWING\_SERVICE  assignedPartner\_role\_BANK  assignedPartner\_role\_LEASING\_COMPANY  infoekspertValuation | Liste der vorhandenen Ereignisse |  |
| senderRoles | List<CustomerRole> | REPAIRER  INSURANCE  EXPERT  MANUFACTURER  GUEST  LAWYER  FLEET  OTHER\_PARTNER  SERVICE\_PROVIDER  CG\_REPAIRER  CG\_EXPERT  PAINT\_SHOP  TOWING\_SERVICE  BANK  LEASING\_COMPANY | Liste der vorhandenen Rollen |  |
| producedFrom | Date |  | Datum des Ereignisses in der Historie |  |

Rückgabe

Liste der Ereignisse eines Auftrags
