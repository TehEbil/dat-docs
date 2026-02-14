---
title: "Änderungen in den Merkmalskatalogen"
topic_id: "30543"
breadcrumb: "Technische Informationen > Ausgabe Nr. 92 August 2025 > Fahrzeugidentifikation > Erweiterungen > Änderungen in den Merkmalskatalogen"
---

# Änderungen in den Merkmalskatalogen

Zur Nutzung der Schnittstellenfunktion getEquimentAttributes sind in unserem SilverDAT Schnittstellen Kompendium die zugehörigen Merkmalskataloge
dokumentiert. Aktuell werden hier folgende Anpassungen durchgeführt:

Legende der Abkürzungen:

- BG = Baugruppe (dient zur Gruppierung der Ausstattungsattribute)
- FG = Funktionsgruppe (weitere Unterteilung der Baugruppen)
- AM = Ausstattungsmerkmal
- EG = Eigenschaft
- ATT = Attribut (besteht aus BG+FG+AM+EG. Relevant ist eigentlich nur AM und EG)

Die EG 823 „vorn“ wird präzisiert durch EG 268 „Fahrersitz“ und EG 117„Beifahrersitz“.
Das betrifft:

- AM 9112 Sitzheizung
- AM 9137 Schalensitze
- AM 9169 Sportsitze
- AM 9170 Komfort-/Ergonomiesitze
- AM 9129 Sitzmemory
- AM 9093 Sitzbelüftung/-klimatisierung
- AM 9114 Massage-/Aktivsitze
- AM 9119 Lendenwirbelstützen
- AM 9123 Oberschenkelauflagenverstellung

Die EG „…hinten“ werden abgesplittet und in eigene AM „… Rücksitze“ überführt.  
Das Bestehende AM wird später dabei als das relevantere auf „… vorn“ umbenannt. Das
betrifft:

- AM 9169 „Sportsitze“ -> AM 9167 „Sportsitze Rücksitze“
- AM 9129 „Sitzmemory“ -> AM 9138 „Sitzmemory Rücksitze“
- AM 9112 „Sitzheizung“ -> AM 9113 „Sitzheizung Rücksitze“ (das alte ATT wird derzeit
  für interne Zwecke noch beibehalten, entfällt später)
- AM 9170 „Komfort-/Ergonomiesitze“ -> AM 9171 „Komfort/-Ergonomiesitze Rücksitze“
- AM 9093 „Sitzbelüftung/-klimatisierung“ -> AM 9095 „Sitzbelüftung/-klimatisierung
  Rücksitze“ (das alte ATT wird derzeit für interne Zwecke noch beibehalten, entfällt
  später)
- AM 9114 „Massage-/Aktivsitze“ -> AM 9121 „Massage-/Aktivsitze Rücksitze“ (das alte
  ATT wird derzeit für interne Zwecke noch beibehalten, entfällt später)
- AM 9119 „Lendenwirbelstützen“ -> AM 9122 „Lendenwirbelstützen Rücksitze“ (das alte
  ATT wird derzeit für interne Zwecke noch beibehalten, entfällt später)
- AM 9123 „Oberschenkelauflagenverstellung“ -> AM 9139 „Oberschenkelauflagenverstellung
  Rücksitze“

Folgende ATT wurden noch umgebaut (die alten Werte werden derzeit für interne Zwecke
noch beibehalten, entfallen später kommentarlos.)

- Raucherpaket: Bisher 5009-824 „Aschenbecher vorn (Raucherpaket)“, jetzt AM 8129-1
  „Raucherpaket vorhanden“ bei den Ausstattungspaketen. Die AM für die Aschenbecher
  wird beibehalten für einzelne Angaben.
- AM 6012 Tagfahrlicht: Es wurde eine neue EG 925 „Standard“ für das Nicht-LED-TFL eingeführt.
  Die bisherige EG 1 „vorhanden“ wird noch beibehalten und später ausgebaut.
- AM 6010 Nebelscheinwerfer: Es wurde eine neue EG 925 „Standard“ für die Nicht-LED-NSW
  eingeführt. Die bisherige EG 1 „vorhanden“ wird noch beibehalten und später ausgebaut.
- Fernlichtassistent: Bisher nur eine EG im AM 6009 „Lichtfunktionen“, ist es jetzt
  das eigenständige AM 6016 „Fernlichtassistent“. Darin wird auch zwischen dem Standardassistenten
  (Ein/Aus) EG 925 und dem blendfreien Fernlicht EG 50 „adaptiv“ unterschieden.
