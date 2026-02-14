---
title: "Parameter getNewVehicleForecast"
topic_id: "2163"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Standardbewertung und Standard Restwertprognose > Standard Restwertprognose Neufahrzeuge > Parameter getNewVehicleForecast"
---

# Parameter getNewVehicleForecast

Element request
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Abhängigkeit mit
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  locale
               
               
                  Locale
               
               
                  
               
               
                  Beispiel: <Locale country="DE" datCountryIndicator="DE" language="de"/>
               
               
                  ISO 3166 ALPHA-2: country, datCountryIndicator
               
               
                  X
               
            
            
               
                  name
               
               
                  String
               
               
                  
               
               
                  Bezeichnung des Vorgangs 
               
               
                  
               
               
                  
               
            
            
               
                  vin
               
               
                  String
               
               
                  
               
               
                  Fahrzeugidentifikationsnummer (Fahrgestellnummer)
               
               
                  17-stellig
               
               
                  
               
            
            
               
                  datECode
               
               
                  String
               
               
                  
               
               
                  DAT €uropa-Code®
               
               
                  15stellig, numerisch
               
               
                  X
               
            
            
               
                  container
               
               
                  String
               
               
                  
               
               
                  Marktindex
               
               
                  [Landessetzung, 2stellig][Nummer des Marktindex, 3stellig]
               
               
                  
               
            
            
               
                  constructionTimeFrom
               
               
                  Integer
               
               
                  
               
               
                  Bauzeit von; in DAT-Notation (als Filter für die Rückgabe)
               
               
                  [4stellig numerisch]
               
               
                  
               
            
            
               
                  constructionTimeTo
               
               
                  Integer
               
               
                  
               
               
                  Bauzeit bis; in DAT-Notation (schränkt die Rückgabe ein)
               
               
                  [4stellig numerisch]
               
               
                  
               
            
            
               
                  constructionTime
               
               
                  Integer
               
               
                  
               
               
                  Bauzeit in DAT-Notation; eine Berechnungsmöglichkeit finden Sie im Glossar
               
               
                  [4stellig numerisch]
               
               
                  
               
            
            
               
                  save
               
               
                  String
               
               
                  
               
               
                  SpeicherkennzeichenBei save="true" wird ein neuer Datensatz im System angelegt.
               
               
                  true,false
               
               
                  X
               
            
            
               
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
               
               
                  weitere Infos siehe Popup-Fenster
               
               
                  
               
            
            
               
                  restriction
               
               
                  String
               
               
                  
               
               
                  Filter zur Einschränkung der Ausgabedaten, Einschränkung auf "nur FI Fahrzeuge", nur
                     "GS Fahrzeuge", "alle Fahrzeuge"
               
               
                  derzeit nur APPRAISAL
               
               
                  X
               
            
            
               
                  equipment
               
               
                  equipment
               
               
                  
               
               
                  Enthält Ausstattungselemente als Unterelemente
               
               
                  
               
               
                  
               
            
            
               
                  curveType
               
               
                  String
               
               
                  
               
               
                  Kurvenart; 3 Werte zur Auswahl: Minimal, nach DAT oder Maximal
               
               
                  MINIMUM,DAT,MAXIMUM
               
               
                  X
               
            
            
               
                  decreaseType
               
               
                  String
               
               
                  
               
               
                  Abwertungsart
               
               
                  weitere Infos siehe Popup-Fenster
               
               
                  X
               
            
            
               
                  priceType
               
               
                  String
               
               
                  
               
               
                  Einkaufs- oder Verkaufspreis
               
               
                  SALESPRICE - VK,PURCHASEPRICE - EK
               
               
                  X
               
            
            
               
                  IncludeVat
               
               
                  String
               
               
                  
               
               
                  mit oder ohne Mehrwertsteuerangabe
               
               
                  true = mitfalse = ohne 
               
               
                  X
               
            
            
               
                  ValueType
               
               
                  String
               
               
                  
               
               
                  Form der Wertrückgabe
               
               
                  MONETARY -  Beträge in Euro,MILEAGE - Kilometer-Laufleistung;PERCENTAGE - in Prozent 
               
               
                  X
               
            
            
               
                  forecastItems
               
               
                  forecastItems
               
               
                  
               
               
                  Enthält eine Liste mit Restwertprognose-Elementen
               
               
                  
               
               
                  X
               
            
            
               
                  ExternalId
               
               
                  String
               
               
                  
               
               
                  Identifikation im Fremdsystem 
               
               
                  
               
               
                  
               
            
            
               
                  regionNo
               
               
                  Integer
               
               
                  
               
               
                  Postleitzahl 
               
               
                  numerisch 
               
               
                  
               
            
            
               
                  mileageType  
               
               
                  String
               
               
                  mileagePerYear, mileageTotal
               
               
                  Angabe der zu verwendenden Laufleistungsangabe; mögliche Werte:YEAR - der Wert aus mileagePerYear wird verwendet (DEFAULT).TOTAL -  der Wert aus mileageTotal wird verwendet. 
               
               
                  YEAR (default);TOTAL
               
               
                  
               
            
            
               
                  extendedMileageCorrection
               
               
                  String
               
               
                  
               
               
                  Indikator, seit Mai 2015 ohne Wirkung, da die Bewertung immer mit erweiterter Meilenzahl-Korrektur
                     betrieben wird
               
               
                  
               
               
                  
               
            
         
      
   
   Element equipment
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Abhängigkeit mit
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  equipmentPosition
               
               
                  equipmentPosition
               
               
                  
               
               
                  DAT Ausstattung; 0-n Ausstattungen können übergeben werden
               
               
                  -
               
               
                  
               
            
         
      
   
   Element equipmentPosition
   
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Abhängigkeit mit
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  datEquipmentId
               
               
                  Integer
               
               
                  
               
               
                  die DAT-AV Nummer der Sonderausstattung
               
               
                  numerisch
               
               
                  X
               
            
            
               
                  devaluationType
               
               
                  String
               
               
                  
               
               
                  Abwertungsart der Ausstattung;Eine Vorgabe wird nur benötigt, falls Sie die DAT-Standardvorgabe überschreiben möchten.
                     
               
               
                  weitere Infos siehe Popup-Fenster
               
               
                  
               
            
            
               
                  residualValue
               
               
                  Decimal
               
               
                  
               
               
                  Restwert der Ausstattung in Euro
               
               
                  numerisch
               
               
                  
               
            
         
      
   
   Element forecastItems
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Abhängigkeit mit
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  forecastItem
               
               
                  forecastItem
               
               
                  
               
               
                  Das Restwertprognose-Element, 0 - n Wiederholungen möglich
               
               
                  -
               
               
                  X
               
            
         
      
   
   Element forecastItem
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Abhängigkeit mit
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  ageInMonth
               
               
                  Integer
               
               
                  
               
               
                  Alter in Monaten
               
               
                  numerisch [6-72]
               
               
                  X
               
            
            
               
                  mileagePerYear
               
               
                  Long
               
               
                  mileageType
               
               
                  Kilometer Laufleistung pro Jahr. Die maximale Laufleistung pro Jahr beträgt derzeit
                     99.000 Kilometer. 
               
               
                  numerisch
               
               
                  bedingt
               
            
            
               
                  mileageTotal
               
               
                  Long
               
               
                  mileageType
               
               
                  Kilometer-Gesamtlaufleistung; die maximale Gesamtlaufleistung ist derzeit auf 200.000
                     Kilometer beschränkt. 
               
               
                  numerisch
               
               
                  bedingt
