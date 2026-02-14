---
title: "Mögliche Fehlercodes calculate"
topic_id: "2671"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > Kalkulieren eines Fahrzeugs ohne Speicherung > Mögliche Fehlercodes calculate"
---

# Mögliche Fehlercodes calculate

| Fehlercode | Fehlertext | Beschreibung |
| --- | --- | --- |
| Server.wrongValueCode | Wrong type of wage: "VRO\_REPAIRWAGE\_ELECTRIC" [VRO\_REPAIRWAGE\_BODY|VRO\_REPAIRWAGE\_MECHANIC] | Bitte prüfen Sie den übergebenen Verrechnungssatz |
| Server.wrongValueCode | Illegal DAT Europa-Code | Ungültiger DAT €uropa-Code ( datECode ) |
| Server.wrongValueCode | Invalid repair code, DENTS supports either L (Lacquer) or I (Overhaul)" | Ungültiger Reparaturcode, DENTS unterstützt entweder L (Lack) oder I (Overhaul) " |
| Server.methodHasNoRequest |  | Sie haben keinen Request übergeben |
| Server.parameterRangeError | Double repairCode [repairCode] for datProcessId: [datProcessId] | Sie haben die gleiche DVN mehrfach übergeben. Bitte überprüfen Sie Ihre Request-Parameter. |
| Server.parameterRangeError | Double repairCode [repairCode] for datProcessId: [datProcessId] | Sie haben die gleiche RepairCode/DVN Kombination mehrfach übergeben. Bitte überprüfen Sie Ihre Request-Parameter. |
| Server.parameterRangeError | Only one repairCode from (E,I,R): [E|I|R] for datProcessId: [datProcessId] | Sie haben die gleiche RepairCode/DVN Kombination mehrfach übergeben. Bitte überprüfen Sie Ihre Request-Parameter. |
| Server.parameterRangeError | Only one repairCode from (L,M): [L|M] for datProcessId: [datProcessId] | Sie haben den Repaircode L rather M mehrfach übergeben. Bitte überprüfen Sie Ihre Request-Parameter. |
| Server.contractHasNoCalculation | Contract has no calculation. | Diese Auftragsnummer hat keine gültige Kalkulation. |
| Server.calculationError | Error with the in memory calculation. | Bestimmte Gründe sind möglich. Bitte kontaktieren Sie [interfaces@dat.eu](mailto:interfaces@dat.eu "Mail DAT interfaces"). |
| Server.internalError | Interal Error  There is no VXS available for this contract. | Bestimmte Gründe sind möglich. Bitte kontaktieren Sie [interfaces@dat.eu](mailto:interfaces@dat.eu "Mail DAT interfaces"). |
| Server.userHasNoPermissions | QuickPartCalculation not permitted | QuickPartCalculation ist nicht erlaubt |
