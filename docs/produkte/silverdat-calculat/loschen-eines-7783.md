---
title: "Löschen eines Dossiers/Vorgangs"
topic_id: "7783"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Löschen eines Dossiers/Vorgangs"
---

# Löschen eines Dossiers/Vorgangs

Mit der Funktion deleteDossier() löschen Sie ein bestehender Vorgang.

Arbeitsweise

1. Der betreffende Vorgang wird mittels der übergebenen DossierId gesucht.
2. Der Vorgang wird gelöscht, falls er gefunden werden konnte.
3. Im Erfolgsfall wird true im Tag Success zurückgegeben, andernfalls eine Fehlermeldung.

Eingabedaten

Als Parameter kann nur die DossierId angegeben werden.

| Parameter | Datentyp | Beschreibung |
| --- | --- | --- |
| DossierId | Long, Pflicht | Eindeutige Vorgangskennung |

Rückgabe

Im Erfolgsfall wird im Tag Success der Wert true zurückgeliefert, ansonsten wird eine Fehlermeldung zurückgegeben.
