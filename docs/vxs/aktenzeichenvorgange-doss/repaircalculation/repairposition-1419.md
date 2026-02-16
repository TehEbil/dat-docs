---
title: "RepairPosition"
topic_id: "1419"
breadcrumb: "Datenaustauschformat VXS > Aktenzeichen/Vorgänge (Dossiers) > RepairCalculation > RepairPositions > RepairPosition"
---

# RepairPosition

Felder:

| Parameter | Typ | Beschreibung | Mögliche Werte |
| --- | --- | --- | --- |
| DATProcessId | Integer, optional | DAT-Datenverarbeitungsnummer (DVN) |  |
| RepairType | String, optional | Reparatur-Art |  |
| Description | String, optional | Beschreibung |  |
| IsManualDescription | Boolean, optional | Wurde der DAT Arbeitstext, der für diese DVN hinterlegt ist, manuell überschrieben? | [true|false]    true: Checkbox"Beschreibung überschreiben" in der Detailerfassung ist aktiv. Das Feld "Description" (Beschreibung) enthält somit der manuell eingegebene Arbeitstext des Benutzers.  Beim Reparaturcode "replace" wird dieser Text als Ersatzteil-Text übernommen, sofern das Feld PartDescription (Beschreibung Ersatzteil) nicht überschrieben wurde.    false: Checkbox "Beschreibung überschreiben" ist inaktiv |
| PartDescription | String, optional | Eine optionale manuelle Beschreibung für das Ersatzteil bei aktiver Checkbox "Beschreibung überschreiben" (IsManualDescription) in der Detailerfassung, ausschließlich beim Reparaturcode "replace".    Wenn das Feld PartDescription (Beschreibung Ersatzteil) leer oder nicht übergeben wird, so wird der Arbeitstext unter „Description" ebenfalls als Ersatzteil-Text verwendet. |  |
| DescriptionId | Integer, optional | Interne Textnummer der Beschreibung, wenn diese nicht manuell überschrieben wurde |  |
| IsForGlass | Boolean, optional | Bestimmt bei den erfassten manuellen Positionen, ob die Reparaturposition in der Glaskalkulation berücksichtigt werden soll. |  |
| Polygon | Integer, optional | Gewähltes Polygon in der Baugruppe |  |
| ConstructionGroupId | Integer, optional | Baugruppen-ID |  |
| ConstructionGroup | String, optional | Baugruppe |  |
| PositionEntryType | String, optional | Art der Eingabeposition | [graphical | manual | additional | removed | maintenance | dents |FREMDLEISTUNG | IFL | AUFBEREITUNG | modifications]    graphical: Standardposition - Anklickbare Position in der graphischen Teileauswahl  manual: Manuelle Position  additionalPosition: Zusatzposition  removed: Aus dem Ergebnis entfernte Positionen  maintenance: Wartungsposition  dents: Hagelpositionen  FREMDLEISTUNG: Fremdleistungsposition  IFL: IFL Position  AUFBEREITUNG: Aufbereitungsposition  modifications:  - manuelle Anpassungen an den Ergebnispositionen bspw. Lackzeit und/oder Lackmaterial bei Lackvorbereitungspositionen.  Betrifft aktuell nur das Datenland Österreich.  - manuelle Anpassung der Preise von den automatisch zugesteuerten Teilen |
| AdditionalInformation | String, optional | Enthält zusätzliche Informationen zur angewählten Schadensposition. Bitte beachten Sie, dass das Element eine reine Ausgabe ist. Eine Übergabe über die Schnittstelle ist ausgeschlossen. |  |
| InspectionReview | Boolean, optional | Gibt an, ob die Schadensposition bei der Inspektions-/Vorortprüfung erfasst wurde | [true|false] |
| OptimizationHandling | String, optional |  |  |
| ConstructionType | String, optional |  |  |
| CrossSeries | Boolean, optional | Positionsbezogene serienübergreifende Kalkulation | [true|false] |
| IsRepairExtension | Boolean, optional | Mögliche Reparaturkostenausweitungs-Position | [true|false] |
| SparePartDiscount | Decimal, optional | Ersatzteilrabatt |  |
| SparePartPriceCorrection | Decimal, optional | Möglicher Auf/Abschlag je Ersatzteil (nur für die Datenländer Tschechien und Slowakei verfügbar) | Prozent, auch negative Werte erlaubt |
| SparePartNumber | String, optional | OEM-Ersatzteilnummer |  |
| SparePartNumberOrigin | String, optional |  |  |
| SparePartNumberManufacturer | String, optional |  |  |
| SparePartPrice | Decimal, optional | Ersatzteilpreis |  |
| SparePartAmount | Decimal, optional | Anzahl Ersatzteile |  |
| SparePartUsed | Boolean, optional |  | [true | false] |
| SparePartExchange | Boolean, optional | Angabe, ob das Ersatzteil als Austauschteil „markiert“ ist, für das es bisher kein Austauschteil gab. Diese Teile werden dann auch bei der Austauschteilsteuer berücksichtigt | [true | false] |
| QuantityUnit | String, optional | Einheit Material | ["" | CCM | DOSE| KART | KG | LFM | LTR | PAAR | PACK | QCM | QDM | QM | SATZ | STCK]    "": keine Angabe  CCM: Kubikzentimeter  DOSE: Dose(n)  KART: Kartuschen  KG: Kilogramm  LFM: Lfd. Meter  LTR: Liter  PAAR: Paar  PACK: Packungen  QCM: Quadratzentimeter  QDM: Quadratdezimeter  QM: Quadratmeter  SATZ: Satz  STCK: Stück |
| SparePartSupplyDescription | String, optional |  |  |
| DamageSegment | Integer, optional | Angabe zu welchem Schaden die entsprechende Schadensposition gehört |  |
| WorkPositionNumber | String, optional | Durch die Übergabe ist es möglich, zwischen beliebigen manuellen Positionen zu differenzieren, selbst wenn diese denselben Namen aufweisen. |  |
| WorkPositionNumberOrigin | String, optional |  |  |
| WorkPositionNumberManufacturer | String, optional |  |  |
| WorkDifficultyLevel | Integer, optional | Arbeitsstufe / Schwierigkeitsgrad |  |
| WorkType | String, optional | Arbeitstyp |  |
| WorkTime | Decimal, optional | Arbeitszeit (Std.) |  |
| WorkLevel | String, optional |  |  |
| WorkPrice | Decimal, optional |  |  |
| WorkPriceOrigin | String, optional |  |  |
| WorkExtensionTime | Decimal, optional | Zusätzliche Arbeitszeit für Reparaturkostenausweitung (Std.) |  |
| WorkExtensionPrice | Decimal, optional | Zusätzliche Lohnkosten Pauschale für Reparaturkostenausweitung  (EUR) |  |
| LacquerLevel | String, optional |  |  |
| LacquerLevelId | Integer, optional |  |  |
| LacquerLevelBaseId | Integer, optional |  |  |
| LacquerPercentage | Decimal, optional |  |  |
| LacquerCountSpotRepair | Integer, optional |  |  |
| LacquerScratchProofFinishTime | Decimal, optional |  |  |
| LacquerPrice | Decimal, optional |  |  |
| LacquerMaterialPrice | Decimal, optional |  |  |
| LacquerMaterialPriceOrigin | String, optional |  |  |
| LacquerWorkPrice | Decimal, optional |  |  |
| LacquerWorkPriceOrigin | String, optional |  |  |
| LacquerMaterialUnitsNumber | Integer, optional |  |  |
| LacquerBlending | Boolean, optional | Beilackierung bei 3/4-Schicht-Lackierung (AZT+Eurolack) | [true | false] |
| PlasticDamageSpotsEasy | Integer, optional |  |  |
| PlasticDamageSpotsAverage | Integer, optional |  |  |
| PlasticDamageSpotsHard | Integer, optional |  |  |
| OverhaulLocation | String, optional |  |  |
| DentsCount | Integer, optional | Anzahl der Dellen    Bei der Hagelmethode CIVD: Durchschnittliche Anzahl Einschläge/m² |  |
| DentsOver20mmCount | Integer, optional |  |  |
| DentsSize | Integer, optional | Dellengröße    Bei der Hagelmethode CIVD: Durchschnittlicher Einschlagdurchmesser bzw. Einschlaggröße in mm |  |
| DentsPartOrientation | String , optional | Bauteillage | horizontal, vertical |
| DentsFlatrate | Decimal, optional | Pauschale (EUR) |  |
| DentsCalculationMethod | String, optional | Hagelkalkulationsmethode    civd = Caravaning Industrie Verband Deutschland  (Veralteter Wert für myClaim: "CIVD")  bvat = Drücken, Bundesverband für Ausbeultechnik BVAT  (Veralteter Wert für myClaim: "BVAT")    german commission =  Drücken, Deutsche Kommission für Lack und Karosserieinstandsetzung    bvat-pre-press = Vordrücken und Lackieren, Bundesverband für Ausbeultechnik BVAT  (Veralteter Wert für myClaim: "PRE\_PRESS\_BVAT")    pre-press = Vorziehen und Lackieren, Deutsche Kommission für Lack und Karosserieinstandsetzung  (Veralteter Wert für myClaim: "PRE\_PRESS")    Die Werte civd, bvat, german commission, bvat-pre-press und pre-press werden auch von myClaim verwendet. | [civd | bvat | german commission | bvat-pre-press | pre-press] |
| DentsWithFinishing | Boolean, optional | Finisharbeit | [true | false] |
| DentsWithSetupTime | Boolean, optional | Rüstzeit einmalig | [true | false] |
| DentsWithAddLightMetals | Boolean, optional |  | [true | false] |
| DentsPrePressTime | Decimal, optional | Vorgabe-Zeit (Std.) |  |
| DentsOutOfReach | Boolean, optional | Arbeiten über Greifzone | [true | false] |
| IsAdditionalLM | Boolean, optional | Zuschlag LM-Teil | [true | false] |
| RepairVariant | String, optional | Reparaturvariante  parking dents: Parkdellen    flattening: Ausbeulhilfe  plastic: Kunststoffreparatur  glass: Glasreparatur | [parking dents | plastic | glass | flattening] |
| PreDamage | Boolean, optional |  | [true | false] |
| GlassDamageSpots | Integer, optional |  |  |
| DentNumberLess | Integer, optional |  |  |
| DentNumberMore | Integer, optional |  |  |
| AlloyLM | Boolean, optional |  | [true | false] |
| LargeScale | Boolean, optional |  | [true | false] |
| AdhesiveTechnologyScale | Boolean, optional |  | [true | false] |
| SetupTime | Integer, optional |  |  |
| BlockWageFlatPrice | Integer, optional |  |  |
| AdditionLM | Boolean, optional |  | [true | false] |
| WorkCompleted | Boolean, optional |  | [true | false] |
| ContainMicroDents | Boolean, optional |  | [true | false] |
| NumDents20 | Integer, optional |  |  |
| NumDents30 | Integer, optional |  |  |
| NumDents45 | Integer, optional |  |  |
| WorkTime20 | Integer, optional |  |  |
| WorkTime30 | Integer, optional |  |  |
| WorkTime45 | Integer, optional |  |  |
| HasAluminium | Boolean, optional |  | [true | false] |
| IsDomusPart | Boolean, optional |  | [true | false] |
| Position | String, optional |  |  |
| Apos2 | String, optional |  |  |
| Apos2MainWork | String, optional |  |  |
| ConstructionGroupMainType | Integer, optional |  |  |
| ConstructionGroupManufacturer | Integer, optional |  |  |
| DVNGroupPositionNumber | Integer, optional |  |  |
| Measure | String, optional |  |  |
| RepairVector | String, optional |  |  |
| SeqNo | Decimal, optional |  |  |
| SparePartDiscountIndicator | Character, optional |  |  |
| WearRus | complexType, optional, MTPLWearRus | Verwendung für einsatzspezifischen Verbrauch nach DVN und/oder Ersatzteilnummer (nur für Russland) |  |
| Finishtype | String, optional |  |  |
| LacquerDifficulty | Integer, optional |  |  |
| GrupoPlastico | String, optional |  |  |
| InputSPD | Integer, optional |  |  |
| InputLP | Integer, optional |  |  |
| InputSDE | Integer, optional |  |  |
| InputSDI | Integer, optional |  |  |
| InputL | Integer, optional |  |  |
| PiezasPO | String, optional |  |  |
| PiezasOP | String, optional |  |  |
| Bulge\_area | Integer, optional |  |  |
| Bulge\_area\_difficulty\_factor | Integer, optional |  |  |
| DMSFlag | String, optional |  |  |
| PartCodeItaly | String, optional |  |  |
| Location | String, optional |  |  |
| WorkTimeItaly | Decimal, optional |  |  |
| WorkLevelItaly | String, optional |  |  |
| WorkManualInput | String, optional | Manuelle Eingabe der Arbeitszeit, nur für SilverDAT calculateItalia | [#]  # = dies bedeutet, dass die Arbeitszeit vom Benutzer manuell auf einen Wert geändert wurde, der nicht der von ANIA erwarteten Logik entspricht |
| NFOPercentage | Decimal, optional |  |  |
| PredamageAmount | Decimal, optional |  |  |
| PredamagePercentage | Decimal, optional |  |  |
| AdhesiveMethod | Boolean, optional | Zuschlag Klebetechnik 30% | [true | false] |
| Length | Decimal, optional | Länge des Ersatzteils.    Bei der Hagelmethode CIVD:  Length\*Width/1000000 = Zu lackierende Gesamtfläche im m² (üblicherweise ist "Width" 1000 und "Length" die Auswahl\*1000, beim Import sind auch andere Werte erlaubt.) |  |
| Width | Decimal, optional | Breite des Ersatzteils.    Bei der Hagelmethode CIVD:  Length\*Width/1000000 = Zu lackierende Gesamtfläche im m² (üblicherweise ist "Width" 1000 und "Length" die Auswahl\*1000, beim Import sind auch andere Werte erlaubt. |  |
| Predefined | Boolean, optional | Vordefinierte Ersatzteilposition |  |
| Manufacturer | String, optional | Ersatzteilhersteller |  |
| Dimension | String, optional | Dimension |  |
| PositionExecutionFlag | String, optional | PositionExecutionFlag ist ein Zeichen, mit dem Applikation weißt, ob die entsprechenden OPEL G+ K Lack Positionen erzeugt werden sollen oder nicht. |  |
| PositionGoodwillPartDescription | String, optional | beschreibt den Name eines Teils. |  |
| PositionEntryTypeKey | Integer, optional | PositionEntryType ist eine Textdarstellung für die Type der zu reparierenden Position. Bei OPEL G+K wird OPELGOODWILL genutzt. |  |
| WorkIndication | Integer, optional | Zeitangabe/Pauschale    ["0" | "1" | "2" | "3" | "4" | "5" | "6"]    0 = keine Eingabe  1 = Arbeitszeit  2 = Lohnkosten Pauschal  3 = Zeit-Aufschlag  4 = Zeit-Abschlag  5 = Erschwerniszuschlag  6 = Pauschale (inkl. Material) | ["0" | "1" | "2" | "3" | "4" | "5" | "6"] |
| IflPositionData | complexType, IflPositionData | IFL Position | [IflWorkData | IflLacquerData | IflMaterialData]    [IflWorkData](iflworkdata-17426.md) (complextype, [IflWorkData](iflworkdata-17426.md) ): Informationen über die IFL Arbeitszeiten  [IflLacquerData](iflworkdata-17426.md) (complextype, [IflWorkData](iflworkdata-17426.md) ): Informationen über die IFL Lackpositionen  [IflMaterialData](iflmaterialdat-17427.md) (complexType, [IflMaterialData](iflmaterialdat-17427.md)):  Informationen über das IFL Material |
| WithSparePart | Boolean, optional |  |  |
| TaxNeutral | Boolean, optional | Der Parameter bestimmt, ob eine HU/AU-Position steuerneutral kalkuliert werden soll. | [true | false] |
| FastTrackOrigin | String, optional |  |  |
| [ParkingDentPositions](parkingdentpos-15552.md) | complexType, optional,  [parkingDentPositions](parkingdentpos-15553.md) | Eingabepositionen für Parkdellen,  [ParkingDentPositions](parkingdentpos-15552.md) dient als Eltern-Element für mehrere (1:n) <[ParkingDentPosition](parkingdentpos-15553.md)>. |  |
| ExternalId | String, optional | Die ExternalId dient als Referenz zwischen den Eingabepositionen (RepairPosition) und den Ergebnispositionen (MaterialPosition, LabourPosition, LacquerPosition, AdditionalCostsPosition) |  |
| ParentRepairType | String, optional | Reparatur-Art (RC) |  |
| ParentDATProcessId | Long, optional | DAT-Datenverarbeitungsnummer (DVN) |  |
| FastTrackOrigin | String, optional | DAT FastTrack ID |  |
| EntryNumber | Integer | Enthält eine Nummer zur Differenzierung der Schadenpositionen bei der manuellen Erfassung |  |
| GeneraliVehicleGroup | Integer | Angabe der für Nebenarbeiten geltenden Festpreise, die im Rahmen der Hagelreparatur gemäß den Vorgaben der Generali zu berücksichtigen sind. Bitte beachten Sie, dass der Parameter nur für die Hagelmethode Bundesverband Ausbeultechnik (BVAT) vorgesehen ist | ["1" | "2" | "3" | "4" | "0"]    [1] Festpreis Nebenarbeiten für Kleinwagen  [2] Festpreis Nebenarbeiten für Mittelklasse  [3] Festpreis Nebenarbeiten für große PKW / SUV / Transporter  [4] Festpreis Nebenarbeiten für Premiumfahrzeuge  [0] Standardoption BVAT-Hagelmethode zurücksetzen |
| LacquerStoneChipProtection | Boolean, optional | Angabe, ob der Steinschlagschutz für das Fahrzeug berücksichtigt wird oder nicht. Bitte beachten Sie, dass dieses Element nur für die Reparaturcodes „Lackieren (L)" und „Montageteil demontiert lackieren (M)" gilt. | [true | false]    true: Der Steinschlagschutz für das Fahrzeug wird berücksichtigt.    false: Der Steinschlagschutz für das Fahrzeug wird nicht berücksichtigt. |
| LacquerCorrosionProtection | Boolean, optional | Angabe, ob der Korrosionsschutz für das Fahrzeug berücksichtigt wird oder nicht. Bitte beachten Sie, dass dieses Element nur für die Reparaturcodes „Lackieren (L)" und „Montageteil demontiert lackieren (M)" gilt. | [true | false]    true: Der Korrosionsschutz für das Fahrzeug wird berücksichtigt.    false: Der Korrosionsschutz für das Fahrzeug wird nicht berücksichtigt. |
