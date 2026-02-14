---
title: "Element metadata"
topic_id: "1620"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > SVG in den DAT Anwendungen > Dokumentstruktur SVG > Wurzelelement svg > Element metadata"
---

# Element metadata

Das Element metadata enthält strukturierte Informationen (Daten) über die in der SVG-Datei enthaltenen Daten. Diese Metainformationen umfassen die folgenden Daten - gegliedert
in weiteren Kindelementen:

| Element | Beschreibung | Vaterelement |
| --- | --- | --- |
| objectInfo | Enthält Titel, Übersetzungen DVN-Nummer, Lage am/im Fahrzeug etc. des graphischen Teilstücks | metadata |
| tooltip | Ergänzende Texte zum graphischen Teilstück, die als Tooltip angezeigt werden können, wenn vorhanden, enthält es eigene Übersetzungen | objectInfo |
| text | Enthält Schriftzüge, die in die Graphik implementiert sind, optional; wird ergänzt durch ein Geschwisterelement "text" zu "metadata" mit der Beschreibung und der textuellen Anzeige | objectInfo |
| title | Der Übersetzungscode des graphischen Teilstücks; findet sein Gegenstück mit Übersetzungen in der svgdescription.xml | objectInfo |
| langs | Enthält die Übersetzungen in verschiedenen Sprachen | title / tooltip / text |
| lang | Auflistung mit den ISO-Sprach- und Länderkennzeichen (in Form von Attributen) und der jeweiligen Übersetzung | langs |
| dvnGroup | DVN-Gruppe; kann aus einem linken und einem rechten Teilstück bestehen | objectInfo |
| kzSeite | Kennzeichen für die Behandlung von Ersatzteilen an der Flash-Oberfläche, die ein bestimmtes Lackkennzeichen aufweisen; mögliche Werte: E (Eurolack) oder H (Herstellerlack) | objectInfo |
| dvnLeft | DVN, Linke Seite | objectInfo |
| dvnRight | DVN, Rechte Seite | objectInfo |
| dvn | DVN-Nummer | dvnLeft / dvnRight |
| etBauart | Kennzeichen für die Behandlung von Ersatzteilen an der Flash-Oberfläche, die bestimmte "EBA" (Ersatzteil Bauart) aufweisen; Das EBA-Kennzeichen ist abhängig von der Bauart (Material, Bauzustand) eines Teils; optional | dvnLeft /dvnRight |
| etBauartOptKz | Kennzeichen für die Behandlung von Ersatzteilen an der Flash-Oberfläche, die bestimmte Merkmale und Kennzeichen aufweisen | dvnLeft / dvnRight |
| rcs | Reparaturcodes, es können mehrere Reparaturcodes zu einer DVN gehören | dvnLeft /dvnRight |
| rc | Reparaturcode, es werden nur Kürzel verwendet | rcs |

Die Kindelemente in metadata werden durch ein Namespace-Alias, das im Prolog definiert wurde, eingeleitet. Im Regelfall ist dies "dat".

Beispiel

```
<g id="Standardebene" fill-rule="evenodd" clip-rule="evenodd" stroke="#000000" stroke-linecap="round" 
fill="none">
  <g id="DATID_068087">
    <metadata>
      <dat:objectInfo position="68">
        <dat:title uebId="32739" stnr="114594">
          <dat:langs>
            <dat:lang languageCode="D" countryCode="D" stnr="114594">Zylinderblock</dat:lang>
            <dat:lang languageCode="H" countryCode="H" stnr="13899058">hengerblokk</dat:lang>
            <dat:lang languageCode="RUS" countryCode="RUS" stnr="16401512">Блок цил.</dat:lang>
            <dat:lang languageCode="E" countryCode="E" stnr="17093863">Bloque de cilindros</dat:lang>
            <dat:lang languageCode="F" countryCode="F" stnr="17359556">Bloc-cylindres</dat:lang>
            <dat:lang languageCode="RO" countryCode="RO" stnr="18331507">Bloc motor</dat:lang>
            <dat:lang languageCode="GR" countryCode="GR" stnr="21854198">Μπλοκ κυλίνδρων</dat:lang>
            <dat:lang languageCode="ENG" countryCode="D" stnr="22096571">cylinder block</dat:lang>
            <dat:lang languageCode="I" countryCode="I" stnr="23871039">monoblocco</dat:lang>
            <dat:lang languageCode="TR" countryCode="TR" stnr="26080954">silindir bloğu</dat:lang>
            <dat:lang languageCode="CZ" countryCode="CZ" stnr="28433360">blok motoru</dat:lang>
            <dat:lang languageCode="SK" countryCode="SK" stnr="30551645">blok motora</dat:lang>
            <dat:lang languageCode="NL" countryCode="NL" stnr="34572703">Cilinderblok</dat:lang>
            <dat:lang languageCode="BG" countryCode="BG" stnr="36102382">Цил.блок</dat:lang>
            <dat:lang languageCode="PL" countryCode="PL" stnr="38557790">blok silnika</dat:lang>
          </dat:langs>
        </dat:title>
        <dat:dvnGroup>0</dat:dvnGroup>
        <dat:kzSeite>e,h</dat:kzSeite>
        <dat:dvnLeft>
          <dat:dvn>80510</dat:dvn>
          <dat:etBauartOptKz>0</dat:etBauartOptKz>
          <dat:rcs>
            <dat:rc>E</dat:rc>
          </dat:rcs>
        </dat:dvnLeft>
      </dat:objectInfo>
    </metadata>
  </g>
```
