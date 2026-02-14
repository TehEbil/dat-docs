---
title: "Funktionsumfang webScan"
topic_id: "18863"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > Bewertung > Börsendaten via webScan REST-API abrufen > Funktionsumfang webScan"
---

# Funktionsumfang webScan

Die webScan Funktion ermöglicht es eine schnelle Handelsbörsenübersicht für ein ausgewähltes
Fahrzeug zu erhalten. Dabei kann zwischen den zwei folgenden Funktionen gewählt werden:

Übersicht der Funktionen und deren Verfügbarkeit

| Funktion | Beschreibung | Parameter |
| --- | --- | --- |
| marketDataFromVXS | Erstellt eine Börsenübersicht aus einem vollständig identifizierten Fahrzeug ohne die Notwendigkeit der Anlage eines Dossiers. | DATECode  Country  Container  ConstructionTime  InitialRegistration  MilageEstimated |
| marketDataFromDossier | Erstellt eine Börsenübersicht aus einem angelegten Dossier mit vollständig identifizierten Fahrzeug. | DossierId |

Die spezifischen Schnittstellen-Funktionen rufen Sie über folgende URL's auf:

Serviceaufruf:

POST https://www.dat.de/myClaim/rest/marketData/marketDataFromVXS

POST https://www.dat.de/myClaim/rest/marketData/marketDataFromDossier
