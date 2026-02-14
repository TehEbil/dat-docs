---
title: "Aktenzeichen/Vorgänge (Dossiers)"
topic_id: "1369"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers)"
---

# Aktenzeichen/Vorgänge (Dossiers)

Das Hauptelement des XML-Schemas ist <Dossiers>. Es darf nur einmal enthalten sein.

Attribute:

| Element | Typ | Beschreibung |
| --- | --- | --- |
| source | string | Das System, das den Inhalt generiert hat, Für Importe in eine der Glas-Anwendungen: SD3. Für Importe aus Fremdanwendungen wird hier der Name der Anwendung vermerkt. |
| type | string | Die Art bzw. den Zweck der Generierung, etwa spezielle abgespeckte Börsenexporte, z.B. SparePartRequest, GlassRep.  Bei Übergabe an eine Glas-Anwendung muß - zusätzlich zum source=SD3 - einer der folgenden Werte in type gesetzt werden:  - glassrep.mbg für Mercedes-Benz Glas  - glassrep.vwg für Volkswagen Glas  - glassrep.sdg für SilverDAT calculateGlass  - glassrep.agp für autoglas Plus  - glassrep.aug für Audi Glas  - glassrep.nsg für Nissan Glas |
| [Dossier[]](#showid/1371 "Aktenzeichen/Vorgang (Dossier)") | [Dossier[]](#showid/1371 "Aktenzeichen/Vorgang (Dossier)") | Eine Liste von Einzelvorgängen bzw. [Dossier](#showid/1371 "Aktenzeichen/Vorgang (Dossier)")s. |
