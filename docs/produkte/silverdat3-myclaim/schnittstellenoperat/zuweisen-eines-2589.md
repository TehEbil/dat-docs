---
title: "Zuweisen eines Partners"
topic_id: "2589"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Zuweisen von Benutzern und Partnern zu einem Auftrag > Zuweisen eines Partners"
---

# Zuweisen eines Partners

Die Funktion assignPartnerToContract weist einen Partner anhand der Partner ID unter einer bestimmten Rolle (Versicherer,
Werkstatt, Hersteller, Sachverstδndiger) einem Auftrag hinzu.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| contractId | Long |  | Identifizierungsnummer des Auftrags | X |
| partnerId | String |  | ID des Partners | X |
| rolePartner | String | REPAIRER, INSURANCE, EXPERT, MANUFACTURER | Rolle des Partners der zugewiesen werden soll | X |

Rückgabe

- true: Falls Zuweisung erfolgreich

- false: Falls Partner schon zugewiesen wurde.
