---
title: "SettingsParameter"
topic_id: "16550"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > SettingsParameters > SettingsParameter"
---

# SettingsParameter

SettingsParameters fungiert als parentNode und kann mit beliebig vielen SettingsParameter bestückt werden. Die Struktur des SettingsParameter Objektes ist immer gleich und hat eine Vielzahl an Attributen.

| Element | Typ | Beschreibung | Wertebereich |
| --- | --- | --- | --- |
| SettingParameter | complexType, optional,  SettingsParameters | Benutzereinstellungen und Betriebseinstellungen |  |
|  | name = String | Definiert, welcher Einstellungsbereich angesprochen wird | [SparePartSettings| LabourSettings | LacquerSettings | GlobalSettings]    SparePartSettings: Ersatzteile-Einstellungen  LabourSettings: Arbeit-Einstellungen  LacquerSettings: Lack-Einstellungen  GlobalSettings: Allgemeine Einstellungen |
| key = String | Definiert den Namen der Einstellung | [SHOW\_FORD\_FINIS\_NUMBER | MANUAL\_TIME\_IN\_HOURS | DAT\_EUROLACQUER\_IN\_HOURS | SPARE\_PART\_INHERIT\_DISCOUNTS | VIN\_AUTOMATIC\_EXECUTION]    SHOW\_FORD\_FINIS\_NUMBER: Ersatzteilnummer statt Ford-Finis-Nummer anzeigen  MANUAL\_TIME\_IN\_HOURS: Manuelle Zeitvorgaben in Stunden  DAT\_EUROLACQUER\_IN\_HOURS: DAT Eurolack in Stunden  SPARE\_PART\_INHERIT\_DISCOUNTS: NfA und Rabatte auch auf zugesteuerte Teile anwenden  VIN\_AUTOMATIC\_EXECUTION: Auskunft über die vom Anwender gesetzte Betriebseinstellung „Automatische VIN Abfrage“ |
| value = Boolean | Enthält den Wert der Einstellung | [true | false] |
| level = String | Definiert die Zugriffsgruppe | [user | company]    user: Benutzereinstellungen  company: Betriebseinstellungen |
