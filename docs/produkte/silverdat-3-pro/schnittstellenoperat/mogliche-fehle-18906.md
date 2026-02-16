---
title: "Mögliche Fehlercodes calculateContract()"
topic_id: "18906"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > (Nach-) Kalkulieren eines bestehenden Vorgangs > Mögliche Fehlercodes calculateContract()"
---

# Mögliche Fehlercodes calculateContract()

| Fehlercode | Fehlertext | Beschreibung |
| --- | --- | --- |
| Server.methodHasNoRequest |  | Sie haben keinen Request übergeben. |
| Server.parameterRangeError | Double repairCode [repairCode] for datProcessId: [datProcessId] | Sie haben die gleiche DVN mehrfach übergeben. Bitte überprüfen Sie Ihre Request Parameter. |
| Server.parameterRangeError | Only one repairCode from (E,I,R): [E|I|R] for datProcessId: [datProcessId] | Sie haben die gleiche RepairCode/DVN Kombination mehrfach übergeben. Bitte überprüfen Sie Ihre Request Parameter. |
| Server.parameterRangeError | Only one repairCode from (L,M): [L|M] for datProcessId: [datProcessId] | Sie haben den Repaircode L rather M mehrfach übergeben. Bitte überprüfen Sie Ihre Request Parameter. |
| Server.valueNotFound | Contract [contractId] is not complete for calculation. Necessary entire datECode | Bitte überprüfen Sie die Vorgangsdaten. |
| Server.internalError | Internal Error  There is no VXS available for this contract. | Bestimmte Gründe sind möglich. Bitte kontaktieren Sie [interfaces@dat.eu](mailto:interfaces@dat.eu "Mail DAT interfaces"). |
| Server.calculationError | Error with calculation the result. | Bestimmte Gründe sind möglich. Bitte kontaktieren Sie [interfaces@dat.eu](mailto:interfaces@dat.eu "Mail DAT interfaces"). |
