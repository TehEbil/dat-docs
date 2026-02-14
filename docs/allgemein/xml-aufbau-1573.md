---
title: "XML-Aufbau"
topic_id: "1573"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > Arbeiten mit den Webservices > XML Definition > XML-Aufbau"
---

# XML-Aufbau

Wurzelelement

Ein XML-Dokument hat ein Wurzelelement, das alle anderen Elemente und deren Inhalte umschließt:

```
<WurzelElement>
    <Inhalt>Erstes XML-Dokument</Inhalt>
    <Text>Das erste Beispiel für ein
          wohlgeformtes XML-Dokument
    </Text>
</WurzelElement>
```

Kommentare

Nachdem ein Wurzelelement geschlossen ist, sind nur noch Kommentare erlaubt. Kommentare
können im ganzen Dokument verwendet werden. Dies bezüglich gibt es keine Einschränkungen.
Eingeleitet wird ein Kommentar mit einer sich öffnenden spitzen Klammer, gefolgt von
einem Ausrufezeichen und zwei Mittestrichen(<!--). Abgeschlossen wird es mit mit zwei Mittestrichten, gefolgt von einer schliessenden
spitzen Klammer (-->). Der Abschluß erfolgt ohne Ausrufezeichen (!).

```
<!-- Ende des XML-Dokumentes -->
```

Wohlgeformtheit

Ein XML-Dokument hat eine logische und eine physische Struktur. Beide sind durch XML festgelegt. XML kennt folgende Sprachelemente für die physische Struktur:

- XML-Deklaration
- Entitäten

XML kennt folgende Sprachelemente für die logische Struktur:

- Verarbeitungsanweisungen
- Elemente (sogenannte Auszeichner)
- Attribute
- Kommentare
- Text

Dokumente, die gemäß XML korrekt aufgebaut sind, werden als wohlgeformt bezeichnet.
Dafür sind sämtliche von XML spezifizierten Regeln sowohl die physische als auch die
logische Struktur betreffend einzuhalten.

XML ist Case Sensitive

XML ist Case Sensitive. Dies bedeutet, dass zwischen Groß- und Kleinschreibung unterschieden
wird. Es bestehen Unterschiede zwischen folgenden drei Tags:

```
<TestElement>
<TESTELEMENT>
<Testelement>
```

Schließen geöffneter Elemente

Jedes geöffnete Element muss wieder geschlossen werden. Die oben geöffneten Elemente
werden nun geschlossen:

```
</TestElement>
</TESTELEMENT>
</Testelement>
```

Offene Elemente führen zum Abbruch der Interpretation:

```
<p>Hier wird ein Text ausgegeben.
```

Richtig:

```
<p>Hier wird ein Text ausgegeben.</p>
```

Für Elemente ohne Inhalt gibt es eine abgekürzte Variante:

```
<!-- Die lange Variante -->
<Element_ohne_Inhalt></Element_ohne_Inhalt>
```

```
<!-- Die gekürzte Variante -->
<Element_ohne_Inhalt />
```

Korrekte Verschachtelung

Wichtig ist die richtige Verschachtelung von Elementen. Verschachtelungen überkreuz
sind nicht gestattet. Der folgende Code ist daher nicht wohlgeformt:

```
<A_Test>
    <B_Test>
</A_Test>
    </B_Test>
```

Kind-Elemente müssen zuvor geschlossen werden, bevor das Eltern-Element geschlossen
wird:

```
<A_Test>
    <B_Test>
    </B_Test>
</A_Test>
```
