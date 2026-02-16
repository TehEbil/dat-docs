---
title: "Beschreibung DAT €uropa-Code Teil 1"
topic_id: "2850"
breadcrumb: "Datenlieferungen > Satzbeschreibung DAT €uropa-Code > Beschreibung DAT €uropa-Code Teil 1"
---

# Beschreibung DAT €uropa-Code Teil 1

Basis-Fahrzeugauswahl auf KBA-Ebene

Der Teil 1 der DAT €uropa-Code®-Lieferung führt anhand von DAT-Auswahlinformationen
(möglichst) eindeutig zu einem KBA-Schlüssel. Hierfür werden die Fahrzeuge gemäß der
DAT-Struktur über die Fahrzeugart, den Hersteller und den Haupttyp bis zum Untertyp
differenziert. Unterhalb des Untertyps erfolgt eine weitere Untergliederung mittels
der für die KBA-Schlüssel relevanten Ausstattungsvarianten (AV) gemäß der vorhandenen
Motorisierung und Karosserieform.

Im Durchschnitt existieren ca. 1,2 KBA-Schlüssel pro möglicher Kombination aus DAT-Untertyp-,
Motor- und Karosserievariante (DAT-UT/Motor-AV/Karosserie-AV). Grund hierfür ist,
dass das KBA in Einzelfällen unterschiedliche HSN/TSN vergibt, sofern das entsprechende
Fahrzeug an weltweit unterschiedlichen Produktionsstandorten der Hersteller gefertigt
wird. Demgegenüber existieren aber pro Hersteller- und Typschlüssel in der Regel auch
mehrere Kombinationen aus den verfügbaren DAT-Untertyp-, Motor- und Karosserievarianten,
da wie oben beschrieben, die DAT-Fahrzeugidentifikation erheblich feiner ist als die
des KBA.

Es wird ein Satz pro UT/Motor-AV/Karosserie-AV – KBA-HSN/TSN – Kombination ausgegeben.

Der Name des XML-Root-Elements lautet „ecode1" und der Name eines Satz-Elements lautet
„ecode1s".
