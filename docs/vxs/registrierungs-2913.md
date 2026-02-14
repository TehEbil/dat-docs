---
title: "Registrierungsdaten (RegistrationData)"
topic_id: "2913"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > Fahrzeug (Vehicle) > Registrierungsdaten (RegistrationData)"
---

# Registrierungsdaten (RegistrationData)

<RegistrationData> ist ein Unter-Element von <Vehicle> und enthält Informationen aus Fahrzeugschein und –brief.

Felder:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| KbaCode | string8 | KBA-Fahrzeugschlüssel im Format HSN/TSN |
| KbaStructurePollution | string30 | KBA-Schlüssel Baugruppe/Schadstoffklasse |
| KbaEngineType | string2 | KBS-Schlüssel Motor |
| LicenseNumber | string30 | KFZ-Kennzeichen |
| LicenseNumberSale | string | KFZ-Kennzeichen bei Verkauf |
| LicenseNumberType | string80 | Art des Kennzeichens |
| RegistrationNumber | string30 | Fahrzeugbrief-Nr. |
| SuspensionDate | date | Abmeldungsdatum |
| CNIT | string | FR: code national d'identification du type, französischer KBA |
| SeasonalLicensePlateMonthFrom | integer | Saisonkennzeichen Zulassungszeitraum Beginn |
| SeasonalLicensePlateMonthTo | integer | Saisonkennzeichen Zulassungszeitraum Ende |
