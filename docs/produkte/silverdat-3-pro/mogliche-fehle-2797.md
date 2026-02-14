---
title: "Direktes Aufrufen von myClaim über POST-Schnittstelle"
topic_id: "2797"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 PRO > Schnittstellenoperationen > PartsService > Ermittlung von DAT €uropa-Code, Fahrzeuginformationen, Ersatzteilnummer und Preishistorie > Mögliche Fehlercodes getSparePartsDetailsForDPNByVIN"
---

# Direktes Aufrufen von myClaim über POST-Schnittstelle

Diese Funktion erlaubt das direkte Navigieren in die myClaim Webapplikation und somit einem bestimmten Vorgang direkt aufzurufen, ohne sich zuerst
über das DAT Anmeldeportal anmelden zu müssen.

Aufruf

Um einen Vorgang in myClaim direkt zu können öffnen, müssen folgende Parameter in der URL übergeben werden.

1. fabrikat: Das Netz in dem der Vorgang sich befindet (Optional). Für fabrikat wird derselbe
   Wert eingegeben wie für den networkType, z.B. für SD3 der Wert DAT.
2. token: Authentifizierungstoken (Wie Sie einen Token generieren entnehmen Sie bitte im Kapitel
   [JSON Web Token Authentication](../../allgemein/dat-developers-gui/json-web-token-14087.md)
3. claim: Die ID des zu öffnenden Vorgangs

Darstellungsoption: Fullscreen Modus Standard

Um den Arbeitsbereich in myClaim größtmöglich darzustellen, ist es möglich beim Aufruf der URL den Parameter "fullscreen=true" hinten mitzugeben. Mit diesem Parameter werden unter anderem Bereiche wie der linke
Filter, die rechte Historie und die unteren Auftragsdetails ausgeblendet.

MyClaim direkt Aufruf einer URL mit fullscreen Parameter.

Nachdem myClaim mit "fullscreen=true" aufgerufen wurde, werden bestimmte Elemente wie der Header mit der Navigationszeile
und der linke und rechte Bereich ausgeblendet.

Abb1. Aufruf ohne fullscreen=true

https://www.dat.de/myClaim/json/security/Login?fabrikat=FABRIKAT\_HERE&token=TOKEN\_HERE&redirect=inbox.jsp#claim?claim=CLAIM\_ID\_HERE

Abb1b. Aufruf ohne fullscreen=true für die Bewertung

https://www.dat.de/myClaim/json/security/Login?fabrikat=FABRIKAT\_HERE&token=TOKEN\_HERE&redirect=inbox.jsp#claim?claim=CLAIM\_ID\_HERE&subView=bundle\_valuation&tabId=tab-FirstValuationVehicleDataFromValPage

Abb2. Aufruf mit fullscreen=true

https://www.dat.de/myClaim/json/security/Login?fabrikat=FABRIKAT\_HERE&token=TOKEN\_HERE&redirect=inbox.jsp#claim?claim=CLAIM\_ID\_HERE&subView=vro\_calculation&fullscreen=true

Darstellungsoption: Fullscreen Modus Erweitert

Mithilfe des erweiterten Fullscreen Modus wird der Arbeitsbereich von myClaim auf
die bestmögliche Größe skaliert um das Erlebnis z.B. auf einem Tablet noch besser
zu machen.

Um den erweiterten Fullscreen Modus zu aktivieren muss beim Aufruf die URL mit dem
Parameter "extendedFullscreen=true" ergänzt werden.

Abb3. Aufruf mit extendedFullscreen=true

https://www.dat.de/myClaim/json/security/Login?fabrikat=FABRIKAT\_HERE&token=TOKEN\_HERE&redirect=inbox.jsp#claim?claim=CLAIM\_ID\_HERE&subView=vro\_calculation&extendedFullscreen=true

Darstellungsoption: Reiter ausblenden

Mithilfe der URL Parameter Option "hideTabs=true", können die anderen Reiter des Auftrags unsichtbar gemacht werden, so das nur der
aktiv genutzte Reiter sichtbar ist.

Dies kann z.B. hilfreich sein bei bestimmten Restriktionen bei denen man nicht in
die Vorgangsübersicht navigieren darf, oder bei der Unterbindung in einem anderen
Bereich innerhalb des Auftrags.

Mit dieser Option ist nur die Schaltfläche zum Speichern sichtbar. Alle anderen Schaltflächen
zur weiteren Navigation sind deaktiviert.

Abb4. Aufruf mit hideTabs=true

https://www.dat.de/myClaim/json/security/Login?fabrikat=FABRIKAT\_HERE&token=TOKEN\_HERE&redirect=inbox.jsp#claim?claim=CLAIM\_ID\_HERE&subView=vro\_calculation&tabId=TAB\_HERE&hideTabs=true
