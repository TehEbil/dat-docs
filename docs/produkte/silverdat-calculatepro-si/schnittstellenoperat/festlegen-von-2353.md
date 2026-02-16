---
title: "Festlegen von Überschläge Kalkulationswerte"
topic_id: "2353"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Festlegen von Überschläge Kalkulationswerte"
---

# Festlegen von Überschläge Kalkulationswerte

Die Funktion setBlanketCalculation gilt nur für das Produkt calculateExpert. Hiermit werden die Werte für die sogenannte Überschlägige Kalkulation gesetzt. Diese
Funktion ist nur möglich für bereits kalkulierte Vorgänge.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| dossierId | String, Pflicht |  | Die eindeutige Kennung eines Vorgangs. |
| labourCosts | String, Optional |  | Arbeitskosten |
| lacquerCosts | String, Optional |  | Lackkosten |
| sparePartsCosts | String, Optional |  | Ersatzteilkosten |

Rückgabe

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| blanketCalculation | blanketCalculation |  |
| message | String | Diese Nachricht bestätigt, dass die gewünschten Werte für die Überschlägige Kalkulation des abgefragten Vorgangs erfolgreich abgespeichert sind. |
