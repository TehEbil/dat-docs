---
title: "Übergabe von strukturierten Rechnungs- oder Kalkulationsdaten"
topic_id: "7500"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Übergabe von strukturierten Rechnungs- oder Kalkulationsdaten"
---

# Übergabe von strukturierten Rechnungs- oder Kalkulationsdaten

Diese Funktion ermöglicht es Rechnungs-, bzw. Kalkulationsergebnisse von Drittanbieter-Systemen
nach myclaim zu übertragen. Diese Daten liegen dann nach dem Import als eine Art "Pseudo Kalkulation"
in myclaim vor und können z.B. dazu genutzt werden um z.B. Kalkulationsvergleiche durchzuführen.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| contractId | Long |  | ID des Auftrags | X |
| summaryType |  | EXTERNAL, MANUAL, INVOICE, PAYMENT | EXTERNAL = Kalkulation aus Drittanbieter-System    MANUAL = Manuell eingegebene Berechnungswerte (Summen    INVOICE = Teilberechnung dient als ausgegebene Rechnung    PAYMENT = Berechnung enthält nur Informationen über die erhaltene Zahlung |  |
| calculationSummary | CalculationSummaryType |  | Ist ein Kalkulationssummen Element des DAT VXS Formats |  |
| invoiceAttributes | InvoiceAttributes |  | Element das die Rechnungsnummer und das Rechnengsdatum beinhaltet |  |

Rückgabe

Kalkulations ID falls erfolgreich
