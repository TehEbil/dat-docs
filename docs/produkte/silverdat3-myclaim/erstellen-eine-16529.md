---
title: "Erstellen eines neuen Auftrags mit Option zum Aktualisieren/Überschreiben"
topic_id: "16529"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Erstellen eines neuen Auftrags mit Option zum Aktualisieren/Überschreiben"
---

# Erstellen eines neuen Auftrags mit Option zum Aktualisieren/Überschreiben

Die Funktion createOrUpdateContractN enthält den gleichen Funktionsumfang wie createOrUpdateContract mit der Erweiterung um den optionalen Parameter "mode".

Bitte beachten Sie, dass beim Aktualisieren des Vehicle Objekts oder RepairPositions die Kalkulationsergebnisse automatisch gelöscht werden.

| VorgangsmodusName | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| contractId | Long |  | ID des Auftrags (wird benötigt für die Aktualisierung eines bestehenden Auftrags) |  |
| contractType | String | vro\_calculation,  glass | Gängigste Auftragstypen    - vro\_calculation für Fahrzeuginstandsetzungskalkulationen    - glass für reine Glaskalkulationen | X |
| networkType | String | DAT | Konstante eines bestimmten myclaim Netzes    - DAT für SD3 | X |
| Dossier | Dossier |  | Element das die Vehicle eXchange Struktur (VXS) beinhaltet | X |
| templateId | Long |  | ID der Auftragsvorlage |  |
| templateData | HashMap<String, Object> |  | Bereich bei dem Benutzerdefinierte Vorlagendaten |  |
| complexTemplateData | ComplexTemplateData |  |  |  |
| <mode> | String, optional | [update | replace]    update:  Mit dem mode „update“ werden allen übergebenen Parameter innerhalb des Knotens RepairCalculation aktualisiert    replace:  Ersetzt bzw. überschreibt allen übergebenen Werten innerhalb des Knotens RepairCalculation. Beim Aufruf der Funktion im mode replace werden alle Parameter bis auf die übergebenen Parameter vollständig aus dem Knoten RepairCalculation entfernt. | Vorgangsmodus |  |

Anzeige des Buchsymbols bei Übergabe eines Fahrzeugs

Wenn Sie ein Fahrzeug zuvor über die VIN-Abfrage über die Schnittstelle identifiziert
haben und es in einem neuen Auftrag über createOrUpdateContractN() hinzufügen möchten, achten Sie bitte darauf, dass Sie folgende Elemente im <Vehicle>-Objekt übergeben.

```
<vxs:VehicleIdentNumber>VIN_NUMBER_HERE</vxs:VehicleIdentNumber>
<vxs:TokenOfVinResult="dat">TOKEN_HERE</vxs:TokenOfVinResult>
<vxs:SubModelVariant origin="dat">1</vxs:SubModelVariant>
```

Rückgabe

ID (Auftrags ID) des neu erstellten bzw. aktualisierten Auftrags.
