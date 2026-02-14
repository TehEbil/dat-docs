---
title: "Exportieren von Dokumenten (SilverDAT 3 valuateExpert, valuateExpertPlusPartner)"
topic_id: "12657"
breadcrumb: "SilverDAT Produkte > Allgemeine Services > Verwalten von Vorgängen > Funktionsumfang Vorgangsverwaltung > Exportieren von Dokumenten (SilverDAT 3 valuateExpert, valuateExpertPlusPartner)"
---

# Exportieren von Dokumenten (SilverDAT 3 valuateExpert, valuateExpertPlusPartner)

Mit der Funktion exportDossierN generieren Sie ein Druckprodukt auf Basis eines bestehenden Vorgangs

Übersicht der Funktionalitäten und deren Verfügbarkeit

| Typ | DossierType | ValuationType | SilverDAT 3 valuateExpert/  PlusPartner |
| --- | --- | --- | --- |
| stichtagsbezogene beziehungsweise  historische Bewertung | valuateExpert  valuateExpertPlusPartner | valuation | X |

Arbeitsweise

1. Es wird geprüft, ob die angegebenen Werte für das Export-Produkt und das Export-Format
   unterstützt werden und ob deren Kombination gültig ist.
2. Der betreffende Vorgang wird mittels der übergebenen DossierId gesucht.
3. Es wird geprüft, ob die Bewertung des Vorgangs aktuell ist.
4. Generierung der Export-Daten unter Berücksichtigung eventuell angegebener Optionen
   für die Darstellung.
5. Im Erfolgsfall wird das Druckprodukt als Base64 kodierter String zurückgegeben, ansonsten wird eine Fehlermeldung zurückgegeben.

Eingabedaten

Es werden nur die nachfolgend beschriebenen Parameter unterstützt, nicht erwähnte
Parameter werden ignoriert.

Für die Parameter wurden folgende Namespace-Definitionen festgelegt:

xmlns:dos="http://www.dat.de/services/Dossier1N" für SilverDAT 3 valuateExpert/PlusPartner

xmlns:vxs="http://www.dat.de/vxs"

Rückgabe

Im Erfolgsfall wird ein Dokument als String im Base64-Format zurückgegeben. Bei Urkunden wird zusätzlich eine Urkundennummer CertificateId generiert. Im Fehlerfall wird eine Fehlermeldung zurückgegeben.

Hinweis zur Weiterverarbeitung

Sie erhalten ein gültiges Dokument, indem Sie die erhaltenen Daten Base64 decodieren und diese in einer binären Datei mit der Endung PDF speichern.
