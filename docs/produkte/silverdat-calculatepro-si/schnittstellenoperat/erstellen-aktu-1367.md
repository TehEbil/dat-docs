---
title: "Erstellen, Aktualisiern und Überschreiben eines Vorgangs"
topic_id: "1367"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Erstellen, Aktualisiern und Überschreiben eines Vorgangs"
---

# Erstellen, Aktualisiern und Überschreiben eines Vorgangs

Mit der Funktion importDossier() kann einen Vorgang anhand eines Dossiers erstellt, aktualisiert oder überschrieben werden.

Das Vehicle Element eines Dossiers wird beim Export unter "Dossier->Vehicle" sowie "Dossier->RepairCalculation->Vehicle" abgelegt.

Beim Import müssen die beiden Strukturen daher somit immer identische Daten enthalten.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| crud | String, Pflicht | "CREATE" | "UPDATE" | "OVERWRITE"| "OVERWRITE\_KEEP\_POSITIONS" | "OVERWRITE\_KEEP\_ATTACHMENTS" | "CREATE":  Bei "CREATE" wird das Dossier zum ersten Mal neu importiert / angelegt. Es existierte vor der Anlage kein Dossier. Die ID des Dossiers wird beim Import erst generiert. Deshalb darf die ID daher in diesem Fall nicht gesetzt sein.  Der Vorgangsname des Dossiers muss unabhängig hiervon eindeutig sein und darf mit keinem anderen Dossier auf dem Server kollidieren.    "UPDATE":  "UPDATE" aktualisiert ein vorhandenes Dossier. Das Dossier wird anhand des Dossiers Parameters, insbesondere dessen ID Felds identifiziert. Wird kein Dossier mit der ID auf dem Server gefunden, wird ein Fehler zurückgegeben.    Beim Aktualisieren von Dossiers werden nur Elemente hinzugefügt bzw. aktualisiert.    "OVERWRITE":  "OVERWRITE" überschreibt ein vorhandenes Dossier. Das Dossier wird anhand des Dossiers Parameters, insbesondere dessen ID Felds identifiziert. Wird kein Dossier mit der ID auf dem Server gefunden, wird ein Fehler zurückgegeben.    "OVERWRITE\_KEEP\_POSITIONS":  Ersetzt bzw. überschreibt allen übergebenen Werten innerhalb des Dossiers, ausgenommen vom Knoten "RepairPositions"    "OVERWRITE\_KEEP\_ATTACHMENTS":  Ersetzt bzw. überschreibt alle übertragenen Werte innerhalb des Dossiers, ausgenommen vom Knoten "Attachments". |
| [dossiers](../../../vxs/aktenzeichenvo-1369.md) | [Dossiers](../../../vxs/aktenzeichenvo-1369.md) Pflicht |  | Das Dossier, das importiert, aktualisiert oder überschrieben werden soll. Es wird nur das erste Dossier in der Liste der Dossiers berücksichtigt |
| [locale](../../../allgemein/dat-developers-guide/arbeiten-mit-den-web/element-locale-1352.md) | [Locale](../../../allgemein/dat-developers-guide/arbeiten-mit-den-web/element-locale-1352.md), optional |  | [Element locale](../../../allgemein/dat-developers-guide/arbeiten-mit-den-web/element-locale-1352.md) |
| automaticVinRequest | Boolean, optional | true / false    true: Es wird eine automatische VIN-Abfrage durchgeführt  false: Es wird keine automatische VIN-Abfrage durchgeführt | Der Parameter ermöglicht die Fahrzeugidentifikation mit der importDossier-Anfrage.    Bitte beachten Sie, dass hier eine kostenpflichtige VIN-Abfrage durchgeführt wird! |
| withoutCafi | Boolean, Pflicht | true / false | Der Parameter withoutCafi wurde für interne Zwecke geschaffen. Wir empfehlen diesen Parameter stets auf false zu setzen oder zu entfernen. |

Bitte beachten Sie beim gewünschten Erstellen oder Aktualisieren eines Vorgangs in
dem Produkt SilverDAT calculateExpert muss der Parameter <vxs:DossierType>calculateExpert</vxs:DossierType> gesetzt werden.

Bitte beachten Sie beim Aktualisieren eines Vorgangs (CRUD="UPDATE") muss das Vehicle-Objekt stets übergeben werden.

Bitte beachten Sie beim Überschreiben eines Vorgangs (CRUD="OVERWRITE") wird dieser Vorgang bis auf die übergebenen Werten komplett geleert.

Rückgabe

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| contract | Long | Die Contract ID des erstellten oder aktualisierten Vorgangs. |
