---
title: "Element g"
topic_id: "1616"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > SVG in den DAT Anwendungen > Dokumentstruktur SVG > Wurzelelement svg > Element g"
---

# Element g

Mit dem Gruppenelement g werden mehrere graphische Elemente zu einer Einheit zusammengefasst. Sie können dann
zum Beispiel gemeinsam referenziert oder auch transformiert werden. Sie können auch
mit Eigenschaften ausgezeichnet sein, die von g geerbt werden.

Ferner bekommt eine solche Gruppe durch das Element metadata allgemeine Metainformationen.

Gruppenelement [id="Hintergrund"]

Zum Auslesen und für die Darstellung des SVG-Dokumentes kann das Gruppenelement mit der id="Hintergrund" inklusive seiner Kindelemente im Regelfall ignoriert werden. Es ist für die weitere
Bearbeitung nicht von Bedeutung.

Das vorgenannten Gruppenelement enthält im Regelfall die folgenden Kindelemente. Sie
sind sowohl in SVG-Dateien mit Pixelgrafik als auch mit Vektorgrafik zu finden:

| Element | Beschreibung | enthält Kindelemente | Häufigkeit im Dokument |
| --- | --- | --- | --- |
| g | Gruppierungselement | X | N-mal |
| polygon | Linienzug des Hintergrundes |  | 1-mal |

Beispiel

```
<g id="Hintergrund" fill-rule="evenodd" clip-rule="evenodd" stroke="#000000" stroke-linecap="round" fill="none">
```

Gruppenelement [id="Standardebene"]

Mit dem Gruppenelement Standardebene beginnt der eigentliche Teil der Grafik, die zur weiteren Bearbeitung genutzt werden
kann. Es enthält die graphischen und textuellen Informationen, die für die Darstellung
der SVG-Datei benötigt werden.

Jedes graphische Teil besteht aus weiteren graphischen Teilstücken, die unterhalb
der Standardebene aufgelistet werden. Sie werden jeweils innerhalb eines weiteren Gruppenelementes g beschrieben.

Der interne Name jedes graphischen Teilstückes wird über das Attribut "id" im Gruppenelement g bekanntgegeben.

Das Gruppenelement Standardebene enthält im Regelfall die folgenden Kindelemente, wobei zwischen SVG-Dateien mit Pixelgrafik und Vektorgrafik zu unterscheiden ist. Die Auflistung der
Elemente erfolgt nicht in Reihenfolge ihres Auftretens:

| Element | Beschreibung | relevant in Pixelgrafik(P)/ Vektorgrafik(V) | enthält Kindelemente | Häufigkeit im Dokument |
| --- | --- | --- | --- | --- |
| g | Gruppierungselement; enthält u.a. den Namen des graphischen Teilstückes, die [geometrischen Zeichenelemente und -pfade](#showid/1618 "Geometrische Zeichenelemente und -pfade"), die die Grafik darstellen | P / V | X | N-mal |
| [metadata](#showid/1620 "Element metadata") | allgemeine Metainformationen; enthält Name, Übersetzungen DVN-Nummer, Lage am/im Fahrzeug etc. des graphischen Teils | P / V | X | N-mal |

Ein Beispiel hierzu finden Sie im Kapitel [Element metadata](#showid/1620 "Element metadata"), zusammen mit einer beispielhaften Anzeige für die metadata.
