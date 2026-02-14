---
title: "Rückgabe von ETN über DAT europa-Code Ausstattung und DVN"
topic_id: "2513"
breadcrumb: "SilverDAT Produkte > SilverDAT PartsInfo > Schnittstellenoperationen > Rückgabe von ETN über DAT europa-Code Ausstattung und DVN"
---

# Rückgabe von ETN über DAT europa-Code Ausstattung und DVN

Die Schnittstellen-Operation getExtPartNoInfoByFullVehicleAndIntPartNo dient der Ermittlung von Informationen anhand von DAT €uropa-Code, Bauzeit und gegebenenfalls bekannten Ausstattungen sowie der Ersatzteil-Kennung (DVN).

Mit dem Parameter coverage kann die zurückgegebene Datenmenge um die Ausstattungsinformationen eingeschränkt
werden. So kann der Rückgabeumfang reduziert werden.

Bauzeit und Ausstattungen könnten beispielsweise im Vorfeld über eine VIN-Abfrage ermittelt worden sein.

Die Operation nimmt bei der Ermittlung der in Frage kommenden Ersatzteile neben DAT €uropa-Code und Ersatzteil-Kennung (DVN) eine genauere Einschränkung über die Ausstattung vor und kann somit ein eindeutiges
Ergebnis liefern.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| datEcode | String | gültiger DAT €uropa-Code | w.v. | X |
| intPartNo | Integer | [Definition ETN und DVN](#showid/2516 "Definition ETN und DVN"), 5 Stellen | Die Teilekennung kann 1 - N mal übergeben werden. | X |
| coverage | String | COMPLETE / BASE / SIMPLE | COMPLETE gibt alle Daten zurück, BASE gibt nur die Basisinformationen wieder; die Ausstattungen zum Fahrzeug werden nicht geliefert. SIMPLE gibt nur die IDs zurück. | X |
| locale | Custom | de und it | Derzeit sind alle Sprachkombinationen für die Länder DE und IT zulässig. | X |
| sessionID | String |  | kann leer bleiben, da schon im Header übergeben | X |
| constructionTime | Integer | gültige DAT-Bauzeit, 4 Stellen |  | X |
| equipment | Long | gültige DAT-AV-Nummer, bis zu 5 Stellen | 0 - N bekannte, gültige AV-Codes für verbaute Ausstattungen |  |

Rückgabe

Die Rückgabe erfolgt in VXS-Struktur. Zurückgegeben werden 1:N [Dossier](#showid/1369 "Aktenzeichen/Vorgänge (Dossiers)"), mit Informationen aus [Fahrzeug](#showid/6692 "Fahrzeug (Vehicle)"), [Ausstattungen zum DAT €uropa-Code, Ausstattungspositionen, Teilepositionen](#showid/1381 "Ausstattungen (Equipment, …Equipment, EquipmentPosition)").

WSDL

Die WSDL für diese Schnittstellen-Funktion ist aktuell zu finden unter

<https://www.dat.de/PartsInfo/services/SpareParts?wsdl>
