---
title: "Informationsermittlung mit Untertyp und ETN"
topic_id: "2539"
breadcrumb: "SilverDAT Produkte > SilverDAT PartsInfo > Schnittstellenoperationen > Informationsermittlung mit Untertyp und ETN"
---

# Informationsermittlung mit Untertyp und ETN

Beschreibung

Die Funktion getExtPartNoInfoByModelAndExtPartNo liefert bei Übergabe von Fahrzeugart, Hersteller, Haupttyp - optional auch: Untertyp
- und den Ersatzteilnummern folgende Werte zurück:

- DAT €uropa-Code®
- Ersatzteilnummer mit Preis
- DVN

Mit dem Parameter coverage kann die zurückgegebene Datenmenge um die Ausstattungsinformationen eingeschränkt
werden. So kann der Rückgabeumfang reduziert werden.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| subModel | integer |  | Untertyp |  |
| baseModel | integer |  | Haupttyp | X |
| vehicleType | integer |  | Fahrzeugart | X |
| manufacturer | Integer | Hersteller-Schlüssel | w.v. | X |
| extPartNo | String | [Definition ETN und DVN](definition-etn-2516.md) | Die Teilekennung kann 1 - N mal übergeben werden. | X |
| coverage | String | COMPLETE / BASE / SIMPLE | COMPLETE gibt alle Daten zurück, BASE gibt nur die Basisinformationen wieder; die Ausstattungen zum Fahrzeug werden nicht geliefert. SIMPLE gibt nur die IDs zurück. | X |

Außerdem wird ein Cookie benötigt, dass die SessionID übergibt. Weitere Informationen entnehmen Sie bitte dem Kapitel [Authentifizierung über die neue SilverDAT Webservices](../../allgemein/dat-developers-gui/authentifizier-1294.md).

Rückgabe

Die Rückgabe erfolgt - abhängig von COVERAGE - in VXS-Struktur und liefert DAT €uropa-Code, Ersatzteilnummer mit Preis und DVN.

WSDL

Die WSDL für diese Schnittstellen-Funktion ist aktuell zu finden unter

<https://www.dat.de/PartsInfo/services/SpareParts?wsdl>
