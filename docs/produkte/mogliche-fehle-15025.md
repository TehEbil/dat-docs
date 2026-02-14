---
title: "Mögliche Fehlercodes searchDossierListN"
topic_id: "15025"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Suchen von Vorgängen > Mögliche Fehlercodes searchDossierListN"
---

# Mögliche Fehlercodes searchDossierListN

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| dat:validation.searchCriteria.missing | Search criterion element missing. | Der Request beinhaltet kein SearchCriterion  Element |
| dat:validation.searchKey.invalid | common.error.validation.searchKey.invalid | Bitte vergeben Sie einen Suchschlüssel. |
| dat:validation.searchKey.invalid | Search field / code invalid: your key value | Der zugewiesene Suchschlüssel wird nicht unterstützt. |
| dat:validation.dossierType.invalid | Dossier type invalid. | Der Parameter DossierType enthält einen ungültigen Wert. |
| dat:validation.resultLimit.outOfRange | Result limit outside the valid range [1 - 1000]. | Der Parameter LIMIT liegt außerhalb des gültigen Bereichs (derzeit 1 bis 1000). |
| dat:Server.invalidNamespace | invalid namespace declaration | Ein zugewiesener Datumswert besitzt ein ungültiges Format. Bitte korrigieren Sie diesen Datumswert. |
| dat:Server.ManufacturerNotLicensed | manufacturer not licensed | Sie sind nicht berechtigt den angegebenen Hersteller abzufragen. Bitte wenden Sie sich an den DAT Vertrieb: sales-support@dat.de. |
| de.dat.sphinx.global.exception.ValidationException | common.error.validation.resultOffset.outOfRange | Der Parameter Offset liegt außerhalb des gültigen Bereichs (derzeit 1-1000). |
| dat:validation.wildcard.invalid | Für den angegebenen Suchbegriff ist die Suche mittels Wildcard nicht möglich. | Für den angegebenen Suchbegriff ist die Suche mittels Wildcard nicht möglich. |
