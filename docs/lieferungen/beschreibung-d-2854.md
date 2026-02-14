---
title: "Beschreibung DAT €uropa-Code Teil 2"
topic_id: "2854"
breadcrumb: "Datenlieferungen > Satzbeschreibung DAT €uropa-Code > Beschreibung DAT €uropa-Code Teil 2"
---

# Beschreibung DAT €uropa-Code Teil 2

Im DAT €uropa-Code® enthaltene Ausstattungen

Der Teil 2 führt anhand von DAT-Auswahlinformationen eindeutig zu einem DAT €uropa-Code®.

Hierfür werden die Fahrzeuge gemäß der DAT-Struktur über die Fahrzeugart, den Hersteller
und den Haupttyp bis zum Untertyp differenziert. Unterhalb des Untertyps erfolgt eine
weitere Untergliederung mittels der klassifizierten charakterisierenden Ausstattungsvarianten.
Bei PKW sind dies neben der Motorisierung und der Karosserieform beispielsweise noch
die Getriebeart und die Ausstattungslinie (bei verschiedenen Herstellern als Paket
vorhanden).

Nicht in Teil 2 enthalten sind die Angaben zum Bauzeitraum des Fahrzeuges sowie dessen
weitere, nicht für die Bildung des DAT €uropa-Codes® relevanten Serien- und Sonderausstattungen
in Abhängigkeit vom genauen Bauzeitpunkt.

Pro DAT €uropa-Code® wird ein Datensatz ausgegeben.

Fahrzeugattribute wie CCM und Kilowatt werden in der Datenbank als einzelne Werte
nicht beim DAT €uropa-Code® geführt, sondern bereits beim DAT-Untertyp. Sie werden
aus dem ersten Untertyp ermittelt, der zum jeweiligen DAT €uropa-Code® passt.

Der Name des XML-Root-Elements lautet „ecode2" und der des Satz-Elements „ecode2\_s".
