---
title: "Zuweisung eines Verrechnungssatzes zu einem Auftrag"
topic_id: "2615"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Zuweisung eines Verrechnungssatzes zu einem Auftrag"
---

# Zuweisung eines Verrechnungssatzes zu einem Auftrag

Diese Funktion ermöglicht es zu einem neu erstellten Auftrag einen Verrechnungssatz
zuzuweisen. D.h. wenn ein neuer Auftrag über createOrUpdateContract angelegt wurde und dieser noch nicht gespeichert wurde, ist die Zuweisung eines Verrechnungssatzes
möglich. Nach dem Speichern des Auftrages in myClaim wirkt sich eine erneute Zuweisung eines Verrechnungssatzes in der Kalkulation bzw
im Auftrag nicht mehr aus bzw. ist nicht mehr möglich.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| contractID | Long |  | Identifikationsnummer des neu erstellten Auftrags | X |
| invoiceRateId | Long |  | identifikationsnummer des Verrechnungssatzes | X |

Rückgabe

- True: Falls Zuweisung erfolgreich

- False: Falls Zuweisung fehlgeschlagen
