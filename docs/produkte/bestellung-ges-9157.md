---
title: "Bestellung gesperrter Fahrzeuge"
topic_id: "9157"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Bestellung gesperrter Fahrzeuge"
---

# Bestellung gesperrter Fahrzeuge

Beschreibung

Die Operation orderMarkedVin ermöglicht Kfz-Sachverständigen und Versicherungen die online Bestellung von VIN-Daten
zu einem gesperrten Fahrzeug. Ein Fahrzeug ist als gesperrt gemeldet, wenn der Aufruf
von getVehicleIdentificationByVIN scheitert und dabei als FaultCode error.vinserver.accessible.vin.vw liefert.

Derzeit mögliche Hersteller/Fabrikate sind Audi, Seat, Skoda und Volkswagen.

Die DAT berechnet dem Besteller € 59,00 zzgl. MwSt. pro gelieferten Fahrzeugdatensatz.

Der Einsatz der Fahrzeugdaten ist ausschließlich zur Bestimmung des Bauzustandes eines
Fahrzeugs im Rahmen der Nutzung der vorhandenen SilverDAT-Module (Reparaturkostenkalkulation,
Gebrauchtfahrzeugbewertung usw.) oder anderen damit direkt zusammenhängenden Geschäftsprozessen
zulässig. Eine darüber hinausgehende Nutzung ist dem Besteller nicht gestattet.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| claimNumber | String | String, max. 50 Stellen | Versicherungsnummer |  |
| contact | String | String, max. 101 Stellen | Name einer Kontaktperson | X |
| email | String | String, max 100 Stellen | E-Mail-Adresse | X |
| telephone | String | String, max 40 Stellen | Telefonnummer | X |
| vin | String | String mit 17 Stellen | Fahrgestellnummer | X |

Rückgabe

Nach einem erfolgreichen Aufruf der Bestellung gesperrter Fahrzeuge wird true zurückgegeben.

WSDL

https://<HOST>/<PRODUKT>/<PROTOKOLL>/<SERVICE>?wsdl

Serviceaufruf

https://<HOST>/<PRODUKT>/<PROTOKOLL>/<SERVICE>

Die Schnittstellenfunktionen der DAT €uropa-Code® Fahrzeugauswahl sind sowohl im gleichnamigen Produkt, als auch in allen anderen Produkten
enthalten.

Produkte

| Name | ProductVariant | <HOST> | <PRODUKT> | <PROTOKOLL> | <SERVICE> |
| --- | --- | --- | --- | --- | --- |
| DAT €uropa-Code Fahrzeugauswahl |  | www.datgroup.com | DATECodeSelection | services | VehicleIdentificationService |
| SilverDAT calculatePro |  | www.datgroup.com | VehicleRepairOnline | services | VehicleIdentificationService |
| SilverDAT calculateExpert | calculateExpert | www.datgroup.com | VehicleRepairOnline | services | VehicleIdentificationService |
| SilverDAT valuateFinance |  | www.datgroup.com | FinanceLine | soap | VehicleIdentificationService |
| SilverDAT valuateExpert | valuateNG.expert | www.datgroup.com | valuateNG | soap | VehicleIdentificationService |
| SilverDAT 3 Pro | DAT | www.datgroup.com | myClaim | soap/v2 | VehicleIdentificationService |
| SilverDAT 3 myclaim | abhängig vom jeweiligen Netz | www.datgroup.com | myClaim | soap/v2 | VehicleIdentificationService |
