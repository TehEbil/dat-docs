---
title: "Informationsermittlung mit Herstellerschlüssel und ETN"
topic_id: "2543"
breadcrumb: "SilverDAT Produkte > SilverDAT PartsInfo > Schnittstellenoperationen > Informationsermittlung mit Herstellerschlüssel und ETN"
---

# Informationsermittlung mit Herstellerschlüssel und ETN

Beschreibung

Die Schnittstellen-Funktion getExtPartNoInfoByMfrAndExtPartNo dient der Ermittlung von Informationen anhand von Hersteller-Schlüssel und externer
Teilekennung. Mit dem Parameter coverage kann die zurückgegebene Datenmenge um die Ausstattungsinformationen eingeschränkt
werden. So kann der Rückgabeumfang reduziert werden.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| mfr | Integer | Hersteller-Schlüssel | w.v. | X |
| extPartNo | String | [Definition ETN und DVN](../definition-etn-2516.md) | Die Teilekennung kann 1 - N mal übergeben werden. | X |
| coverage | String | COMPLETE / BASE / SIMPLE | SIMPLE liefert nur die Schlüssel von Modellinformationen (Fahrzeugart, Hersteller, Haupttyp, Untertyp)  BASE / COMPLETE liefert Schlüssel und Benennungen der Modellinformationen. | X |

Rückgabe

Die Rückgabe erfolgt in VXS-Struktur. Zurückgegeben werden 1:N [Dossier](../../../vxs/aktenzeichenvo-1369.md), mit Informationen aus [Fahrzeug](../../../vxs/aktenzeichenvorgange-doss/fahrzeug-vehic-6692.md), [Ausstattungen zum DAT €uropa-Code, Ausstattungspositionen, Teilepositionen,](../../../vxs/aktenzeichenvorgange-doss/fahrzeug-vehicle/ausstattungen-1381.md)

WSDL

Die WSDL für diese Schnittstellen-Funktion ist aktuell zu finden unter

<https://www.dat.de/PartsInfo/services/SpareParts?wsdl>
