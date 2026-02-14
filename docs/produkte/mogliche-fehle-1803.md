---
title: "Mögliche Fehlercodes getVehicleIdentificationByVin"
topic_id: "1803"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Fahrzeugidentifikation anhand VIN (VIN-Abfrage) > Mögliche Fehlercodes getVehicleIdentificationByVin"
---

# Mögliche Fehlercodes getVehicleIdentificationByVin

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| requireCode | %value% is required! | Pflichtfeld fehlt. |
| wrongValueCode | Wrong Ecode | Bitte überprüfen Sie den DAT €uropa-Code® |
| valueNotFound | Container not found for this construction time. | Bauzeit und Marktindex passen nicht zusammen. |
| valueNotFound | Ecode not found. | Mit diesen Werten kann kein gültiger DAT €uropa-Code® gefunden werden. Im Fall, dass die Herstellerdaten zur Verfügung stehen, werden sie als String in Form einer [Datenkarte](#showid/11682 "ECode not found  - Datenkarte") zurückgegeben. |
| internalError | Given Restriction sign is wrong, allowed values are: 'ALL', 'REPAIR', 'APPRAISAL' | Der Wert für die Filteroption ist falsch. Bitte verwenden Sie nur einen der erlaubten Werte. |
| internalError | Typemismatch for property "coverage". | Der Wert für die Abdeckung ist falsch. Bitte verwenden Sie nur einen der erlaubten Werte. |
| CountryError | locale is missing | Das Element locale ist Pflichtfeld, aber fehlt im request. |
| CountryError | wrong language value | Der Wert für die Spracheinstellung ist falsch. Bitte verwenden Sie nur die zulässigen Werte (ISO 639-1). |
| CountryError | wrong country value | Der Wert für die Landeseinstellung ist falsch. Bitte verwenden Sie nur die zulässigen Werte (ISO 3166 ALPHA-2). |
| LocaleError | wrong country indicator value | Der Wert für den Zielmarkt ist falsch. Bitte verwenden Sie nur die zulässigen Werte (ISO 3166 ALPHA-2). |

Weitere Fehlercodes entnehmen sie bitte aus der Liste der [Test-VIN für Fehlermeldungen](#showid/1796 "Test-VIN für Fehlermeldungen (Abruf kostenfrei)").
