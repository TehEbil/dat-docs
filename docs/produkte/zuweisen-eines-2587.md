---
title: "Zuweisen eines Partners anhand der internen Identifikation"
topic_id: "2587"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Zuweisen von Benutzern und Partnern zu einem Auftrag > Zuweisen eines Partners anhand der internen Identifikation"
---

# Zuweisen eines Partners anhand der internen Identifikation

Die Funktion assignPartnerByInternalIdentification weist einen Partner (der über eine interne Identifikationsnummer identifiziert wird)
unter einer bestimmten Rolle wie z.B. Versicherer, Hersteller, Sachverständiger, Werkstatt
einem Auftrag hinzu. Die optionale interne Identifikation wird beim Hinzufügen eines
neuen Partners vom Benutzer vergeben.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| contractId | Long |  | Identifizierungsnummer des Auftrags | X |
| internalIdentification | String |  | Interne Identifizierungsnummer des Partners der zugeordnet werden soll. | X |
| rolePartner | String | REPAIRER, INSURANCE, EXPERT, MANUFACTURER | Rolle des Partners der zugewiesen werden soll | X |

Rückgabe

- True: Falls Zuweisung erfolgreich

- False: Falls Partner schon zugewiesen wurde.
