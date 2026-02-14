---
title: "Zuweisen eines Partners anhand der Kundennummer"
topic_id: "2585"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Zuweisen von Benutzern und Partnern zu einem Auftrag > Zuweisen eines Partners anhand der Kundennummer"
---

# Zuweisen eines Partners anhand der Kundennummer

Die Funktion assignPartnerByCustomerNumber weist einen Partner (der über die Kundennummer identifiziert wird) unter einer bestimmten
Rolle (rolePartner) einem Auftrag hinzu.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| contractId | Long |  | Identifizierungsnummer des Auftrags | X |
| customerNumber | String |  | Kundennummer des zuweisenden Partners | X |
| rolePartner | String | REPAIRER, INSURANCE, EXPERT, MANUFACTURER | Rolle des Partners der zugewiesen werden soll | X |

Rückgabe

- True: Falls Zuweisung erfolgreich

- False: Falls Partner schon zugewiesen wurde.
