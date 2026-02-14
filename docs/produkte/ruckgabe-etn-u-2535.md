---
title: "Rückgabe ETN über VIN und DVN"
topic_id: "2535"
breadcrumb: "SilverDAT Produkte > SilverDAT PartsInfo > Schnittstellenoperationen > Rückgabe ETN über VIN und DVN"
---

# Rückgabe ETN über VIN und DVN

Beschreibung

Die Schnittstellen-Funktion getExtPartNoInfoByVinAndIntPartNo dient der Ermittlung von Teileinformationen anhand von Vehicle Identification Number
(VIN) und DVN. Mit dem Parameter coverage kann die zurückgegebene Datenmenge um die Ausstattungsinformationen eingeschränkt
werden. So kann der Rückgabeumfang reduziert werden.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| vin | String | Vehicle Identification Number | 17stellige Fahrzeug-Nr. | X |
| intPartNo | Integer | [Definition ETN und DVN](#showid/2516 "Definition ETN und DVN") | Die Teilekennung kann 1 - N mal übergeben werden. | X |
| coverage | String | COMPLETE / BASE / SIMPLE | SIMPLE liefert nur die Schlüssel von Modellinformationen (Fahrzeugart, Hersteller, Haupttyp, Untertyp)  BASE / COMPLETE liefert Schlüssel und Benennungen der Modellinformationen. | X |

Rückgabe

Die Rückgabe erfolgt in VXS-Struktur. Zurückgegeben werden 1:N [Dossier](#showid/1369 "Aktenzeichen/Vorgänge (Dossiers)"), mit Informationen aus [Fahrzeug](#showid/6692 "Fahrzeug (Vehicle)"), Ausstattungen zur VIN, Ausstattungen zum DAT €uropa-Code, [Ausstattungspositionen, Teilepositionen,](#showid/1381 "Ausstattungen (Equipment, …Equipment, EquipmentPosition)")

WSDL

Die WSDL für diese Schnittstellen-Funktion ist aktuell zu finden unter

<https://www.dat.de/PartsInfo/services/SpareParts?wsdl>
