---
title: "Mögliche Fehlercodes resetDossierTechDataN"
topic_id: "25812"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Zurücksetzen von technischen Daten eines Vorgangs auf die DAT-Vorgaben > Mögliche Fehlercodes resetDossierTechDataN"
---

# Mögliche Fehlercodes resetDossierTechDataN

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| dat:validation.dossierId.missing | Vorgangs-ID fehlt. | Der Parameter DossierId wurde nicht angegeben. |
| dat:validation.dossierId.notFound | Vorgang nicht gefunden. | Es existiert kein Vorgang mit der angegebenen Vorgangs-ID. |
| dat:validation.dossierId.locked | Vorgang ist gesperrt. | Der Vorgang ist momentan durch einen anderen Benutzer gesperrt. |
| dat:Server.ManufacturerNotLicensed | manufacturer not licensed | Sie sind nicht berechtigt den angegebenen Hersteller abzufragen. Bitte wenden Sie sich an den DAT Vertrieb: sales-support@dat.de. |
| dat:validation.WrongUsage | Aktion ist bei unvollständigen Aktenzeichen nicht erlaubt. | Der Aufruf von resetDossierTechDataN ist nicht erlaubt für unvollständige Aktenzeichen. |
| dat:validation.noPermission | Der Benuzer besitzt keine Rechte, um auf diesen Vorgang zuzugreifen. | Der verwendete Benutzer hat keine Berechtigung den Vorgang aufzurufen. |
