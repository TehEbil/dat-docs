---
title: "Reparaturkostenkalkulation ohne Speicherung"
topic_id: "18882"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Reparaturkostenkalkulation ohne Speicherung"
---

# Reparaturkostenkalkulation ohne Speicherung

Mit der Funktion calculateN() wird eine Reparaturkostenkalkulation durchgeführt, ohne einen Vorgang in der Anwendung
zu speichern.

Diese Funktion calculateN() unterstützt im Gegensatz zu der alten Funktion calculate() die gängige standardisierte VXS-Struktur.

Parameter

| Name / Elternelement | Datentyp | Beschreibung | Kind-Elemente |
| --- | --- | --- | --- |
| locale | complexType, Locale | Datenland, Land- und Spracheinstellung |  |
| [dossiers](../../../vxs/aktenzeichenvorgange-doss/index.md) | [Dossiers[]](../../../vxs/aktenzeichenvorgange-doss/index.md), Pflicht | Dossiers ist ein übergeordneter Knoten und enthält das sogennante [dossier](../../../vxs/aktenzeichenvorgange-doss/aktenzeichenvorgang/index.md). | [dossier](../../../vxs/aktenzeichenvorgange-doss/aktenzeichenvorgang/index.md) ([Dossier](../../../vxs/aktenzeichenvorgange-doss/aktenzeichenvorgang/index.md), Pflicht): enthält das Fahrzeugobjekt, die Arbeitslöhne, Kalkulationsfaktoren, Schadenspositionen und  das Kalkulationssergebnis. |

Rückgabe

Die Antwort ist eine komplette Kalkulation als [Dossier im VXS-Format](../../../vxs/aktenzeichenvorgange-doss/aktenzeichenvorgang/index.md).

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| [Dossier](../../../vxs/aktenzeichenvorgange-doss/aktenzeichenvorgang/index.md) | [Dossier](../../../vxs/aktenzeichenvorgange-doss/aktenzeichenvorgang/index.md) | Enthält das Fahrzeugobjekt, die Arbeitslöhne, Kalkulationsfaktoren, Schadenspositionen und  das Kalkulationssergebnis |
