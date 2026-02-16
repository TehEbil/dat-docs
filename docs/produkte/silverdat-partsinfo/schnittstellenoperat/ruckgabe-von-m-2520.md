---
title: "Rückgabe von Modellinfo über HST und ETN"
topic_id: "2520"
breadcrumb: "SilverDAT Produkte > SilverDAT PartsInfo > Schnittstellenoperationen > Rückgabe von Modellinfo über HST und ETN"
---

# Rückgabe von Modellinfo über HST und ETN

Die Funktion getModelInfoByMfrAndExtPartNo liefert die möglichen Modellinformationen (Fahrzeugart, Hersteller, Haupttyp, Untertyp)
zu den gelieferten Eingaben Hersteller + Ersatzteilnummer (ETN).

Mit dem Parameter coverage kann die zurückgegebene Datenmenge um die Ausstattungsinformationen eingeschränkt
werden. So kann der Rückgabeumfang reduziert werden.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| manufacturer | Integer | Hersteller-Schlüssel | w.v. | X |
| extPartNo | String | [Definition ETN und DVN](../definition-etn-2516.md) | Die Teilekennung kann 1 - N mal übergeben werden. | X |
| coverage | String | COMPLETE / BASE / SIMPLE | SIMPLE liefert nur die Schlüssel von Modellinformationen (Fahrzeugart, Hersteller, Haupttyp, Untertyp)  BASE / COMPLETE liefert Schlüssel und Benennungen der Modellinformationen. | X |

Außerdem wird ein Cookie benötigt, dass die SessionID übergibt. Weitere Informationen entnehmen Sie bitte dem Kapitel "[Authentifizierung über die neuen SilverDAT Webservices](../../../allgemein/dat-developers-guide/authentifizierung-de/index.md)".

Rückgabe

Die Rückgabe erfolgt in VXS-Struktur und liefert die möglichen Modellinformationen (Fahrzeugart, Hersteller, Haupttyp,
Untertyp) zu den gelieferten Eingaben Hersteller + Ersatzteilnummer.

WSDL

Die WSDL für diese Schnittstellen-Funktion ist aktuell zu finden unter

<https://www.dat.de/PartsInfo/services/SpareParts?wsdl>
