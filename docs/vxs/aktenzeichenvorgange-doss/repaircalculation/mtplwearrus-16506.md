---
title: "MTPLWearRus"
topic_id: "16506"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > RepairPositions > RepairPosition > MTPLWearRus"
---

# MTPLWearRus

Das russische MTPL Verschleiß enthält die folgende Elemente:

Felder

| Element | Typ | Beschreibung | Mögliche Werte |
| --- | --- | --- | --- |
| WearGroup | String, optional | Gruppe Verschleiß | "1" - Verschleißfrei  "3" - Reifenverschleiß  "6" - Benutzerdefinierte Verschleißberechnung (WearAge,WearMileage,WearAdditional)  "7" - Manuelle Verschleiß von Feld "WearPercent" |
| WearAge | Integer, optional | Alter des Ersatzteils für kundenspezifische Berechnung |  |
| WearMileage | Integer, optional | Kilometerstand des Ersatzteils für kundenspezifische Berechnung |  |
| WearAdditional | Decimal, optional | zusätzliche Verschleißteile für kundenspezifische Berechnung |  |
| WearPercent | Decimal, optional | Manueller Verschleißprozentsatz für bestimmte Ersatzteile |  |
| WearPrice | Decimal, optional | Veraltet, derzeit nicht kompatibel |  |
