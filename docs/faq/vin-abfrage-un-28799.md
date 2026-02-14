---
title: "VIN-Abfrage Unterschied GUI <-> Schnittstelle"
topic_id: "28799"
breadcrumb: "Häufig gestellte Fragen > VIN-Abfrage Unterschied GUI <-> Schnittstelle"
---

# VIN-Abfrage Unterschied GUI <-> Schnittstelle

Die VIN-Abfrage funktioniert über die Webanwendung, aber nicht über die Schnittstelle.

Beschreibung:

Gelegentlich tritt das Problem auf, dass eine VIN-Abfrage über unsere Webanwendung
scheinbar erfolgreich ist, jedoch für dieselbe VIN über die Schnittstelle ein „ECode
not found“-Fehler zurückgegeben wird. Eine Überprüfung der Datenkarte in der Webanwendung
(einsehbar durch das Buch-Symbol) zeigt, dass die VIN-Abfrage hier ebenfalls nicht
erfolgreich war. Erkennbar daran, dass die Untertypvariante als 0000 (unbekannt) angezeigt
wird, da eine der klassifizierenden Ausstattungen nicht gefunden wurde.

Eine mögliche Ursache kann eine fehlende Zuordnung eins Herstellercode zu den DAT-Austattungen
sein. Gerne können die ihren Fall über [interfaces@dat.eu](mailto:interfaces@dat.eu "Mail an DAT interfaces") an uns zur Überprüfung senden.

Lösung:

Die fehlenden Daten müssen vom Benutzer manuell erfasst werden. Unsere Webanwendung
bietet dabei Unterstützung durch einen Automatismus:

- Für die Kombinationsfelder (Comboboxen) der klassifizierenden Ausstattungen (z.B.
  Motor, Karosserie, Getriebe), bei denen nur ein möglicher Eintrag vorhanden ist, wird
  dieser automatisch ausgewählt.

Spezielle Fälle:

Für manche Fahrzeuge ist die Datenlage so, dass für die fehlenden klassifizierenden
Ausstattungen nur ein möglicher Wert vorhanden ist. In diesen Fällen vervollständigt
die GUI die Daten automatisch und die fehlende Untertypvariante wird dadurch automatisch
ermittelt.

Beispiel: Dacia Sandero II Access (01 194 005 050). Starten Sie in der Webanwendung
mit diesem unvollständigen DAT €uropa Code und drücken dann auf die Lupe rechts. Die
Untertypvariante automatisch bestimmt.
