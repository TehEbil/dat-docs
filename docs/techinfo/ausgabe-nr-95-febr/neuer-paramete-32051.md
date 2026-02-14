---
title: "Neuer Parameter Reset für die Funktion setValueInfluencingFactors"
topic_id: "32051"
breadcrumb: "Technische Informationen > Ausgabe Nr. 95 Februar 2026 > Fahrzeugbewertung > SilverDAT 3 PRO > Erweiterungen > Neuer Parameter Reset für die Funktion setValueInfluencingFactors"
---

# Neuer Parameter Reset für die Funktion setValueInfluencingFactors

Beim Aufruf der Funktion setValueInfluencingFactors des ValuationN-Services kann für freie Aktenzeichen ab sofort für wertbeeinflussende Faktoren optional
der neue Parameter Reset übergeben werden.

Mit dem neuen Parameter kann analog zur Webanwendung bestimmt werden, ob die Handelsspanne
aus den wertbeeinflussenden Faktoren oder aus dem prozentualen Wert bzw. Sachverständigenwert
berechnet werden soll.

| Parameter | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| Reset | Boolean | Zurücksetzen eines benutzerdefinierten wertbeeinflussenden Faktors auf DAT-Standard. | true = Wenn für den wertbeeinflussenden Faktor kein Netto- und/oder Brutto-Wert übergeben wurde, wird der wertbeeinflussende Faktor auf DAT-Standard zurückgesetzt. false (default) = Der wertbeeinflussende Faktor wird nicht auf DAT-Standard zurückgesetzt. |  |

Weitere Details zur Funktion setValueInfluencingFactors entnehmen sie bitte dem Kompendium.

Bitte führen Sie entsprechende Anpassungen in Ihren Anwendungen durch, wenn Sie die
neue Funktionalität nutzen möchten.
