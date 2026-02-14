---
title: "Mögliche Fehlercodes marketDataFromDossier"
topic_id: "18837"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Börsendaten via webScan REST-API abrufen > Funktionsumfang webScan > Mögliche Fehlercodes marketDataFromDossier"
---

# Mögliche Fehlercodes marketDataFromDossier

###### Mögliche Fehlercodes marketDataFromDossier | Rückgabecode | Fehlertext | Beschreibung | | --- | --- | --- | | dat:validation.ContractID.missing | Parameter ContractID fehlt | Der Parameter DossierId wurde nicht angegeben. | | dat:Server.WrongPermissions | Angeforderter Datensatz konnte nicht gefunden werden. Er wurde entweder gelöscht oder Sie haben keine Berechtigung den Datensatz einzusehen. | Es existiert kein Vorgang mit der angegebenen Vorgangs-ID oder Sie haben keine Berechtigung den Datensatz einzusehen. | | dat:validation.dossierId.locked | Vorgang ist gesperrt. | Der Vorgang ist momentan durch einen anderen Benutzer gesperrt. | | dat:validation.isDisengaged.notAllowed | Börsenübersicht ist für freie Aktenzeichen nicht verfügbar. | Die webScan-Funktionalität kann nicht für freie Aktenzeichen verwendet werden. | | dat:valuation.WrongProcedureType | Börsendaten sind nicht verfügbar für Neufahrzeuge, Vorführfahrzeuge und Tageszulassungen. | Die webScan-Funktionalität kann nicht für die Vorgangsarten NEW\_VEHICLE, PRE\_REGISTRATION und DEMONSTRATION verwendet werden. | | dat:validation.webscan2.notLicensed | Für diese Funktion liegt keine Lizenzierung vor. | Die webScan Funktionalität ist für die Kundennummer nicht lizenziert. |
