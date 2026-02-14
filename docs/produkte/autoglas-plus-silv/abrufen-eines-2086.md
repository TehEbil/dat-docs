---
title: "Abrufen eines einzelnen Vorgangs mit getContract"
topic_id: "2086"
breadcrumb: "SilverDAT Produkte > Autoglas Plus SilverDAT inside + SilverDAT calculateGlass > Methodenüberblick > Methoden > Abrufen eines einzelnen Vorgangs mit getContract"
---

# Abrufen eines einzelnen Vorgangs mit getContract

Nur kalkulierte Vorgänge können abgerufen werden.

Mit der Funktion getContract() kann eine bestimmte Kalkulation abgerufen werden. Der Vorgang wird danach als abgerufen
markiert. Die Definition erfolgt mit Übergabe der Auftragsnummer.

Wird ein Vorgang mit getContract abgerufen, kann er nicht nochmals mit getNewContracts() oder getNewContractNumbers() abgerufen werden.
