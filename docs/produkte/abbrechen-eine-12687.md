---
title: "Abbrechen eines Auftrags"
topic_id: "12687"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Neubewertung und Nachbewertung der Dossiers > Abbrechen eines Auftrags"
---

# Abbrechen eines Auftrags

Mit der Funktion cancelTaskN brechen Sie den angegebenen Auftrag ab. Der Auftrag muss sich dafür im Status INWORK oder WAITING befinden. Wenn die Methode cancelTaskN aufgerufen wird, dann wird der Auftragsstatus CANCELED angezeigt.

Parameter cancelTaskN

| Name | Datentyp | Beschreibung | Schreibweise | Pflicht |
| --- | --- | --- | --- | --- |
| TaskId | Integer | Auftragsnummer |  | X |