- AM 6005 LED-Scheinwerfer: Neue EG 929 „Voll-LED“ ersetzt EG 131 „Bi-LED“, zudem wurde
  die EG 1076 „adaptive Lichtverteilung/Matrix“ vom AM 6009 „Lichtfunktion“ direkt hierher
  übertragen.
- Multifunktionslenkrad: Bisher nur eine EG im AM 5036 „Lenkrad“, ist es jetzt das eigenständige
  AM 5051 „Lenkrad mit Multifunktion“.
- Lenkrad mit Schaltfunktion: Bisher nur eine EG im AM 5036 „Lenkrad“, ist es jetzt
  das eigenständige AM 2017 „Schaltung am Lenkrad“ in der FG „Kraftübertragung – Kupplung/Schaltung“.
- Sitzverstellung Rücksitze elektrisch: Das AM 5045 „Sitzverstellung Rücksitze“ wurde
  textuell präzisiert auf „Sitzverstellung Rücksitze elektrisch“, daher Umbau von EG
  290 „2. Sitzreihe elektrisch“ auf EG 9 „2. Sitzreihe“.

Folgende ATT wurden neu organisiert:

- Nichtraucherpaket: Bisher AM 5001 „Ablage - Nichtraucherpaket“, jetzt AM 8130 „Nichtraucherpaket“
  in der FG „Ausstattungspakete“.
- AM 5037 „Lenkraddekor“: Die EG wurden neu definiert und in das AM 5038 (vorher „Lenkradkranz“,
  jetzt umbenannt auf „Lenkradmaterial/-dekor“) integriert.
- AM 5042 „Sonnenblenden“: Die Informationen aus den AM 9111„Sonnenblenden mit Spiegel“:
  AM 6037 „Make-up Spiegel beleuchtet“ und AM 8668 „Sonnenblenden im Fond“ wurden im
  bestehenden AM 5042 „Sonnenblenden“ mit neuen EG integriert.
- AM 5047 Beinauflage klappbar: Die EG „hinten“, „hinten links“ und „hinten rechts“
  wurden ersetzt durch EG 40 „2. Sitzreihe links“ und EG 41 „2. Sitzreihe rechts“.
- AM 5040 „Pedalerie“: EG „Pedale Metall/-optik“ wurde präzisiert und ersetzt in EG
  216 „Edelstahl“, EG 61 „Aluminium“ und für ältere, kombinierte AV EG 964 „Aluminium
  oder Edelstahl“.
- AM 8308 „Fußstütze Fahrer“: EG Metall/-optik“ wurde präzisiert und ersetzt in EG 216
  „Edelstahl“ und EG 61„Aluminium“.

Lackierungen

- Die Lackierungen wurden komplett neu systematisiert. Das betrifft auch die Dachfarben.
- Bis zu 3 vorhandene Karosseriefarben und die Dachfarbe sind jetzt einzeln definierbar,
  um z. B. Mehrfarbenlackierungen mit unterschiedlichen Beschaffenheiten abzubilden
  (Uni/metallic, glänzend/matt etc.).
- Die neuen AM sind 4089 „Lackierung 1“, 4090 „Lackierung 2“, 4093 „Lackierung 3“, 4091
  „Lackierung Dach“.
- Darin enthalten sind jetzt jeweilige Informationen zu

  - Farbgruppen (rot, grün etc.)
  - Uni, Metallic, Perleffekt/Mica
  - Matt, hochglänzend
- Die bisherigen AM 9276 Uni-Lackierung, AM 9274 Metallic/Perleffekt-Lackierung und
  AM 9275 Mehrfarbenlackierung wurden entfernt und in die AM 4089 Lackierung 1 übertragen.
- Die Informationen über die Dachfarbe, die bisher im AM 4044 „Dachausführung/-farbe“
  enthalten waren (matt, uni, schwarz etc.) wurden übertragen in das AM 4091 „Lackierung
  Dach“. Lediglich die EG 447 „Kontrastfarbe“ und EG 390 „Wagenfarbe“ wurde beibehalten.
  Andere Dachbeschaffenheiten wie Carbon, Kunststoff, Leichtbau, vinylbezogen bleiben
  bestehen.
- Die Information über eine Mehrfarbenlackierung ist nun als EG 986 „Mehrfarbenlackierung“
  im AM 4088 „Lackmerkmale“ verfügbar.
- Im AM 4088 „Lackmerkmale“ ist vorläufig noch die EG 537 „matt“ enthalten. Der Wert
  werden derzeit für interne Zwecke noch beibehalten, entfällt später kommentarlos.
