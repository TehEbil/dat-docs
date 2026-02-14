---
title: "SVG-Metainformationen zur DVN"
topic_id: "2866"
breadcrumb: "Datenlieferungen > Satzbeschreibung DAT €uropa-Code > Beschreibung Zusatzelement 4 > Erläuterungen zur SVG Schema Definition > SVG-Metainformationen zur DVN"
---

# SVG-Metainformationen zur DVN

Die SVG-Datei wird um Meta-Informationen erweitert. Der SVG-Header bekommt die Information
über Fahrzeugart, Hersteller, Haupttyp, Untertyp und Baugruppe. Diese Information
mappt die Grafik mit der Baugruppe:

Beispiel

```
<svg width="100%" height="100%" viewBox="0 0 83.873 137.419" xmlns:xlink="http://www.w3.org/1999/xlink"
 xml:space="preserve"
    xmlns:dat = 'http://www.dat.de/sphinx/svg'>
...
    <dat:constructionGroup>
          <!-- Fahrzeugart -->
       <dat:fza>1</dat:fza>
      <!-- Hersteller -->
      <dat:hst>340</dat:hst>
      <!-- Haupttyp -->
      <dat:ht>6</dat:ht>
      <!-- Baugruppennummer -->
      <dat:constructionGroupId>9</dat:constructionGroupId>
      <!-- Land -->
      <dat:lkz>D</dat:lkz>
          </dat:constructionGroup>
...
</svg>
```
