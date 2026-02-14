---
title: "Abruf aller Ersatzteilevarianten"
topic_id: "18568"
breadcrumb: "SilverDAT Produkte > SilverDAT calculatePro / SilverDAT calculateExpert > Schnittstellenoperationen > VehicleRepairService > Abruf aller Ersatzteilevarianten"
---

# Abruf aller Ersatzteilevarianten

Die Funktion getSparePartVariants() liefert alle möglichen Ersatzteile für eine DAT-interne Datenverarbeitungsnummer (DVN) und das angegebene Fahrzeug, zusammen mit den Bedingungen, unter denen das Teil
verwendet werden darf oder nicht. Alle optionalen Parameter werden zur Einschränkung
der Ergebnismenge verwendet. Fehlt z.B. der Bauzeitraum, werden alle möglichen Ersatzteile
aus allen Bauzeiträumen zurückgegeben.

Parameter

| Name | Datentyp | Beschreibung |
| --- | --- | --- |
| locale | complexType, Locale | Landeseinstellung, Datenland und Spracheinstellung |
| datECode | String, Pflicht | DAT €uropa-Code |
| datProcessId | Integer, Pflicht | DAT-interne Datenverarbeitungsnummer (DVN) |
| constructionTime | Integer, optional | Bauzeit basierend auf DAT-Notation, 4 Ziffern |
| equipment | List<Long>, optional | Verfügbare Ausstattungen |
| manufacturerCode | List<String>, optional | Herstellercodes |
| vin | String, optional | Fahrzeugidentifikationsnummer |

Rückgabe

| Name | Datentyp | Beschreibung | Kind - Elemente |
| --- | --- | --- | --- |
| datProcessId | Integer | DAT-interne Datenverarbeitungsnummer (DVN) |  |
| equipment | complexType, Equipment | Auflistung aller in den Bedingungen verwendeten Ausstattungen | [name | number]    name(String): Beschreibung der Ausstattung  number (Long): Ausstattungsnummer |
| sparePartVariant | complexType, SparePartVariant | Ersatzteilevarianten | [constructionCondition | constructionTimeFrom | constructionTimeTo | description | excludingCondition | manufactureCodeCondition | partNumber | price | vinCondition]    constructionCondition (String): Verbauungsbedingung  constructionTimeFrom (Integer): Bauzeit von  constructionTimeTo (Integer): Bauzeit bis  description (String): die Beschreibung des Ersatzteils  excludingCondition (String): Ausschlussbedingung  manufactureCodeCondition (String): Herstellercodes  partNumber (String): Ersatzteilnummer  price (BigDecimal/Float):  vinCondition (String): Die letzten angegebenen Stellen müssen alphanumerisch größer sein |
