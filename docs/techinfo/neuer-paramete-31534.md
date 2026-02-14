---
title: "Neuer Parameter für die Finance-Funktion getBatteryValuationParams"
topic_id: "31534"
breadcrumb: "Technische Informationen > Ausgabe Nr. 94 Dezember 2025 > Fahrzeugbewertung > valuateFinance > Erweiterungen > Neuer Parameter für die Finance-Funktion getBatteryValuationParams"
---

# Neuer Parameter für die Finance-Funktion getBatteryValuationParams

Beim Aufruf der Funktion getBatteryValuationParams des DossierN-Services kann ab sofort optional der neue Parameter DeterminatedDate übergeben werden.

| Parameter | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| DeterminatedDate | Date | Stichtag zur Prüfung der Möglichkeit der erweiterten Bewertung für Elektrofahrzeuge. | YYYY-MM-DD |  |

Der Parameter DeterminatedDate  wird auch in der Response ausgegeben, wenn er im Request übergeben wurde.

Bitte führen Sie entsprechende Anpassungen in Ihren Anwendungen durch, wenn Sie die
neue Funktionalität nutzen möchten.
