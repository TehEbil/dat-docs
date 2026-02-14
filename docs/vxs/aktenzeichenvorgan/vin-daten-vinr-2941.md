---
title: "VIN-Daten (VinResult)"
topic_id: "2941"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Fahrzeug (Vehicle) > VIN-Daten (VinResult)"
---

# VIN-Daten (VinResult)

<VinResult > ist ein Unter-Element von <Vehicle> und enthält die Ergebnisse der VIN-Abfrage.

Felder:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| VinInterfaceVersion | string | Versionsnummer der VIN-Abfrage Schnittstelle |
| CrossBorder | fieldBoolean | falls Fahrzeug grenzüberschreitend identifiziert |
| VinDatProcedure | boolean | VIN Abfrage durchgeführt mit DAT VIN-Verfahren |
| VINECodes |  | [s. VINECodes](dat-europa-cod-2943.md) |
| VINEquipments |  | [s. VINEquipments](ausstattungen-2947.md) |
| VinEquipmentsEncrypted | string | Verschlüsselte Informationen des Herstellers (1) |
| VINColors |  | s. VINColors |
| VINVehicle |  | [s. VINVehicle](herstelleranga-2953.md) |
| VINumber |  | [s. VINumber](vin-nummer-vin-2955.md) |

(1) VinEquipmentsEncrypted

Dieses Feld ist relevant für Fälle, bei denen der Hersteller die DAT verpflichtet,
besondere Herstellerdaten in der VIN-Antwort nur zu internen Zwecken zu verwenden
und niemals an Kunden weiterzugeben. In solchen Fällen nimmt dieses neue Feld diese
Information in Form eines kryptischen Strings auf. Dieser String kann mehrere tausend
Zeichen, auch mehrere zehntausend Zeichen oder mehr beinhalten. Eine Obergrenze gibt
es nicht.

Damit unsere Anwendungen ordnungsgemäß funktionieren muss auch diese verschlüsselte
Information beim VXS-Import übergeben werden.
