---
title: "Neuer Parameter für die Expert-Funktion getBatteryValuationParams"
topic_id: "31533"
breadcrumb: "Technische Informationen > Ausgabe Nr. 94 Dezember 2025 > Fahrzeugbewertung > valuateExpert/valuateExpertPlusPartner > Erweiterungen > Neuer Parameter für die Expert-Funktion getBatteryValuationParams"
---

# Neuer Parameter für die Expert-Funktion getBatteryValuationParams

Beim Aufruf der Funktion getBatteryValuationParams des Dossier1N-Services kann ab sofort optional der neue Parameter DeterminatedDate übergeben werden.

Wenn er nicht übergeben wird, wird weiterhin das Tagesdatum als Stichtag herangezogen.

| Parameter | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| DeterminatedDate | Date | Stichtag zur Prüfung der Möglichkeit der erweiterten Bewertung für Elektrofahrzeuge. | YYYY-MM-DD |  |

Der Parameter DeterminatedDate  wird nun auch in der Response ausgegeben.

Bitte führen Sie entsprechende Anpassungen in Ihren Anwendungen durch, wenn Sie die
neue Funktionalität nutzen möchten.
