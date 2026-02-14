---
title: "Mögliche Fehlercodes getVehicleApproximateValue"
topic_id: "2179"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Annäherungsbewertung > Mögliche Fehlercodes getVehicleApproximateValue"
---

# Mögliche Fehlercodes getVehicleApproximateValue

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| dat:validation.initialRegistration.missing | Erstzulassungsdatum fehlt. | Die Erstzulassung ist falsch oder fehlt. Bitte überprüfen Sie den Erstzlassungstermin. |
| dat:validation.initialRegistration.afterDataMonth | Erstzulassungsdatum liegt nach Datenmonat/-jahr. | Die Erstzulassung liegt in der Zukunft. Bitte korrigieren Sie die Erstzulasung. |
| dat:validation.approximationSign.invalid | Das Bewertungskennzeichen ist ungültig. Mögliche Werte sind 'MINIMUM', 'APPROXIMATION', 'MAXIMUM' | Das Bewertungskennzeichen ist ungültig. Bitte verwenden Sie nur einen der erlaubten Werte. |
| dat:validation.approximationSign.missing | Das Bewertungskennzeichen fehlt. Mögliche Werte sind ‘MINIMUM‘, ‘APPROXIMATION‘, ‘MAXIMUM‘. | Das Bewertungskennzeichen fehlt. Bitte geben Sie das Bewertungskennzeichen an. |
| dat:validation.exFactoryPrice.missing | Bei Angabe des Bewertungskennzeichens ‚APPROXIMATION‘ muss der Parameter exFactoryPrice angegeben werden. | Der Parameter exFactoryPrice wurde nicht angegeben, ist aber bei Angabe des Bewertungskennzeichens APPROXIMATION Pflicht. Bitte geben Sie den Parameter exFactoryPrice. |
| dat:validation.VIN.invalid | Die angegebene VIN (17-stellig) ist ungültig. | Die VIN muss 17-stellig sein. Bitte korrigieren Sie die VIN. |
| dat:validation.VIN\_manufacturer.notSupported | Für den angegebenen Hersteller können keine VIN-Abfragen durchgeführt werden. | Für den angegebenen Hersteller können keine VIN-Abfragen durchgeführt werden. |
| dat:validation.registrationDate\_KBA.outOfRange | Die Erstzulassung ist außerhalb des gültigen Bereichs. | Die Erstzulassung oder die Bauzeit ist außerhalb des gültigen Bereichs für das angegebene Fahrzeug.Bitte korrigieren Sie die Erstzulassung beziehungsweise die Bauzeit. |
| dat:validation.registrationDate\_VIN.outOfRange | Die Erstzulassung ist außerhalb des gültigen Bereichs. | Die Erstzulassung oder die Bauzeit ist außerhalb des gültigen Bereichs für das angegebene Fahrzeug.Bitte korrigieren Sie die Erstzulassung beziehungsweise die Bauzeit. |
| dat:Server.valueNotFound | Vehicle not found. No evaluation possible.: ; VIN: no vehicle to evaluate found | Für die angegebene VIN fehlt der zugehörige DAT €uropa-Code®. Bitte informieren Sie [interfaces@dat.eu](mailto:interfaces@dat.eu "Mail DAT interfaces"). |
| dat:validation.ecode\_Model.notFound | Es wurde kein passender DATECode gefunden. | Für den Modellcode wurde kein passender DAT €uropa-Code® gefunden. |
| dat:validation.registrationDate\_DATECODE.outOfRange | Die Erstzulassung ist außerhalb des gültigen Bereichs. | Die Erstzulassung oder die Bauzeit ist außerhalb des gültigen Bereichs für das angegebene Fahrzeug.Bitte korrigieren Sie die Erstzulassung beziehungsweise die Bauzeit. |
| dat:Server.ManufacturerNotLicensed | Manufacturer not licensed. | Sie sind nicht berechtigt den angegebenen Hersteller abzufragen. Bitte wenden Sie sich an den DAT Vertrieb: sales-support@dat.de. |
| dat:validation.LicenseNumber.length | Die maximale Zeichenlänge für Kennzeichen für das Datenland <Datenland> beträgt <Zahl> Zeichen. | Die maximale Zeichenlänge für das Kennzeichen LicenseNumber für das gewählte Datenland wurde überschritten. Bitte passen Sie den Parameter LicenseNumber an. |
| dat:validation.identificationOrder.invalid | Die angegebene Reihenfolge der Identifizierung ist ungültig, zulässige Werte sind 'DATECODE', 'KBA', 'VIN', 'MODEL', 'NATIONALCODE' | Der Parameter identificationOrder enthält einen ungültigen Wert. Gültige Werte sind 'DATECODE', 'KBA', 'VIN', 'MODEL', 'NATIONALCODE'. Bitte korrigieren Sie den Parameter identificationOrder. |
| dat:validation.manualEquipmentExFactoryPrice.missing | Der Ausstattungsgesamtpreis fehlt. | Der Node manualEquipmentDevaluations wurde angegeben, aber der Parameter manualEquipmentExFactoryPrice fehlt. Bitte übergeben Sie den Parameter manualEquipmentExFactoryPrice im Request. |
| dat:validation.manualEquipmentDevaluation\_percent.missing | Die Prozentangabe für das manuelle Ausstattungsabwertungspaket fehlt. | Der Parameter percent und manualEquipmentDevaluation fehlt. Bitte übergeben Sie den Parameter percent im Request. |
| dat:validation.manualEquipmentDevaluation\_percent.invalid | Die Summe der Prozentangaben für die Ausstattungsabwertungspakete ist größer als 100. | Die Summe der Prozentangaben unter manualEquipmentDevaluation ist größer als 100. BItte korrigieren Sie die Prozentangaben im Request. |
| dat:validation.nationalCode.notAllowed | Der Parameter nationalCode ist nur für Österreich erlaubt. | Der Parameter nationalCode kann nur für das Datenland Österreich angegeben werden. |
| dat:validation.kba.notAllowed | Der Parameter kba ist nur für Deutschland erlaubt. | Der Parameter kba kann nur für das Datenland Deutschland angegeben werden. |
| dat:validation.mileage.invalid | Laufleistung ist ungültig. | Der Parameter mileage liegt außerhalb des gültigen Bereichs. |
