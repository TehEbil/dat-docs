---
title: "Behandlung von neuen Elementen in Responses"
topic_id: "1568"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > Arbeiten mit den Webservices > Behandlung von neuen Elementen in Responses"
---

# Behandlung von neuen Elementen in Responses

Aufgrund von Kundenanforderungen werden immer wieder neue Elemente in unseren Responses
für die neuen SilverDAT Produkte eingebaut. Neue Felder im Response dürfen bei Ihnen nicht zu einem Anwendungsfehler
führen. Falls Sie ein Framework verwenden, dann aktivieren Sie bitte die Option "ignore unknown Elements" (so, oder so ähnlich heißt diese Option).

So gut wie alle bekannten Frameworks bieten die Möglichkeit, unbekannte Elemente zu
ignorieren. Eine Liste der bekanntesten Frameworks finden Sie unter: http://de.wikipedia.org/wiki/Framework.

Es gibt unterschiedliche Methoden, die Option so einzustellen, dass unbekannte Elemente
einfach ignoriert werden. Manchmal werden Klassen zur Verfügung gestellt, die diese
Option zur Verfügung stellen, in manchen Frameworks ist es eine simple Checkbox, die
aktiviert werden muss. Die folgenden zwei Links dienen hier als Beispiele:

- http://msdn.microsoft.com/en-us/library/system.xml.serialization.xmlserializer.unknownelement.aspx
- http://stackoverflow.com/questions/1924216/backwards-compatibility-and-web-services
