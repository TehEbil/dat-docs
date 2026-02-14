---
title: "Abruf aller existierenden Druckvorlagen"
topic_id: "2349"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abruf aller existierenden Druckvorlagen"
---

# Abruf aller existierenden Druckvorlagen

Die Funktion getTemplates() listet Informationen über alle Druckvorlagen für die entsprechende Kundennummer auf.

Parameter

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| locale | locale, optional | [Element locale](../../allgemein/dat-developers-gui/element-locale-1352.md) |

Rückgabe

In der Antwort werden die Informationen aller Druckvorlagen, in 1:n Knoten ExportProduct, zurückgegeben.

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| ExportProduct | complextype, [ExportProduct](exportproduct-19507.md)[] | Informationen zu allen Druckvorlagen |
