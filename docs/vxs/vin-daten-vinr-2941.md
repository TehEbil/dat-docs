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
| VINECodes |  | [s. VINECodes](#showid/2943 "DAT Europa-Codes aus dem VIN-Abfrage-Ergebnis (VINECode)") |
| VINEquipments |  | [s. VINEquipments](#showid/2947 "Ausstattungen VIN-Abfrageergebnis (VINEquipments)") |
| VinEquipmentsEncrypted | string | Verschlüsselte Informationen des Herstellers (1) |
| VINColors |  | s. VINColors |
| VINVehicle |  | [s. VINVehicle](#showid/2953 "Herstellerangaben zum Fahrzeug (VINVehicle) ") |
| VINumber |  | [s. VINumber](#showid/2955 "VIN-Nummer (VINumber) ") |

(1) VinEquipmentsEncrypted

Dieses Feld ist relevant für Fälle, bei denen der Hersteller die DAT verpflichtet,
besondere Herstellerdaten in der VIN-Antwort nur zu internen Zwecken zu verwenden
und niemals an Kunden weiterzugeben. In solchen Fällen nimmt dieses neue Feld diese
Information in Form eines kryptischen Strings auf. Dieser String kann mehrere tausend
Zeichen, auch mehrere zehntausend Zeichen oder mehr beinhalten. Eine Obergrenze gibt
es nicht.

Damit unsere Anwendungen ordnungsgemäß funktionieren muss auch diese verschlüsselte
Information beim VXS-Import übergeben werden.
