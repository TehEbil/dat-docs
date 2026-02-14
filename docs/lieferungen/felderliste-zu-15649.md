---
title: "Felderliste Zusatzelement 4a"
topic_id: "15649"
breadcrumb: "Datenlieferungen > Satzbeschreibung DAT €uropa-Code > Beschreibung Zusatzelement 4a > Felderliste Zusatzelement 4a"
---

# Felderliste Zusatzelement 4a

Die technische Metabeschreibung als XSD (XML SCHEMA DEFINITION) finden Sie als zusatz4a.xsd in der Datenlieferung.

constructiongroups

| Feld | Beschreibung | Datentyp |
| --- | --- | --- |
| constructiongroup | Parent-Node beinhaltet die nachfolgenden Child-Nodes | complexType,  constructiongroupType |
| fza | Fahrzeugart | byte |
| hst | Hersteller | short |
| ht | Haupttyp | short |
| constructionGroupId | Baugruppen-ID | short |
| constructionGroupNames | Baugruppen-Bezeichnung | langsType |
| metadata | Metadaten | metadataType |
| zones | Liste der zugehörigen Fahrzeugzonen | zonenType |
| subModels | Liste der Untertypen, für die die jeweilige Baugruppengrafik Gültigkeit besitzt.  Es handelt sich um eine ODER-Bedingung, d.h. die Baugruppengrafik ist für jeden der gelisteten Untertypen gültig, jedoch ausschließlich für diese, nicht für abweichende Untertypen. | subModelsType |
| options | Liste der Ausstattungen, für die die jeweilige Baugruppengrafik Gültigkeit besitzt.  Es handelt sich um eine ODER-Bedingung, d.h. die Baugruppengrafik ist für jede der gelisteten Ausstattungen gültig, jedoch ausschließlich für diese, nicht für abweichende Ausstattungen. . | optionsType |
| constructionTimeFrom | Bauzeit in DAT Notation ab der die jeweilige Baugruppengrafik Gültigkeit besitzt. | short |

metadataType

| Feld | Beschreibung | Datentyp |
| --- | --- | --- |
| objectInfo | Parent-Node beinhaltet Child-Nodes title, dvnLeft, dvnRight, position | metadataType |
| title | Liste mit Benennung des gezeichneten Bauteils in der zugehörigen Baugruppengrafik (SVG) in allen verfügbaren Übersetzungen. | langsType |
| dvnLeft | Liste der zum Bauteil verfügbaren Reparaturcodes  Hinweis: Existiert nur einen Eintrag für dvnLeft handelt es sich um ein Einzelteil bspw. Windschutzscheibe.  Ansonsten handelt es sich um das Bauteil auf der linken Fahrzeugseite bspw. Kotflügel vorn links. | complexType  dvn, int  rcs, sequence of string |
| dvnRight | Liste der zum Bauteil verfügbaren Reparaturcodes  Hinweis: Existiert nur einen Eintrag für dvnRight handelt es sich um ein Einzelteil bspw. Motorhaube.  Ansonsten handelt es sich um das Bauteil auf der rechten Fahrzeugseite bspw. Kotflügel vorn rechts. | complexType  dvn, int  rcs, sequence of string |
| position | Positions-ID zum jeweiligen Polygon in der zugehörigen Baugruppengrafik (SVG) | int |

zonenType

| Feld | Beschreibung | Datentyp |
| --- | --- | --- |
| zone | Liste von Fahrzeugzonen zu denen die Baugruppengrafik zugeordnet ist. | complexType, zoneType |

subModelsType

| Feld | Beschreibung | Datentyp |
| --- | --- | --- |
| subModel | Untertyp, falls die Baugruppengrafik auf spezifische Untertypen eingeschränkt ist. | short |

optionsType

| Feld | Beschreibung | Datentyp |
| --- | --- | --- |
| option | Ausstattung, falls die Baugruppengrafik auf spezifische Ausstattungen eingeschränkt ist. | unsignedInt |
