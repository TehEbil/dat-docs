---
title: "Abfragen von DVNs anhand von DAT €uropa-Code, Bauzeit und AVs"
topic_id: "18666"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Kalkulation > Abfragen von DVNs anhand von DAT €uropa-Code, Bauzeit und AVs"
---

# Abfragen von DVNs anhand von DAT €uropa-Code, Bauzeit und AVs

Die Funktion getValidDATProcesses() liefert mögliche DAT-interne Datenverarbeitungsnummer (DVNs) anhand von DAT-€uropa-Code, Bauzeit und Ausstattung.

Parameter

Übergeben werden muss ein DAT €uropa-Code und eine gültige Bauzeit, zusammen mit den entsprechenden Ausstattungscodes.

Ein weiterer Parameter (coverage) erlaubt eine Begrezung der Rückgabe des DVNs.

| Name | Datentyp | Mögliche Werte | Beschreibung |
| --- | --- | --- | --- |
| constructionTime | String, optional |  | Bauzeit nach DAT-Notation, 4stellig |
| datECode | String, Pflicht |  | Gültiger DAT €uropa-Code |
| equipment | Long[], optional |  | Alle verfügbaren Sonder- und Serienausstattungen |
| locale | Locale, optional |  | Landeinstellung, Dateland und Spracheinstellung |
| coverage | String, optional | "BASE" | Mit dem Wert BASE werden alle DVNs, die mindestens Reparaturcode "E" (Ersetzen) aufweisen, ausgeliefert |
| "WITH\_MAINTENANCE" | Mit dem Wert WITH\_MAINTENANCE werden alle Wartung-DVNs ausgeliefert |
| "GLASS" | Mit dem Wert GLASS werden alle Glass-DVNs ausgeliefert |
| "HAIL" | Mit dem Wert HAIL werden alle Hagel-DVNs ausgeliefert |
| "COMPLETE" | Mit dem Wert COMPLETE werden alle DVNs mit allen unterstützten Reparaturcodes ausgeliefert |

Rückgabe

Zurückgeliefert wird eine Liste von DVNs zu jedem übergebenen Ausstattungscode. Langbezeichnungen
werden nicht zurückgegeben.

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| datProcessId | Long | DVN-Nummer |
