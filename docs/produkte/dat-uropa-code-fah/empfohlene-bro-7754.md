---
title: "Empfohlene Browser für die DAT Oberflächen-Schnittstellen"
topic_id: "7754"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Oberflächen-Schnittstelle > Integration der Oberfläche > Empfohlene Browser für die DAT Oberflächen-Schnittstellen"
---

# Empfohlene Browser für die DAT Oberflächen-Schnittstellen

Für die DAT Oberflächen-Schnittstellen empfehlen wir die folgenden Browser:

- Google Chrome
- Mozilla Firefox
- Microsoft Edge

Ebenfalls bei der Ausführung von Internet Explorer im Emulations-Modus Edge, bricht das Rendering ab. Der Internet Explorer stolpert in dieser Konstellation über die JQuery inputmask (Jquery-Ui-Plugin jquery.inputmask.bundle.js) und schaltet auf den Quirks-Modus.

Als Workaround empfehlen wir der Default WebBrowser Document Mode 10 oder 11 zu verwenden. Um sicherzustellen, dass der Internet Explorer den Quirks-Modus vermeidet, schlagen wir die folgenden Änderungen vor:

1. Als erste Zeile einfügen:

   ```
       <!DOCTYPE html>
   ```
2. Folgendes als erste Angaben innerhalb des <head>-Tags einfügen:

   ```
       <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
       <meta charset="utf-8">
       <meta name="description" content="" />
       <meta name="viewport" content="width=device-width" />
   ```
