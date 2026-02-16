---
title: "Anzeige/Abfrage des DAT Systemstatus"
topic_id: "31197"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > Anzeige/Abfrage des DAT Systemstatus"
---

# Anzeige/Abfrage des DAT Systemstatus

Die DAT bietet ihren Kunden eine Vielzahl unterschiedlicher Anwendungen und Dienste
an. Alle Dienste werden von der DAT ständig überwacht, so dass bei einer Störung sofort
die zuständigen Teams eingreifen können, um etwaige Ausfallzeiten zu minimieren. Bisher
war es nicht möglich die Kunden über solche Ereignisse umgehend und präzise zu informieren.

Mit der neu entwickelten Systemstatusanzeige schafft die DAT jetzt volle Transparenz.
Schnittstellenpartner können über Webservice ab sofort in 5-Minuten Intervallen über
Hinweise in den Systemen der DAT informiert werden. Ebenfalls können allgemeine Nachrichten
sowie Nachrichten zu den einzelnen Services abgerufen werden, sobald welche geschalten
sind.

Über die gängigen Ampelfarben kann erkannt werden ob Hinweise vorliegen.

- Grün (Wert 1 im Webservice) signalisiert volle Verfügbarkeit
- Gelb (Wert 0 im Webservice) signalisiert eine eingeschränkte Verfügbarkeit
- Rot (Wert -1 im Webservice) signalisiert eine gestörte Verfügbarkeit

Jeder Service enthält eine Beschreibung der dahinterliegenden Applikation/Funktion,
so dass die Schnittstellenpartner den Anwendern deren Software zielgerichtet nur diejenigen
Services anzeigen können, die dort zum Einsatz kommen.

Bei der entsprechenden Einbindung in den Systemen ist vom Schnittstellenpartner darauf
zu achten, dass von einer „Meldung bei der DAT“ oder „Hinweis bei der DAT“ zu sprechen
ist und der Sprachgebrauch einer „Störung“ nicht zu verwenden ist, da eine Meldung
der Systemüberwachung in dieser Ausprägung mit den 3 gelieferten Werten nicht immer
einer kompletten Störung gleicht.

Um den Systemstatus zu beauftragen, senden Sie bitte eine Mail an [interfaces@dat.eu](mailto:interfaces@dat.eu "Mail DAT interfaces") mit dem Betreff: Systemstatus

- [abfruf-systems-31199](abfruf-systems-31199.md)
- [anzeige-uber-d-31198](anzeige-uber-d-31198.md)
