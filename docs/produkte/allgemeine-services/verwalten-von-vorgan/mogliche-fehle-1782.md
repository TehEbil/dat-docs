---
title: "Mögliche Fehlercodes exportDossierN"
topic_id: "1782"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Exportieren von Dokumenten (SilverDAT 3 valuateFinance) > Mögliche Fehlercodes exportDossierN"
---

# Mögliche Fehlercodes exportDossierN

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| dat:validation.exportProduct.invalid | Vorgaben für Export-Produkt nicht zulässig. | Der Parameter ExportProduct fehlt oder enthält ungültige Attribute. |
| dat:validation.format.invalid | Export-Format ungültig. | Der Parameter Format fehlt oder enthält einen ungültigen Wert. |
| dat:validation.dossierId.missing | Vorgangs-ID fehlt. | Der Parameter DossierId wurde nicht angegeben. |
| dat:validation.dossierId.notFound | Vorgang nicht gefunden. | Es existiert kein Vorgang mit der angegebenen Vorgangs-ID. |
| dat:validation.evaluation.outOfDate | Bewertung nicht aktuell. | Für den gewählten Vorgang wurde keine aktuelle Bewertung durchgeführt, d.h. die Bewertungsdaten sind veraltet. |
| dat:validation.indicationOfValue.invalid | Ungültige Wertangabe: [X]. Mögliche Werte sind: [net | gross]. | Die Wertangabe indicationOfValue ist nicht net oder gross. Bitte überprüfen Sie die Wertangabe. |
| dat:validation.priceType.invalid | Ungültige Preisangabe. Mögliche Werte sind: [purchase | sales | purchaseAndSales]. | Die Preisangabe priceType ist nicht purchase, sales oder purchaseAndSales. Bitte überprüfen Sie die Wertangabe. |
| dat:Server.internalError | Couldn't create PDF data for null | Die PDF konnte nicht erstellt werden. Bitte überprüfen Sie die gewählten Vorgaben. |
| dat:validation.forecast.noData | Keine Restwertprognosen vorhanden. | In der Methode createDossierN müssen im Body ForeCast die Unterelemte gesetzt werden. |
| dat:validation.ForeCast.missing | Die Restwertprognose fehlt. Bitte fügen Sie eine Restwertprognose hinzu. | In der Methode createDossierN müssen im Body ForeCast die Unterelemte gesetzt werden. |
| dat:validation.ForeCast.OnlyForUsedCar | Dieser Ausdruck kann nur für Gebrauchtfahrzeuge verwendet werden. | Der gewählte Ausdruck ist nur für Gebrauchtfahrzeuge verfügbar. |
| dat:validation.ForeCast.OnlyForNewCar | Dieser Ausdruck kann nur für Neufahrzeuge verwendet werden. | Der gewählte Ausdruck ist nur für Neufahrzeuge verfügbar. |
