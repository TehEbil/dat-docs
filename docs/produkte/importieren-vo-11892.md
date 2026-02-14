---
title: "Importieren von manuellen Positionen"
topic_id: "11892"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Importieren von manuellen Positionen"
---

# Importieren von manuellen Positionen

Mit der Schnittstellenfunktion importManualPositions werden die eigenen, wiederkehrenden "Manuelle Positionen" (Material- und/oder Lohnpositionen)
importiert.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| DatCategory | [DatCategory](#showid/11911 "DatCategory") |  | Liste von Kategorien mit Namen und darunterliegenden manuellen Positionen |
| DatPosition | [DatPosition](#showid/11912 "DatPosition") |  | Liste von unkategorisierten Positionen |

Rückgabe

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| impotSuccessful | Boolean | Ist der Wert auf "true" gesetzt, deutet dies darauf hin, dass die gewünschten manuellen Positionen erfolgreich importiert worden sind. |
