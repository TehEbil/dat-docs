---
title: "Abholen der Kontaktdaten"
topic_id: "15563"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Schnittstellenoperationen > Abholen der Kontaktdaten"
---

# Abholen der Kontaktdaten

Mit der Funktion getContactData holen Sie die Kontaktdaten zu einem bestehenden Vorgang.

Parameter

| Name | Datentyp | Mögliche Werte | Beschreibung | Pflichtfeld |
| --- | --- | --- | --- | --- |
| contractId | Long |  | Id des Auftrags | X |
| contactDataTypes | AddresKind[] Array | owner  insurer  expert  driver  counterParty  insured  repairer  bodyshop  paintShop  inspectionPlace  opponent  insurant  accidentPlace  buyer  partner  addressBook  additional  insuranceBroker  ownerContactPerson  buyerContactPerson | Kontaktdaten Typ wie z.B. Fahrzeighalter, Versicherungsnehmer,Werkstatt usw. | X |
