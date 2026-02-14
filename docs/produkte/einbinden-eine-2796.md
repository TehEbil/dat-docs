---
title: "Einbinden einer fremden Webseite mit IFrame"
topic_id: "2796"
breadcrumb: "SilverDAT Produkte > SilverDAT®3 myclaim > Datentypen > Einbinden einer fremden Webseite mit IFrame"
---

# Einbinden einer fremden Webseite mit IFrame

MyClaim erlaubt es die Einbindung einer fremden Webseiten innerhalb eines Template Reiters.

Die Inkludierung erfolgt mittels einer spezielen UI Komponente namens "foreignIFrame".

Innerhalb der "foreignIFrame" Komponente muss im callURL Parameter die URL der Webseite die eingebunden werden soll eingetragen werden.

Beispiel

```
<foreignIFrame​ callURL="https://www.anypage.com?contractID=@{claim.id}"postParameters="login=@{user.datrcbkb.benuId}&customerNumber=@{customer.customerNumber}"/>
```
