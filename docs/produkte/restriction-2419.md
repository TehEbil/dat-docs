---
title: "restriction"
topic_id: "2419"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Datentypen > restriction"
---

# restriction

Über Restrictions werden die Suchergebnisse eingeschränkt. Es kann nur auf das Vorhandensein einer
Restriction geprüft.

| Attribut | Bedeutung | Typ und Wertebereich |
| --- | --- | --- |
| calculationStatus | Kalkulationsstatus | String, mögliche Werte:  "edited" | "sent" | " calculated" |
| contractName | Alle Vorgangsnamen die den Namen enthalte werden berücksichtigt. Es reicht aus wenn der contractName als Namensteil im Vorgang enthalten ist. Die Groß/Kleinschreibung wird ignoriert. | String |
| orderNumber | Auftragsnummer | String |
| invoiceNumber | Rechnungsnummer | String |
| garageContractName | Ansprechpartner Werkstatt / Autohaus | String |
| registrationNumber | Contract Id (cid) | String |
| vin | VIN | String |
| datEcode | ECode | String |
| contractId |  | Long |
| createDateFrom | Schränkt den Erstellungszeitraum ein  Das Intervall kann einseitig offen sein. Um z. B. alle Vorgänge bis zu einem bestimmten Datum anzuzeigen, bleibt das "createDateTo" leer, während das "createDateFrom" gesetzt ist. Umgekehrt können auch alle Verträge ab einem bestimmten Datum gefiltert werden indem "createDateFrom" leer und "createDateTo" gesetzt ist. | AnyType |
| createDateTo | AnyType |
| changeDateFrom | Schränkt den Änderungszeitraum ein  Das Intervall kann einseitig offen sein. Um z. B. alle Vorgänge bis zu einem bestimmten Datum anzuzeigen, bleibt das "changeDateTo" leer, während das "changeDateFrom" gesetzt ist. Umgekehrt können auch alle Verträge ab einem bestimmten Datum gefiltert werden indem "changeDateFrom" leer und "changeDateTo" gesetzt ist. | AnyType |
| changeDateTo | AnyType |
| createUser | Der Parameter ermöglicht die Filterung der Vorgänge nach einem bestimmten Benutzernamen | String, optional |
| filterByUser | Der Parameter ermöglicht die Filterung der Vorgänge nach dem Benutzernamen | Boolean, optional |
| vehicleType | FZA | String |
| manufacturer | HST (nicht ohne FZA) | String |
| baseModel | HT (nicht ohne FZA, HST) | String |
| subModel | UT (nicht ohne FZA, HST, HT) | String |
| insuranceClaim | Versicherungsfall ja, nein (BOOLEAN) | Boolean |
| suitableForOffline |  | Boolean |
