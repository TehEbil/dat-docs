---
title: "generateToken"
topic_id: "19108"
breadcrumb: "Häufig gestellte Fragen > generateToken"
---

# generateToken

[generateToken](../allgemein/dat-developers-gui/soap-request-g-14126.md) - welche Parameter brauche ich

Um den Token generieren zu können benötigen Sie folgende Zugangs-Parameter:

- DAT-Kundennummer (customerNumber)
- DAT-Benutzer (userLogin)
- Benutzer-Passwort (customerPassword)
- Schnittstellenpartner-Nummer (interfacePartnerNumber) in den meisten Fällen ihre DAT-Kundennummer
- Schnittstellenpartner-Signatur (interfacePartnerSignature)
- optional noch die Produktvariante (productVariant) bei den Expert-Produkten:

  - Produkt valuateExpert -> valuateNG.expert
  - Produkt valuateExpertPlusPartner -> valuateNG.expertPlusPartner
  - Produkt calculateExpert -> calculateExpert

Siehe im Kompendium:

https://www.dat.de/fileadmin/de/support/interface-documentation/MG/SilverDAT\_Schnittstellen-Kompendium\_Mag/#/home/1578/20/21
