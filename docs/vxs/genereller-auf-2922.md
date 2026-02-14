---
title: "Genereller Aufbau"
topic_id: "2922"
breadcrumb: "Datenaustauschformat VXS > Genereller Aufbau"
---

# Genereller Aufbau

VXS - Vehicle Exchange Structure - ist ein XML-Format. Art und Struktur sind in der
XML Schema Definition VXS.xsd definiert. Es gibt zwei Arten von Elementen:

- Strukturierungen

  Hierzu gehören z.B. <Dossier>, <Vehicle>, u.ä.

  Diese Elemente dienen alleine zum besseren Auffinden der Daten oder sind aus technischen
  Gründen nötig, etwa wenn es mehrere gleichartige „Datensätze" gibt (z.B. mehrere Ausstattungen,
  also <EquipmentPosition>).

  Im Allgemeinen haben Struktur-Elemente keine Attribute und können andere Struktur-Elemente
  und Felder enthalten.
- Felder

  Diese Elemente enthalten die eigentlichen Daten. Der Inhalt ist vom Datentyp abhängig.
