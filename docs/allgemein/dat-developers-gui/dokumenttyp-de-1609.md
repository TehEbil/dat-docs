---
title: "Dokumenttyp-Deklaration"
topic_id: "1609"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > SVG in den DAT Anwendungen > Dokumentstruktur SVG > Dokumenttyp-Deklaration"
---

# Dokumenttyp-Deklaration

Die Dokumenttyp-Deklaration (DOCTYPE) steht im Regelfall direkt nach dem Prolog eines XML-Dokumentes und vor dem Wurzelelement. Die DOCTYPE bezeichnet den Hauptteil des Dokumentes, definiert welche Elemente auftreten können,
und gibt die Quelle an, die eine formale Beschreibung der möglichen Elemente enthält.
Hier ein Beispiel für SVG 1.0:

```
<!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 1.x//EN" "http://www.w3.org/Graphics/SVG/1.x/DTD/svg1x.dtd">
```

Bei den SVG-Dateien mit Pixelgrafik kann eine Dokumenttyp-Deklaration auch fehlen. Sie kann durch
die zwei folgenden Attribute im Tag <svg> ersetzt werden. Dies wird aus Kompatibilitätsgründen vorgeschlagen:

| Attribut-Name | Mögliche Werte | Beschreibung |
| --- | --- | --- |
| version | "1.0" | "1.1" | "1.2" | Gibt die SVG Sprachversion des SVG Dokumentes wieder |
| baseProfile | "none" | "full" | "basic" | "tiny" | Beschreibt das SVG Sprachprofil, das notwendig ist, um den Inhalt korrekt zu rendern; vorgeschlagener Wert: "full" |

Ein Implementierungsbeispiel zu den Attributen finden Sie im Kapitel [Wurzelelement svg](wurzelelement-1611.md).
