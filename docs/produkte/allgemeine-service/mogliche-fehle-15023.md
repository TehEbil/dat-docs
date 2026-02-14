---
title: "Mögliche Fehlercodes updateDossierN"
topic_id: "15023"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Aktualisieren eines Vorgangs ohne Wertänderung > Mögliche Fehlercodes updateDossierN"
---

# Mögliche Fehlercodes updateDossierN

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| dat:validation.dossierId.missing | Vorgangs-ID fehlt. | Der Parameter DossierId wurde nicht angegeben. |
| dat:validation.dossierId.notFound | Vorgang nicht gefunden. | Es existiert kein Vorgang mit der angegebenen Vorgangs-ID. |
| dat:validation.dossierId.locked | Vorgang ist gesperrt. | Der Vorgang ist momentan durch einen anderen Benutzer gesperrt. |
| dat:Server.ManufacturerNotLicensed | manufacturer not licensed | Sie sind nicht berechtigt den angegebenen Hersteller abzufragen. Bitte wenden Sie sich an den DAT Vertrieb: sales-support@dat.de. |
| dat:validation.WrongUsage | Aktion ist bei unvollständigen Aktenzeichen nicht erlaubt. | Der Aufruf von updateDossierN ist nicht erlaubt für unvollständige Aktenzeichen. |
| dat:validation.noPermission | Der Benuzer besitzt keine Rechte, um auf diesen Vorgang zuzugreifen. | Der verwendete Benutzer hat keine Berechtigung den Vorgang aufzurufen. |
