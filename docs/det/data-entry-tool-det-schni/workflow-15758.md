---
title: "Workflow"
topic_id: "15758"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Workflow"
---

# Workflow

Der vorgesehene Aktivitätsablauf in einer Datenabrufsitzung ist wie folgt:

Es gibt zwei Alternativen, um geeignete Fahrzeuge zu ermitteln:

- Bei der ersten Alternative werden im ersten Schritt die verfügbaren Fahrzeugmarken
  abgefragt, im zweiten Schritt die verfügbaren Modelle zu einer Marke. Dann werden
  die Derivate eines Modells ohne weitere Beschränkungen abgefragt. Optional können
  die zurückgegebenen grundlegenden Derivatmerkmale dann verwendet werden, um die Menge
  der Derivate durch wiederholtes Aufrufen der Funktion getDerivatives einzugrenzen.
- Bei der zweiten Alternative werden die Derivatmerkmale zusammen mit optionalen Markeninformationen
  angegeben, um sofort eine Liste der Derivate zu erhalten. Diese Liste kann wie bei
  der ersten Alternative eingegrenzt werden.

Nachdem ein einzelnes Derivat ausgewählt wurde, erfolgt die Konfiguration auf Kundenseite.
Im letzten Schritt wird die Schnittstelle aufgerufen, um die ausgewählte Konfiguration
zu validieren.
