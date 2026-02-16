---
title: "Neuer Parameter MarginFromValueInfluencingFactors für die Funktion setValueInfluencingFactors"
topic_id: "32018"
breadcrumb: "Technische Informationen > Ausgabe Nr. 95 Februar 2026 > Fahrzeugbewertung > SilverDAT 3 PRO > Erweiterungen > Neuer Parameter MarginFromValueInfluencingFactors für die Funktion setValueInfluencingFactors"
---

# Neuer Parameter MarginFromValueInfluencingFactors für die Funktion setValueInfluencingFactors

Beim Aufruf der Funktion setValueInfluencingFactors des ValuationN-Services kann für freie Aktenzeichen ab sofort optional der neue Parameter MarginFromValueInfluencingFactors übergeben werden.

Mit dem neuen Parameter kann analog zur Webanwendung bestimmt werden, ob die Handelsspanne
aus den wertbeeinflussenden Faktoren oder aus dem prozentualen Wert bzw. Sachverständigenwert
berechnet werden soll.

| Parameter | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| MarginFromValueInfluencingFactors | Boolean | Berechnungsmethode der Handelsspanne. | true = Die Handelsspanne wird immer aus den wertbeeinflussenden Faktoren berechnet. false (default) = Falls im Request mindestens einer der Parameter PercentageOfSalesPrice, InPercentageOfSalesPriceNet und InPercentageOfSalesPriceGross gesetzt sind, wird die Handelsspanne aus prozentualem bzw. Sachverständigenwert berechnet, sonst aus den wertbeeinflussenden Faktoren. |  |

Der neue Parameter MarginFromValueInfluencingFactors wird auch in der Response ausgegeben. Weitere Details zur Funktion setValueInfluencingFactors entnehmen sie bitte dem Kompendium.

Bitte führen Sie entsprechende Anpassungen in Ihren Anwendungen durch, wenn Sie die
neue Funktionalität nutzen möchten.
