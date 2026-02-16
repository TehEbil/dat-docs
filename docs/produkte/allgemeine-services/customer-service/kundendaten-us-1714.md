---
title: "Kundendaten: UserData"
topic_id: "1714"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Customer Service > Datentypen > Kundendaten: UserData"
---

# Kundendaten: UserData

Das UserData Objekt enthält die Userdaten/Kundendaten der entsprechenden Kundennummer.

| Attribut | Bedeutung | Typ und Wertebereich |
| --- | --- | --- |
| customerNumber | DAT-Kundennummer | String(7) |
| userLogin | Login für den automatisch angelegten Benutzer. Der Login wird von der DAT erzeugt. | String(8) |
| userPassword | Password, das die DAT initial vergibt, bei der Anlage des Benuzters. | String(8) |
| externalCustomerID | Externe Kundennummer. Diese Kundennummer wird bei der Anlage des Kindkunden im Objekt customer als externalCustomerID übergeben. | String(12) |
