---
title: "Mögliche Fehlercodes exportDossierN"
topic_id: "25354"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Exportieren von Dokumenten (SilverDAT 3 valuateExpert, valuateExpertPlusPartner) > Mögliche Fehlercodes exportDossierN"
---

# Mögliche Fehlercodes exportDossierN

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| dat:validation.exportProduct.invalid | Export-Produkt ungültig. | Der Parameter ExportProduct fehlt oder enthält ungültige Attribute. |
| dat:validation.format.invalid | Export-Format ungültig. | Der Parameter Format fehlt oder enthält einen ungültigen Wert. |
| dat:validation.dossierId.missing | Vorgangs-ID fehlt. | Der Parameter DossierId wurde nicht angegeben. |
| dat:validation.dossierId.notFound | Vorgang nicht gefunden. | Es existiert kein Vorgang mit der angegebenen Vorgangs-ID. |
| dat:validation.evaluation.outOfDate | Bewertung nicht aktuell. | Für den gewählten Vorgang wurde keine aktuelle Bewertung durchgeführt, d.h. die Bewertungsdaten sind veraltet. |
| dat:validation.indicationOfValue.invalid | Ungültige Wertangabe: [X]. Mögliche Werte sind: [net | gross]. | Die Wertangabe indicationOfValue ist nicht net oder gross. Bitte überprüfen Sie die Wertangabe. |
| dat:validation.priceType.invalid | Ungültige Preisangabe: [X]. Mögliche Werte sind: [purchase | sales | purchaseAndSales]. | Die Preisangabe priceType ist nicht purchase, sales oder purchaseAndSales. Bitte überprüfen Sie die Wertangabe. |
| dat:validation.Tax.invalid | Ungültige Steuer | Für die Besteuerung tax wurde ein ungültiger Wert angegeben. |
| dat:validation.Taxation.mismatch | Besteuerungstyp enthält keinen gültigen Wert | Für die Besteuerung tax wurde ein ungültiger Wert angegeben. |
| dat:validation.Layout.invalid | Ungültiges Layout | Der Wert für das Attribut layout ist ungültig. |
| dat:validation.ValueIndication.invalid | Wertangabe enthält keinen gültigen Wert | Der Wert für das Attribut valueIndication ist ungültig. |
| dat:validation.Value.invalid | Ungültiger Wert | Der Wert für das Attribut value ist ungültig. |
| dat:validation.PrintOptin.invalid | Ungültige Druckoption | Der Wert für das Attribut printOption ist ungültig. |
| dat:Server.internalError | Couldn't create PDF data for null | Die PDF konnte nicht erstellt werden. Bitte überprüfen Sie die gewählten Vorgaben. |
| dat:ExportProductAddOns.product.ValuationExpertiseNew.invalid | exportDossierN.validation.ExportProductAddOns.product.ValuationExpertiseNew.invalid | Wird productName=ValuationExpertiseNew angegeben, muss unter ExportProductAddOns für product der Wert VALUATION\_EXPERTISE angegeben werden. |
| dat:ExportProductAddOns.product.ValuationExpertise.invalid | Im Parameter ExportProductAddOns im product ist nur VALUATION\_EXPERTISE erlaubt, wenn Sie eine ValuationExpertise drucken möchten. | Wird productName=ValuationExpertise angegeben, muss unter ExportProductAddOns für product der Wert VALUATION\_EXPERTISE angegeben werden. |
| dat:ExportProductAddOns.product.EstimationCertificateNew.invalid | exportDossierN.validation.ExportProductAddOns.product. EstimationCertificateNew.invalid | Wird productName=EstimationCertificateNew angegeben, muss unter ExportProductAddOns für product der Wert ESTIMATION\_CERTIFICATE angegeben werden. |
| dat:ExportProductAddOns.product.EstimationCertificate.invalid | Im Parameter ExportProductAddOns im product ist nur ESTIMATION\_CERTIFICATE erlaubt, wenn Sie ein EstimationCertificate drücken möchten. | Wird productName=EstimationCertificate angegeben, muss unter ExportProductAddOns für product der Wert ESTIMATION\_CERTIFICATE angegeben werden. |
| dat:ExportProductAddOns.product.BaseCheckReportNew.invalid | exportDossierN.validation.ExportProductAddOns.product. BaseCheckReportNew.invalid | Wird productName=BaseCheckReportNew angegeben, muss unter ExportProductAddOns für product der Wert BASECHECK angegeben werden. |
| dat:ExportProductAddOns.product.BaseCheckReport.invalid | Im Parameter ExportProductAddOns im Attribut product ist nur BASECHECK erlaubt, wenn Sie einen BaseCheckReport drucken möchten. | Wird productName=BaseCheckReport angegeben, muss unter ExportProductAddOns für product der Wert BASECHECK angegeben werden. |
| dat:ExportProductAddOns.product.LeasingReturnReportNew.invalid | exportDossierN.validation.ExportProductAddOns.product. LeasingReturnReportNew.invalid | Wird productName=LeasingReturnReportNew angegeben, muss unter ExportProductAddOns für product der Wert LEASING\_RETURN angegeben werden. |
| dat:ExportProductAddOns.product.LeasingReturnReport.invalid | Im Parameter ExportProductAddOns im product ist nur LEASING\_RETURN erlaubt, wenn Sie einen LeasingReturnReport drucken möchten. | Wird productName=LeasingReturnReport angegeben, muss unter ExportProductAddOns für product der Wert LEASING\_RETURN angegeben werden. |
| dat:validation.withConditionComments.invalid | Das Attribut withConditionComments enthält keinen gültigen Wert. | Im Parameter withConditionComments können nur die Werte 1 (true) oder 0 (false) übergeben werden. |
