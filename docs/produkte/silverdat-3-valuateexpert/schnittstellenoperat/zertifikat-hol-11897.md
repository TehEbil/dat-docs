---
title: "Zertifikat holen"
topic_id: "11897"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateExpert > Schnittstellenoperationen > Funktionen für Sachverständige > Funktionsumfang > Zertifikat holen"
---

# Zertifikat holen

Mit der Funktion getCertificate holen Sie ein Zertifikat zu dem bestehenden Vorgang.

Vorbedingung: Holen Sie die CertificateId von exportDossierNResponse.

Parameter getCertificate

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| DossierId | Long | Eindeutige Vorgangskennung |  | x |
| CertificateId | String | Eindeutige Zertifikatennummer |  | x |
