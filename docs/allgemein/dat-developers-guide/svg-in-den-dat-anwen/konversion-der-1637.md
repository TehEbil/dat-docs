---
title: "Konversion der SVG-Datei zu Flash-Image"
topic_id: "1637"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > SVG in den DAT Anwendungen > Implementation > Konversion der SVG-Datei zu Flash-Image"
---

# Konversion der SVG-Datei zu Flash-Image

Es ist möglich, eine SVG-Datei in ein Flash-Image zu konvertieren, um SVG-Dateien für ältere Browser darstellbar zu machen. Dazu wird SVG-Web (WebSVG) benötigt. WebSVG ist eine Javascript-Bibliothek, die SVG-Dateien in fast 95% aller Browser unterstützt.

Vorteile von WebSVG

- funktioniert auch in älteren Browsern, sofern das Plugin installiert bzw. aktiviert ist

Nachteile von WebSVG

- erheblicher Aufwand, um die Konvertierung durchzuführen.
- Einschränkungen bei der Konvertierung zu Flash
- funktioniert nicht lokal
- funktioniert nicht ohne entsprechendes Browser-Plugin

Wegen der umständlichen Implementierung von Event-Handlern, z.B. einem Mouseover,
können wir die Konversion zu Flash nicht empfehlen!

Wenn Sie diese Implementierung nutzen möchten, können Sie sich das Paket unter http://code.google.com/p/svgweb/
herunterladen. Im Paket sind Dokumentationen und Beispiele zur Benutzung enthalten.

Für diese Möglichkeit können wir keinerlei Support übernehmen. Sollten Sie diese Möglichkeit
trotzdem wählen, geschieht dies in eigener Verantwortung!
