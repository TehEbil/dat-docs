---
title: "Parameter getVehicleApproximateValue"
topic_id: "1818"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Annäherungsbewertung > Parameter getVehicleApproximateValue"
---

# Parameter getVehicleApproximateValue

Bei der Methode getVehicleApproximateValue ist es erforderlich einer der folgenden Parameter anzugeben: model, kba, nationalCode oder datECode.
   
   Die Funktion getVehicleApproximteValue hat eine eine theoretische Laufzeit von 60 – 600 Abfragen pro Minute. Solche Lasten sind anzumelden
      und die DAT behält sich vor bei zuviel unklarer Last den Zugang temporär zu kappen
   Element request
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Abhängigkeit mit 
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
               
                  Hinweis
               
            
            
               
                  locale
               
               
                  Locale
               
               
                  
               
               
                  Beispiel: <Locale country="DE" datCountryIndicator="DE" language="de"/>Sprachauswahl für die GUI
               
               
                  ISO 3166 ALPHA-2: country, datCountryIndicator
               
               
                  X
               
               
                  
               
            
            
               
                  name
               
               
                  String
               
               
                  
               
               
                  Bezeichnung des Vorgangs
               
               
                  
               
               
                  
               
               
                  
               
            
            
               
                  model 
               
               
                  String
               
               
                  kba, nationalCode,  datECode
               
               
                  Modell-Schlüssel (Kombination aus Fahrzeugart-/Hersteller-/Haupttyp- und Untertypschlüssel),
                     zumindest einer der Schlüssel ist Pflicht.
               
               
                  11-stellig, numerisch
               
               
                  bedingt
               
               
                  
               
            
            
               
                  DATEquipmentId
               
               
                  Long
               
               
                  model
               
               
                  Hier können 0-n DAT AV Nummern der klassifizierenden Ausstattung übergeben werden, z.B. Motor und Getriebe. Die Übergabe von Sonderausstattungen ist
                     nicht möglich!
               
               
                  5-stelligweitere Infos siehe Popup-Fenster
               
               
                  
               
               
                  Hier können keine Sonderausstattungen übergeben werden.
               
            
            
               
                  datECode 
               
               
                  String
               
               
                  kba, nationalCode, model
               
               
                  DAT €uropa-Code®  Schlüssel, zumindest einer der Schlüssel ist Pflicht. 
               
               
                  15-stellig, numerisch
               
               
                  bedingt
               
               
                  
               
            
            
               
                  kba
               
               
                  String
               
               
                  datECode, nationalCode,  model
               
               
                  HSN/TSN-Schlüssel, zumindest einer der Schlüssel ist Pflicht. Nur für das Datenland
                     Deutschland zulässig.
               
               
                  [4-stellig numerisch]/[3-stellig alphanumerisch]
               
               
                  bedingt
               
               
                  Bei Verwendung des HSN/TSN-Schlüssel kann die Verabeitungsdauer über 10 Sekunden betragen.
               
            
            
               
                  nationalCode
               
               
                  String
               
               
                  datECode, kba, model
               
               
                  Österreichischer Nationalcode; Schlüssel, zumindest einer der Schlüssel ist Pflicht.
                     Nur für das Datenland Österreich zulässig.
               
               
                  6-stellig, alphanumerisch
               
               
                  bedingt
               
               
                  
               
            
            
               
                  container
               
               
                  String
               
               
                  datECode
               
               
                  Marktindex, wird nur in Verbindung mit dem Parameter: DAT €uropa-Code® gesetzt. 
               
               
                  [Landessetzung, 2-stellig][Nummer des Marktindex, 3-stellig]
               
               
                  
               
               
                  
               
            
            
               
                  constructionTimeFrom
               
               
                  Integer
               
               
                  datECode, container,
                  construtionTimeTo
               
               
                  Bauzeit von; in DAT-Notation (als Filter für die Rückgabe); Dieser Wert wird verwendet,
                     wenn man die construtionTime nicht angeben will.
               
               
                  [4-stellig numerisch]
               
               
                  bedingt
               
               
                  
               
            
            
               
                  constructionTimeTo
               
               
                  Integer
               
               
                  datECode, container,
                  construtionTimeFrom
               
               
                  Bauzeit bis; in DAT-Notation (als Filter für die Rückgabe); Dieser Wert wird verwendet,
                     wenn man die construtionTime nicht angeben will
               
               
                  [4-stellig numerisch]
               
               
                  bedingt
               
               
                  
               
            
            
               
                  constructionTime
               
               
                  Integer
               
               
                  datECode, container
               
               
                  Bauzeit wird nur in Verbindung mit DAT €uropa-Code® und Marktindex gesetzt, Bauzeit in DAT-Notation; eine Berechnungsmöglichkeit finden
                     Sie im Glossar
               
               
                  [4-stellig numerisch]
               
               
                  
               
               
                  
               
            
            
               
                  mileage
               
               
                  Long
               
               
                  registrationDate
               
               
                  Kilometerangabe; Wird das Feld nicht gefüllt, wird die Bezugsfahrstrecke verwendet.
                     Für die Ermittlung der Bezugsfahrstrecke wird das Jahr der Erstzulassung (EZL) verwendet,
                     wenn dieses in der Bauzeit-Von/Bauzeit-Bis Spanne liegt. Liegt die EZL außerhalb dieser
                     Spanne, wird das am nächsten liegende Jahr genommen. Die Bauzeit wird nur für die
                     AV-Bestückung zugrunde gelegt. Die Bezugsfahrstrecke wird auf das echte Fahrzeugalter in Monaten gerechnet. Vorteil
                     ist, dass durch die monatliche Aktualisierung der Kilometerangabe ein besserer Bezug
                     zum Fahrzeugalter möglich ist und der Fahrzeugwert sich kontinuierlicher ändert.Beispiel: EZL 10-2018 --> Datenstand 02/2020 = 16 Monate Bezugsfahrstrecke, Klasse
                     i, Alter 16 Monate = 32.000 km 
               
               
                  numerisch, Default Wert hängt von der Fahrzeugart ab
               
               
                  
               
               
                  
               
            
            
               
                  registrationDate
               
               
                  Date
               
               
                  mileage
               
               
                  Erstzulassung (EZL); Zugelassen sind EZL, die max. 11 Monate vor oder nach den möglichen
                     Bauzeit; Ist mileage nicht gefüllt, wird die EZL benutzt, um die Laufleistung aus der  Bezugsfahrstrecke
                     zu ermitteln. 
               
               
                  YYYY-MM-DD
               
               
                  X
               
               
                  
               
            
            
               
                  approximationSign
               
               
                  String
               
               
                  exFactoryPrice
               
               
                  Bewertungskennzeichen gibt vor, welche Fahrzeugidentifikation aus der Menge der gefundenen
                     Fahrzeugen verwendet werden soll: die günstigste MINIMUM, die teuerste MAXIMUM, diejenige, die dem mitgegebenen Listenneupreis am nächsten liegt APPROXIMATION oder diejenige, die dem Durchschnittswert der Listenneupreise am nächsten liegt AVERAGE. 
               
               
                  MINIMUMAPPROXIMATIONAVERAGEMAXIMUM
               
               
                  X
               
               
                  
               
            
            
               
                  exFactoryPrice
               
               
                  Double
               
               
                  approximationSign
               
               
                  Listenneupreis ist nur erforderlich, wenn approximationSign = APPROXIMATION, ansonsten optional; Der Listenneupreis ist der für dieses Fahrzeug im gewünschten
                     Erstzulassungsjahr letzte gültige Listenpreis in der Konfiguration des DAT €uropa-Code® + Marktindex.
               
               
                  numerisch
               
               
                  bedingt
               
               
                  
               
            
            
               
                  manualEquipmentExFactoryPrice
               
               
                  Integer
               
               
                  
               
               
                  Ein beliebiger Ausstattungsgesamtpreis in Euro
               
               
                  numerisch
               
               
                  bedingt
               
               
                  
               
            
            
               
                  manualEquipmentDevaluations
               
               
                  manualEquipmentDevaluations
               
               
                  
               
               
                  Enthält Abwertungseinstellungselemente
               
               
                  
               
               
                  
               
               
                  
               
            
            
               
                  regionNo
               
               
                  Integer
               
               
                  
               
               
                  Postleitzahl
               
               
                  numerisch
               
               
                  
               
               
                  
               
            
            
               
                  coverage
                  
                     
                        Mit dem Parameter coverage steuern Sie den Datenumfang der zurückgegeben werden soll.
                        
                        
                           
                              
                                 
                                    
                                       Wert
                                    
                                    
                                       Datenumfang
                                    
                                 
                                 
                                    
                                       MARKETPLACEEXPORT
                                    
                                    
                                       Datenumfang COMPLETE ergänzt um die Daten für den Börsenexport (nur SilverDAT 3 PRO).
                                    
                                 
                                 
                                    
                                       EXTENDEDBYTRADING
                                    
                                    
                                       Datenumfang COMPLETE ergänzt um die Unterelemente TradingActivity und TradingAdditional mit den Handelsdaten der Methoden setPurchaseData, setAdmissionData und setSalesData (nur SilverDAT 3 PRO).
                                    
                                 
                                 
                                    
                                       COMPLETE
                                    
                                    
                                       Defaultwert;  Standard Datenumfang für die Datenrückgabe
                                    
                                 
                                 
                                    
                                       NOVALUATIONRESULT
                                    
                                    
                                       Datenrückgabe ohne die Unterelemente Valuation und VAT
                                    
                                 
                                 
                                    
                                       ENRICHED
                                    
                                    
                                       Benennungen entfallen teilweise, aber mit den Bennennungen der Ausstattungen
                                    
                                 
                                 
                                    
                                       BASE
                                    
                                    
                                       Datenrückgabe ganz ohne Benennungen
                                    
                                 
                                 
                                    
                                       SIMPLE
                                    
                                    
                                       Bei diesem Wert entfallen zusätzlich bestimmte  Unterelemente, wie zum Beispiel: CustomerAddress, TradingData, RepairCalculation, RepairOrder,  RegistratinData, Engine, Equipment oder TechInfo.
                                    
                                 
                                 
                                    
                                       NONE
                                    
                                    
                                       Datenrückgabe entweder mit leerem Rahmen, nur mit der DossierId oder nur mit DossierType. 
                                    
                                 
                              
                           
                        
                     
                  
               
               
                  String
               
               
                  
               
               
                  definiert die Datenausgabemenge 
               
               
                  weitere Infos siehe Popup-Fenster von coverage
                  
                     
                        Mit dem Parameter coverage steuern Sie den Datenumfang der zurückgegeben werden soll.
                        
                        
                           
                              
                                 
                                    
                                       Wert
                                    
                                    
                                       Datenumfang
                                    
                                 
                                 
                                    
                                       MARKETPLACEEXPORT
                                    
                                    
                                       Datenumfang COMPLETE ergänzt um die Daten für den Börsenexport (nur SilverDAT 3 PRO).
                                    
                                 
                                 
                                    
                                       EXTENDEDBYTRADING
                                    
                                    
                                       Datenumfang COMPLETE ergänzt um die Unterelemente TradingActivity und TradingAdditional mit den Handelsdaten der Methoden setPurchaseData, setAdmissionData und setSalesData (nur SilverDAT 3 PRO).
                                    
                                 
                                 
                                    
                                       COMPLETE
                                    
                                    
                                       Defaultwert;  Standard Datenumfang für die Datenrückgabe
                                    
                                 
                                 
                                    
                                       NOVALUATIONRESULT
                                    
                                    
                                       Datenrückgabe ohne die Unterelemente Valuation und VAT
                                    
                                 
                                 
                                    
                                       ENRICHED
                                    
                                    
                                       Benennungen entfallen teilweise, aber mit den Bennennungen der Ausstattungen
                                    
                                 
                                 
                                    
                                       BASE
                                    
                                    
                                       Datenrückgabe ganz ohne Benennungen
                                    
                                 
                                 
                                    
                                       SIMPLE
                                    
                                    
                                       Bei diesem Wert entfallen zusätzlich bestimmte  Unterelemente, wie zum Beispiel: CustomerAddress, TradingData, RepairCalculation, RepairOrder,  RegistratinData, Engine, Equipment oder TechInfo.
                                    
                                 
                                 
                                    
                                       NONE
                                    
                                    
                                       Datenrückgabe entweder mit leerem Rahmen, nur mit der DossierId oder nur mit DossierType. 
                                    
                                 
                              
                           
                        
                     
                  
               
               
                  
               
               
                  
               
            
            
               
                  restriction
               
               
                  String
               
               
                  
               
               
                  Filter zur Einschränkung der Ausgabedaten
               
               
                  derzeit nur APPRAISAL
               
               
                  
               
               
                  
               
            
            
               
                  identificationOrder
               
               
                  String
               
               
                  kba, nationalCode,  datECode, model
               
               
                  Gibt die Reihenfolge an, in der übergebene Schlüssel berücksichtigt werden sollen.
                     Die Kombination KBA und nationalCode ist nicht möglich. Die Reihenfolge wird separiert durch das Pipe (|); Default-Wert ist:
                     DATECODE|KBA/NATIONALCODE|MODEL
               
               
                  DATECODE(KBA oderNATIONALCODE)MODEL
               
               
                  
               
               
                  
               
            
            
               
                  vatType
               
               
                  String
               
               
                  
               
               
                  Besteuerungsart; Wird kein Wert oder ein falscher Wert übergeben, wird mit Differenzbesteuerung
                     bewertet.
               
               
                  REGULAR oder R = RegelbesteuerungDIFFERENCE oder D = DifferenzbesteuerungDefault Wert = DIFFERENCE
               
               
                  
               
               
                  
               
            
            
               
                  extendedMileageCorrection
               
               
                  String
               
               
                  
               
               
                  Indikator, seit Mai 2015 ohne Wirkung, da die Bewertung immer mit erweiterter Meilenzahl-Korrektur
                     betrieben wird
               
               
                  
               
               
                  
               
               
                  
               
            
         
      
   
   Element manualEquipmentDevaluations
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Abhängigkeit mit 
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
               
                  Hinweis
               
            
            
               
                  manualEquipmentDevaluation
               
               
                  manualEquipmentDevaluation
               
               
                  manualEquipmentExFactoryPrice
               
               
                  Abwertungseinstellung; darf nur zusammen mit manualEquipmentExFactoryPrice übergeben werden. Die Abwertungseinstellung kann n-mal gesetzt werden (siehe Parameter
                     percent).
               
               
                  
               
               
                  
               
               
                  
               
            
         
      
   
   Element manualEquipmentDevaluation
   
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Abhängigkeit mit 
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
               
                  Hinweis
               
            
            
               
                  devaluationType
               
               
                  String
               
               
                  manualEquipmentExFactoryPrice
               
               
                  Abwertungsart für das gesamte Fahrzeug mit Serienausstattung 
               
               
                  weitere Infos siehe Popup-Fenster devaluationType
               
               
                  X
               
               
                  
               
            
            
               
                  percent
               
               
                  Integer
               
               
                  devaluationType
               
               
                  Prozentangabe; Die Summe aller Prozentangaben darf max. 100 sein. Ist die Summe <
                     100 wird automatisch der Rest mit der Standardabwertung Table2 aufgefüllt. Die Sonderausstattung kann über diesen Parameter in zwei Teile aufgeteilt werden,
                     das jeweils seine eigene Abwertung erhält. Beispiel: Paket1, 60%, RW | Paket2, T4.
               
               
                  numerisch; 1 - 100
               
               
                  X
