---
title: "Die Angabe von Anmeldedaten (Credentials) im HTTP Header"
topic_id: "6871"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Customer Service > Die Angabe von Anmeldedaten (Credentials) im HTTP Header"
---

# Die Angabe von Anmeldedaten (Credentials) im HTTP Header

Die Anmeldedaten werden bei jedem Funktionsaufruf im HTTP Header angegeben.

| Feld | Beschreibung | Typ und Wertebereich |
| --- | --- | --- |
| customerSignature | Signatur des Kunden | String, Pflicht |
| customerNumber | DAT-Kundennummer | String(7), Pflicht |
| interfacePartnerNumber | DAT-Kundennummer des Schnittstellenpartners | String(7), Pflicht |
| interfacePartnerSignature | Signatur des Schnittstellenpartners | String, Pflicht |
| customerLogin | Benutzername | String(8), Pflicht |
