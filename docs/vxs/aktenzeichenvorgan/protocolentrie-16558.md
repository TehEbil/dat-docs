---
title: "ProtocolEntriesWithRemoval"
topic_id: "16558"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > Kalkulationsergebnisse CalcResult > CalculationProtocol > ProtocolEntriesWithRemoval"
---

# ProtocolEntriesWithRemoval

Felder:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| DATProcessId | Integer, optional | Die DVN zu dem Hinweis |
| RepairType | String, optional | Art der Reparatur (RC, z.B. replace) |
| Description | String, optional | Beschreibung für den Hinweis (z.B. Bezeichnung des Ersatzteils) |
| ContainedInDATProcessId | Integer, optional | DATProcessId der Position, durch die die Position entfernt wurde. Z.B. eine Arbeit, die die Position umfasst |
| ContainedInRepairType | String, optional | Der RepairType der Position, durch die die Position entfernt wurde |
| ContainedInLacquerLevel | Integer, optional | Die Lackstufe der Position, durch die die Position entfernt wurde |
| LacquerLevel | Integer, optional | Lackstufe (Nur bei Logik lacquer) |
| Logic | String, optional | Logik des Hinweises (z.B. parts, lacquer, work) |
