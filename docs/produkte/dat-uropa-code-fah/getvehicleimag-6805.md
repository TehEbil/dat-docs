---
title: "getVehicleImagesN"
topic_id: "6805"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugbilder Funktionen > getVehicleImagesN"
---

# getVehicleImagesN

Beschreibung

Die Funktion getVehicleImagesN liefert die Fahrzeugbilder zu einem DAT €uropa-Code®.

Die von der Schnittstellenfunktion gelieferten Bilddaten unterliegen dem Urheberrecht
und dürfen nur innerhalb der DAT-Kundenanwendungen angezeigt werden.  
Für weiterführende Verwendungen können gesonderte Verträge abgeschlossen werden. Bei
Interesse kontaktieren Sie bitte unseren Vertrieb: [sales-support@dat.de](mailto:sales-support@dat.de "Mail an DAT sales-support")

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| datECode | String | DAT €uropa-Code® | Gültiger DAT €uropa-Code® (11 oder 15 Stellen) | X |
| aspect | Enumeration | ALL, FRONTVIEW, ANGULARFRONT, SIDEVIEW, REARVIEW, DASHBOARD, ANGULARREAR, TRUNK | Einschränkung der Bilder: ALL bedeutet "alle Bilder", FRONT bedeutet "Vorderseite", ... | X |
| imageType | Enumeration | PICTURE | Einschränkung der Bilder: PICTURE bedeutet "Foto" | X |

Rückgabe

Liste aller Fahrzeugbilder; jedes Fahrzeugbild besteht aus den Rückgabefeldern:

aspect (Datentyp Enumeration, mögliche Werte: FRONTVIEW, ANGULARFRONT, SIDEVIEW, REARVIEW, DASHBOARD, ANGULARREAR, TRUNK): Aspekt des Bildes

imageType (Datentyp Enumeration, möglicher Wert: PICTURE): Art des Bildes

imageBase64: Binärdaten des Bildes im Base64-Format kodiert. Dieses ist nötig um den
problemlosen Transport der Binärdaten zu gewährleisten.

imageFormat (Datentyp Enumeration, mögliche Werte: JPG, PNG, GIF): Format der Binärdaten
des Bildes.

WSDL

https://<HOST>/<PRODUKT>/<PROTOKOLL>/<SERVICE>?wsdl

Serviceaufruf

https://<HOST>/<PRODUKT>/<PROTOKOLL>/<SERVICE>

Die Schnittstellenfunktionen der DAT €uropa-Code® Fahrzeugauswahl sind sowohl im gleichnamigen Produkt, als auch in allen anderen Produkten
enthalten.

Produkte

| Name | ProductVariant | <HOST> | <PRODUKT> | <PROTOKOLL> | <SERVICE> |
| --- | --- | --- | --- | --- | --- |
| DAT €uropa-Code Fahrzeugauswahl |  | www.datgroup.com | DATECodeSelection | services | VehicleImagery |
| SilverDAT calculatePro |  | www.datgroup.com | VehicleRepairOnline | services | VehicleImagery |
| SilverDAT calculateExpert | calculateExpert | www.datgroup.com | VehicleRepairOnline | services | VehicleImagery |
| SilverDAT valuateFinance |  | www.datgroup.com | FinanceLine | soap | VehicleImagery |
| SilverDAT valuateExpert | valuateNG.expert | www.datgroup.com | valuateNG | soap | VehicleImagery |
| SilverDAT 3 Pro | DAT | www.datgroup.com | myClaim | soap/v2 | VehicleImagery |
| SilverDAT 3 myclaim | abhängig vom jeweiligen Netz | www.datgroup.com | myClaim | soap/v2 | VehicleImagery |
