---
title: "Parameter getVehicleEvaluation"
topic_id: "2169"
breadcrumb: "SilverDAT Produkte > SilverDAT 3 valuateFinance > Schnittstellenoperationen > Standardbewertung und Standard Restwertprognose > Standardbewertung > Parameter getVehicleEvaluation"
---

# Parameter getVehicleEvaluation

Element request
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
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
               
               
                  15stellig
               
               
                  X
               
            
            
               
                  container
               
               
                  String
               
               
                  Marktindex 
               
               
                  [Landessetzung, 2stellig][Nummer des Marktindex, 3stellig]
               
               
                  X
               
            
            
               
                  constructionTimeFrom
               
               
                  Integer
               
               
                  Bauzeit von; in DAT-Notation (als Filter für die Rückgabe)
               
               
                  [4stellig numerisch]
               
               
                  
               
            
            
               
                  constructionTimeTo
               
               
                  Integer
               
               
                  Bauzeit bis; in DAT-Notation (als Filter für die Rückgabe)
               
               
                  [4stellig numerisch]
               
               
                  
               
            
            
               
                  constructionTime
               
               
                  Integer
               
               
                  Bauzeit in DAT-Notation; eine Berechnungsmöglichkeit finden Sie im Glossar
               
               
                  [4stellig numerisch]
               
               
                  X
               
            
            
               
                  save
               
               
                  String
               
               
                  Speicherkennzeichen;
               
               
                  true,
                  false
               
               
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
               
               
                  
               
            
            
               
                  mileage
               
               
                  Long
               
               
                  Kilometerangabe
               
               
                  numerisch
               
               
                  X
               
            
            
               
                  registrationDate
               
               
                  Date
               
               
                  Erstzulassung; 
               
               
                  JJJJ-MM-DD
               
               
                  X
               
            
            
               
                  restriction
               
               
                  String
               
               
                  Filter zur Einschränkung der Ausgabedaten, Einschränkung auf "nur FI Fahrzeuge", nur
                     "GS Fahrzeuge", "alle Fahrzeuge"
               
               
                  derzeit nur APPRAISAL
               
               
                  X
               
            
            
               
                  equipment
               
               
                  equipment
               
               
                  Enthält Ausstattungselemente als Unterelemente
               
               
                  
               
               
                  
               
            
            
               
                  locale
               
               
                  Locale
               
               
                  Beispiel: <Locale country="DE" datCountryIndicator="DE" language="de"/>
               
               
                  ISO 3166 ALPHA-2: country, datCountryIndicator
               
               
                  X
               
            
            
               
                  vatType
               
               
                  String
               
               
                  Besteuerungsart. Wird kein Wert oder ein falscher Wert übergeben, wird bei Gebrauchtfahrzeugen
                     mit Differenzbesteuerung und bei Neufahrzeugen mit Regelbesteuerung bewertet.
               
               
                  REGULAR oder R = Regelbesteuerung
                  DIFFERENCE oder D = Differenzbesteuerung
               
               
                  
               
            
            
               
                  condition
               
               
                  condition
               
               
                  ermöglicht eine genauere Zustandsbewertung. Beinhaltet noch die folgenden Parameter,
                     um eine exaktere Wertkorrektur durchführen zu können.
               
               
                  
               
               
                  
               
            
            
               
                  extendedMileageCorrection
               
               
                  String
               
               
                  Indikator, seit Mai 2015 ohne Wirkung, da die Bewertung immer mit erweiterter Meilenzahl-Korrektur
                     betrieben wird
               
               
                  
               
               
                  
               
            
            
               
                  licenseNumber
               
               
                  String
               
               
                  Amtliches Kennzeichen
               
               
                  12-stellig
               
               
                  
               
            
         
      
   
   Element equipment
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  equipmentPosition
               
               
                  equipmentPosition
               
               
                  Ausstattung; 0-n Sonderausstattungen können übergeben werden
               
               
                  
               
               
                  
               
            
         
      
   
   Element equipmentPosition
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  datEquipmentId
               
               
                  Integer
               
               
                  DAT-AV Nummer der Sonderausstattung
               
               
                  numerisch
               
               
                  X
               
            
            
               
                  devaluationType
               
               
                  String
               
               
                  Abwertungsart der Ausstattung; 
                  Eine Vorgabe wird nur benötigt, falls Sie die DAT-Standardvorgabe überschreiben möchten.
                     
               
               
                  weitere Infos siehe Popup-Fenster
               
               
                  
               
            
         
      
   
   Element condition
   
      
         
            
               
                  Parameter
               
               
                  Datentyp
               
               
                  Beschreibung
               
               
                  Schreibweise
               
               
                  Pflicht
               
            
            
               
                  increaseInValue
               
               
                  Decimal
               
               
                  Werterhöhung als Geldbetrag
               
               
                  +###########.##
               
               
                  
               
            
            
               
                  decreaseInValue
               
               
                  Decimal
               
               
                  Wertminderung als Geldbetrag
               
               
                  +###########.##
               
               
                  
               
            
            
               
                  tiresMountedValue
               
               
                  Decimal
               
               
                  Wertänderung durch montierte Reifen; im Fahrzeuggrundwert ist bereits der Neupreis
                     der Serienbereifung mit 50 % enthalten. Um diese pauschale Annahme zu verfeinern wird
                     mit dem Parameter eine Wertänderung als Geldbetrag zu diesem angenommenen Restwert
                     angegeben, der sowohl positiv als auch negativ sein kann.
               
               
                  +/-###########.##
               
               
                  
               
            
            
               
                  tiresUnmountedValue
               
               
                  Decimal
               
               
                  Wert der unmontierten Reifen
               
               
                  +###########.##
               
               
                  
               
            
            
               
                  accidentDamage
               
               
                  String
               
               
                  Unfallkennzeichen (nur beschreibend, ohne Einfluss auf Wertkorrektur)
               
               
                  weitere Infos siehe Popup-Fenster
               
               
                  
               
            
            
               
                  numberOfOwners
               
               
                  Integer
               
               
                  Anzahl der Besitzer 
               
               
                  numerisch
               
               
                  
               
            
            
               
                  ownerCorrectionPercent
               
               
                  Decimal
               
               
                  Korrektur durch Anzahl Vorbesitzer in Prozent 
               
               
                  numerisch [0-100]
               
               
                  
               
            
            
               
                  correctionFactorPercent
               
               
                  Decimal
               
               
                  Allgemeiner Wertkorrekturfaktor in Prozent
               
               
                  numerisch [0-200]
               
               
                  
               
            
            
               
                  repairCosts
               
               
                  Decimal
               
               
                  Kosten noch durchzuführender Reparaturen.
               
               
                  +#######.##
               
               
                  
               
            
            
               
                  batteryStateOfHealth
               
               
                  Decimal
               
               
                  Ist - State of Health der Batterie
               
               
                  
               
               
                  
               
            
            
               
                  batteryCorr
               
               
                  Decimal
               
               
                  Wertkorrektur der Traktionsbatterie (Netto)
                  Wenn batteryCorr und batteryCorrGross angegeben wurden, wird batteryCorr in der Bewertung berücksichtigt.
                  Nicht möglich für Fahrzeuge mit DatEquipmentId=76
               
               
                  
               
               
                  
               
            
            
               
                  batteryCorrGross
               
               
                  Decimal
               
               
                  Wertkorrektur der Traktionsbatterie (Brutto)
                  Wenn batteryCorr und batteryCorrGross angegeben wurden, wird batteryCorr in der Bewertung berücksichtigt.
                  Nicht möglich für Fahrzeuge mit DatEquipmentId=76
               
               
                  
               
               
                  
               
            
            
               
                  identificationProcedureStateOfHealth
               
               
                  String
               
               
                  Identifikationsverfahren des Ist - State of Health
                  nur möglich, wenn batteryStateOfHealth gesetzt wurde
