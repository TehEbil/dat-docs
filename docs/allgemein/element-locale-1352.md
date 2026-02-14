---
title: "Element locale"
topic_id: "1352"
breadcrumb: "Allgemeine Informationen > DAT Developers Guide > Arbeiten mit den Webservices > Wiederkehrende Parameter > Element locale"
---

# Element locale

Das Element locale wird in den meisten Webservices abgefragt, um die richtigen Sprach- und Dateneinstellungen
      vorzunehmen. Das Element locale besteht aus einer Land-/Sprachkombination. Sie können damit Benennungen in abweichender
      Sprache abfragen. 
   Element locale enthält drei Attribute:
   
      
         
            
               
                  Attributname
               
               
                  Codierung
               
               
                  Beschreibung
               
               
                  Beispiel
               
            
            
               
                  country
               
               
                  ISO 3166 ALPHA-2
               
               
                  Landeseinstellung für die Oberfläche, bestehend aus 2 Buchstaben
               
               
                  z.B. "DE"
               
            
            
               
                  datCountryIndicator
               
               
                  ISO 3166 ALPHA-2
               
               
                  Landesflag für den Zielmarkt, bestehend aus 2 Buchstaben
               
               
                  z.B. "DE"
               
            
            
               
                  language
               
               
                  ISO 639-1
               
               
                  Spracheinstellungen für die Oberfläche, bestehend aus 2 Buchstaben
               
               
                  z.B. "de"
               
            
         
      
   
   
   datCountryIndicator
   Die DAT verfügt über Daten verschiedener Länder; um gezielt auf Daten eines Landes
      bzw. Marktes zugreifen zu können, wird der Zielmarkt in den Schnittstellen über locale.datCountryIndicator gesetzt.
   Möchte man zum Beispiel Daten erhalten, die für Deutschland gültig sind, dann wird
      hier "DE" gesetzt. Für Frankreich "FR", für die Türkei "TR" usw. 
   
   country und language
   Unsere Anwendungen sind in der Lage, sämtliche Daten in unterschiedlichen Sprachen
      darzustellen. Hierfür ist die Kombination aus locale.country und locale.language zuständig. Beides zusammen stellt ein sogenanntes Idiom dar. Das System lässt nur
      gültige Idiome zu. Zulässige Beispiele (locale.language-locale.country) sind:
   
      
         deutsch (Deutschland) de-DE
      
      
         englisch (USA) en-US
      
      
         türkisch (Türkei) tr-TR
      
      
         französisch (Frankreich) fr-FR
      
      
         italienisch (Italien) it-IT
      
      
         slowakisch (Slowakei) sk-SK
      
      
         tschechisch (Tschechien) cs-CZ
      
      
         spanisch (Spanien) es-ES
      
      
         russisch (Russland) ru-RU
      
      
         rumänisch (Rümänien) ro-RO
      
      
         ungarisch (Ungarn) hu-HU
      
      
         bulgarisch (Bulgarien) bg-BG
      
      
         holländisch (Niederlande) nl-NL
      
      
         deutsch (Österreich) de-AT
      
      
         polnisch (Polen) pl-PL
      
      
         griechisch (Griechenland) el-GR
      
      
         chinesisch (China) zh-CN
      
      
         deutsch (Schweiz) de-CH
      
      
         französisch (Schweiz) fr-CH
      
      
         italienisch (Schweiz) it-CH
      
      
         koreanisch (Korea) ko-KR
      
   
   Hier eine ungültige Kombination: locale.country=DE und locale.language=tr ist nicht gültig, da "türkisch" keine Amtssprache in Deutschland darstellt.
   
   Mögliche Fehlercodes
   
      
         
            
               
                  Fehlercode
               
               
                  Fehlertext
               
               
                  Beschreibung
               
            
            
               
                  maxLengthCode
               
               
                  Country/ datCountryIndicator /language is too long. Max length is 2
               
               
                  Bitte die Sprach- und Landeseinstellung überprüfen.
               
            
            
               
                  minLengthCode
               
               
                  Country/ datCountryIndicator /language is too short. Min length is 2
               
               
                  Bitte die Sprach- und Landeseinstellung überprüfen.
               
            
            
               
                  authorizationFailed
               
               
                  Authorisation failed.
               
               
                  Bitte die Login-Daten prüfen.
