---
title: "Mögliche Fehlercodes deleteDossier"
topic_id: "7785"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Löschen eines Dossiers/Vorgangs > Mögliche Fehlercodes deleteDossier"
---

# Mögliche Fehlercodes deleteDossier

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| dat:validation.dossierId.missing | Vorgangs-ID fehlt. | Der Parameter DossierId wurde nicht angegeben. |
| dat:validation.dossierId.notFound | Vorgang nicht gefunden. | Es existiert kein Vorgang mit der angegebenen Vorgangs-ID. |
| dat:validation.dossierId.locked | Vorgang ist gesperrt. | Der Vorgang ist momentan durch einen anderen Benutzer gesperrt. |
