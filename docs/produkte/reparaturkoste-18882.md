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
| [dossiers](#showid/1369 "Aktenzeichen/Vorgänge (Dossiers)") | [Dossiers[]](#showid/1369 "Aktenzeichen/Vorgänge (Dossiers)"), Pflicht | Dossiers ist ein übergeordneter Knoten und enthält das sogennante [dossier](#showid/1371 "Aktenzeichen/Vorgang (Dossier)"). | [dossier](#showid/1371 "Aktenzeichen/Vorgang (Dossier)") ([Dossier](#showid/1371 "Aktenzeichen/Vorgang (Dossier)"), Pflicht): enthält das Fahrzeugobjekt, die Arbeitslöhne, Kalkulationsfaktoren, Schadenspositionen und  das Kalkulationssergebnis. |

Rückgabe

Die Antwort ist eine komplette Kalkulation als [Dossier im VXS-Format](#showid/1371 "Aktenzeichen/Vorgang (Dossier)").

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| [Dossier](#showid/1371 "Aktenzeichen/Vorgang (Dossier)") | [Dossier](#showid/1371 "Aktenzeichen/Vorgang (Dossier)") | Enthält das Fahrzeugobjekt, die Arbeitslöhne, Kalkulationsfaktoren, Schadenspositionen und  das Kalkulationssergebnis |
