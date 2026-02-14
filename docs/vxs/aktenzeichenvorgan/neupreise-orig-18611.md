---
title: "Neupreise (OriginalPriceInfo)"
topic_id: "18611"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Fahrzeug (Vehicle) > Neupreise (OriginalPriceInfo)"
---

# Neupreise (OriginalPriceInfo)

<OriginalPriceInfo> ist ein Unter-Element von <Vehicle> und enthält Informationen den Neupreisen.

Nur für die VIN-Abfrage im Anwendungsfall Fahrzeugbewertung (restriction=APPRAISAL)

Felder:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| OriginalPriceNet | decimal | Neupreis Netto (ohne Sonderausstattungen) |
| OriginalPriceGross | decimal | Neupreis Brutto (ohne Sonderausstattungen) |
| OriginalPriceVATRate | decimal | Mehrwertsteuersatz |
| OriginalPriceNoVA | decimal | VERALTET! Normverbrauchsabgabe (nur für Österreich) |
| (Dat)OriginalPriceNoVARate | decimal | Prozentsatz der Normverbrauchsabgabe (nur für Österreich) |
| OriginalPriceBonus | decimal | NoVA Bonus (nur für Österreich) |
| OriginalPriceMalus | decimal | NoVA Malus (nur für Österreich) |
| RegistrationTaxRate | decimal | Zulassungssteuersatz (für Spanien) |
| TransportationCosts | decimal | Transportkosten (für Spanien) |
| RegistrationTax | decimal | Wert der Zulassungssteuer (für Italien) |
