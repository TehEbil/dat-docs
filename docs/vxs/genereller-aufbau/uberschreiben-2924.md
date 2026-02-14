---
title: "Überschreiben von DAT-Vorgaben"
topic_id: "2924"
breadcrumb: "Datenaustauschformat VXS > Genereller Aufbau > Überschreiben von DAT-Vorgaben"
---

# Überschreiben von DAT-Vorgaben

Bei den mit (DAT) gekennzeichneten Feldern kann der Anwender die von der DAT ermittelten
Werte überschreiben.

In diesem Fall wird der überschriebene Wert mit dem Attribut „origin="user" gekennzeichnet und es gibt ein weiteres Element, das mit „DAT" beginnt und den ermittelten Wert enthält.

Auf diese Weise ist der aktuell zu verwendende Wert immer im selben Element, und die
DAT-Vorgabe ist bei Bedarf nach einem einfachen, festen Schema zu ermitteln.

DAT-Vorgaben können mit origin="dat" gekennzeichnet sein, dies ist aber nicht zwingend der Fall, da das Überschreiben
erst in einer späteren Versionen ermöglicht worden sein könnte oder vom Produkt abhängig
ist.

Beispiele

```
<!-- nicht überschriebene DAT-Standardwerte -->
<SomeValue>42</SomeValue>
<SomeValue origin="dat">0815</SomeValue>
```

```
<!-- Benutzereingabe -->
<SomeOtherValue origin="user">100</SomeOtherValue>
<DATSomeOtherValue>99</DATSomeOtherValue>
```
