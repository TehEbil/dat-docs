---
title: "Mehrere unvollständige Fahrzeuge"
topic_id: "21940"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Fahrzeugidentifikation anhand VIN (VIN-Abfrage) > ECode not found  - Datenkarte > Mehrere unvollständige Fahrzeuge"
---

# Mehrere unvollständige Fahrzeuge

Beispiel Test-VIN VF3DEXTESTSTUB005

In manchen Fällen kann es auch vorkommen, dass mehrere unvollständige DAT €uropa-Codes® in der Fehlermeldung "ECode not found" enthalten sind. In diesem Fall werden in unserer Web-Anwendung die möglichen Fahrzeuge
zur Auswahl angezeigt. Über Schnittstelle findet man dann unter <additionalInformation> zum ersten Fahrzeug in <MetaPositions> eine Liste der weiteren möglichen DAT €uropa Codes® mit dem Schlüssel "additionalVehicle". Der enthaltene Wert wird im Format [VinAccuracy]: [DAT €uropa Code],[Bauzeit] ausgegeben.

Beispiel

```
<ns2:MetaPosition key="additionalVehicle" value="4: 026701050100000,5416"/>
```

enthaltene Fahrzeugdaten

```
<additionalInformation>
   <ns2:Vehicle xmlns:ns2="http://www.dat.de/vxs">
      <ns2:VehicleIdentNumber>VF3DEXTESTSTUB005</ns2:VehicleIdentNumber>
      <ns2:ConstructionTime>5416</ns2:ConstructionTime>
      <ns2:VehicleTypeName>Transporter</ns2:VehicleTypeName>
      <ns2:ManufacturerName origin="dat">Peugeot</ns2:ManufacturerName>
      <ns2:BaseModelName origin="dat">Boxer (330/333/335/435) Pritsche RS4035mm (2007-&gt;)</ns2:BaseModelName>
      <ns2:SubModelName origin="dat">HDi Doppelkabine (335)</ns2:SubModelName>
      <ns2:VehicleType>2</ns2:VehicleType>
      <ns2:Manufacturer>670</ns2:Manufacturer>
      <ns2:BaseModel>87</ns2:BaseModel>
      <ns2:SubModel>12</ns2:SubModel>
      <ns2:VinAccuracy>3</ns2:VinAccuracy>
      <ns2:SubModelVariant>0</ns2:SubModelVariant>
      <ns2:VINResult>
         <ns2:VINEquipments>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>B0A02</ns2:ManufacturerCode>
               <ns2:ShortName>NUTZFAHRZEUGE</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>B0B0P</ns2:ManufacturerCode>
               <ns2:ShortName>PEUGEOT</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>B0CU9</ns2:ManufacturerCode>
               <ns2:ShortName>BOXER 3</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>B0D6X</ns2:ManufacturerCode>
               <ns2:ShortName>LKW-FAHRGESTELL MIT KABINE DOPPELT, LANG TYP 16</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>B0E0H</ns2:ManufacturerCode>
               <ns2:ShortName>STANDARD</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>B0FDQ&amp;TMG</ns2:ManufacturerCode>
               <ns2:ShortName>TURBODIESEL PUMA C 96 EURO5 130 PS</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>B0H04</ns2:ManufacturerCode>
               <ns2:ShortName>(D)</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>B0K0C</ns2:ManufacturerCode>
               <ns2:ShortName>HAUPTINDEX "0C"</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>B0MP0</ns2:ManufacturerCode>
               <ns2:ShortName>DECKENDE LACKIERUNG</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>B0NWP</ns2:ManufacturerCode>
               <ns2:ShortName>EWP - LACK WEISS BANQUISE</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>B0P35</ns2:ManufacturerCode>
               <ns2:ShortName>STOFF DARKO + TWILL "35"</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>B0RFX</ns2:ManufacturerCode>
               <ns2:ShortName>"FX"</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DAB00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE DIEBSTAHLSICHERUNG</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DAL00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE SITZ HINTEN</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DAN00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE ZUSATZ SITZBANK</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DAQ00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE ANHANGERKUPPLUNG</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DBF01</ns2:ManufacturerCode>
               <ns2:ShortName>OBERE BATTERIE</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DBQ00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE VERSTRKUNG ELEKTRISCHE AUSRSTUNG</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DBV13</ns2:ManufacturerCode>
               <ns2:ShortName>AUFLIEGER DOPPELKABINE</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DCD06</ns2:ManufacturerCode>
               <ns2:ShortName>DIESEL</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DCJ03</ns2:ManufacturerCode>
               <ns2:ShortName>STANDARD GESTELL</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DCP01</ns2:ManufacturerCode>
               <ns2:ShortName>ANZEIGE IN KM/H</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DCW58</ns2:ManufacturerCode>
               <ns2:ShortName>ANTRIEBSMOMENT 13 X 68</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DCX01</ns2:ManufacturerCode>
               <ns2:ShortName>LINKSLENKER</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DCY02</ns2:ManufacturerCode>
               <ns2:ShortName>MONTAGE MIT FERNBEDIENUNG</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DDK00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE ZUSATZ HEITZUNG</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DDO00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE FREISPRECHSET</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DDV20</ns2:ManufacturerCode>
               <ns2:ShortName>TM 18 X 14</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DDX01</ns2:ManufacturerCode>
               <ns2:ShortName>ANTI-SCHLUPF</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DES00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE ANSCHLUSS FUER ZUBEHOER</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DFE09</ns2:ManufacturerCode>
               <ns2:ShortName>SIGNALLEUCHTEN LANGES FAHRZEUG</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DFO00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE GEHÄUSE SITZ</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DFX00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE ZUSATZ UNTERMOTORSCHUTZ</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DGG00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE AUSSTATTUNG VERKLEIDUNG</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DGY33</ns2:ManufacturerCode>
               <ns2:ShortName>MOTOREN FORD</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DGZ14</ns2:ManufacturerCode>
               <ns2:ShortName>2200 CM3</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DHC00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE FAHRTENSCHREIBER</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DHG00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE RADIOFERNBEDIENUNG</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DHL00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE BETÄTIGUNG SEITENTÜR</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DHU03</ns2:ManufacturerCode>
               <ns2:ShortName>UMKLAPPBARER MANUEL AUS SPIEGEL</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DIN00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE SITZHÖHENEINSTELLUNG BEIFAHRER VORN</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DIP01</ns2:ManufacturerCode>
               <ns2:ShortName>SITZBETAET VORNE MANUELL FAHRER</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DIQ01</ns2:ManufacturerCode>
               <ns2:ShortName>BETAET VORDER SITZ MANUELL BEIFAHR</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DIU00</ns2:ManufacturerCode>
               <ns2:ShortName>RUECKLEHNE BEIFAHRERSITZ FESTSTEHEND</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DJA11</ns2:ManufacturerCode>
               <ns2:ShortName>1 SCHLÜSSEL HOCHFREQUENZ-FERNBEDIENUNG+1 EINZELNER HAUPTSCHLÜSSEL</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DJU00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE SORTIERKASTEN</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DJY00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE NAVIGATIONSSYSTEM</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DKA33</ns2:ManufacturerCode>
               <ns2:ShortName>ABGASNORM EURO5+ (ZULASSUNG)</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DKG00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DLI00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE AFIL SPURASSISTENTEN</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DLL00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE TÜRÖFFNUNG</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DLV00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE ERSATZRAD</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DME00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE HALTERUNG NAVIGATIONSSYSTEM NOMADE</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DNA00</ns2:ManufacturerCode>
               <ns2:ShortName>NICHT HEIZBARER SITZ</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DND00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE SCHEINWERFERWASCHANLAGE</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DNF00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE SEITENAIRBAG</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DNN00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE BEIFAHRER-AIRBAG</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DNR00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE ZUSATZ-KLIMAANLAGE</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DON01</ns2:ManufacturerCode>
               <ns2:ShortName>RUECKSPIEGEL NICHT HEIZBAR</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DPB00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE HINTERTUER</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DPC00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE SEITLICHE SCHIEBETUER</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DPG10</ns2:ManufacturerCode>
               <ns2:ShortName>VORD TUER BETAETIGUNG - DECKENLEUCHTE</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DPQ01</ns2:ManufacturerCode>
               <ns2:ShortName>MONTAGE LEITERTRAEGER</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DPR00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE NEBELSCHEINWERFER</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DPX00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE SCHUTZ FAHRERHAUS VORNE</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DQB01</ns2:ManufacturerCode>
               <ns2:ShortName>NORMALE SPUR HINTEN</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DRE00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE KLIMA-ANLAGE</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DRG00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE TEMPO-MAT</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DRK02</ns2:ManufacturerCode>
               <ns2:ShortName>AUSSENSPIEGEL BEIFAHRER, MANUELL</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DRP01</ns2:ManufacturerCode>
               <ns2:ShortName>MONTAGE STAHL-RAEDER</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DRX02</ns2:ManufacturerCode>
               <ns2:ShortName>RUECKSICHT STANDARD</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DSA01</ns2:ManufacturerCode>
               <ns2:ShortName>RESERVERADHALTER STANDARD</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DUA02</ns2:ManufacturerCode>
               <ns2:ShortName>STAHL-FEDERUNG</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DUB00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE HINDERNISWARNVORRICHTUNG</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DUE00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE ANZEIGE REIFENDRUCKVERLUST</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DVC00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE SCHEIBE HINTEN</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DVG00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE SEITENSHEIBE</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DVH01</ns2:ManufacturerCode>
               <ns2:ShortName>STANDARD-LENKRAD</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DVI00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE SEITENSCHEIBE REIHE 3</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DVQ26</ns2:ManufacturerCode>
               <ns2:ShortName>MECHANISCHES GETRIEBE MLGU6</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DXY00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE ZUSATZHEIZUNG</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DYD00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE ZUGRIFF UND FREIHAND-ANLASSEN</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>DYM00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE HILFSANSCHLUSS AUDIO-SET</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:ManufacturerCode>WHC:VF3</ns2:ManufacturerCode>
               <ns2:ShortName/>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>256</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DDJ04</ns2:ManufacturerCode>
               <ns2:ShortName>FACELIFT</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>814</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DYC00</ns2:ManufacturerCode>
               <ns2:ShortName>OHNE STOP AND START</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>6435</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DCZ07</ns2:ManufacturerCode>
               <ns2:ShortName>NUTZLAST LEICHT 16Q</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>8000</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DCA02</ns2:ManufacturerCode>
               <ns2:ShortName>DOPPELKABINE</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>9000</ns2:AvNumberDat>
               <ns2:ManufacturerCode>B0JGA</ns2:ManufacturerCode>
               <ns2:ShortName>LADEFLAECHE</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>10704</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DPF01</ns2:ManufacturerCode>
               <ns2:ShortName>DACH STANDARD</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>14700</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DAT18</ns2:ManufacturerCode>
               <ns2:ShortName>DACHANTENNE LANG</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>18609</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DEK08</ns2:ManufacturerCode>
               <ns2:ShortName>TAGFAHRLICHT VORN (DRL)</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>19117</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DNB03</ns2:ManufacturerCode>
               <ns2:ShortName>SCHEIBENWISCHER VORN OHNE REGENSENSOR</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>20011</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DED16</ns2:ManufacturerCode>
               <ns2:ShortName>SEITENSCHUTZLEISTEN DURCHGEFAERBT</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>20404</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DPE02</ns2:ManufacturerCode>
               <ns2:ShortName>MIT SCHMUTZFAENGER HINTEN</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>20411</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DGL01</ns2:ManufacturerCode>
               <ns2:ShortName>MIT PLATTE</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>21604</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DPD53</ns2:ManufacturerCode>
               <ns2:ShortName>STOSSFÄNGER VO STANDARD NEUTRAL</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>22008</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DVD02</ns2:ManufacturerCode>
               <ns2:ShortName>GETOENT</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>22513</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DVF10</ns2:ManufacturerCode>
               <ns2:ShortName>WSS WERBUNDGLAS + SEITLICHE UND HINTERE GEHAERTET</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>24407</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DRC29</ns2:ManufacturerCode>
               <ns2:ShortName>4 LAUTSPRECHER OHNE RADIO</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>25022</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DJI01</ns2:ManufacturerCode>
               <ns2:ShortName>VORBEREITUNG BATTERIE-KABEL</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>26801</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DSH02</ns2:ManufacturerCode>
               <ns2:ShortName>AIRBAG FAHRERSEITE</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>29404</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DNS01</ns2:ManufacturerCode>
               <ns2:ShortName>GAS VORWAERMER GEHAEUSE</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>32203</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DAX01</ns2:ManufacturerCode>
               <ns2:ShortName>BEIFAHRER 2 ER SITZBANK</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>32203</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DWM06</ns2:ManufacturerCode>
               <ns2:ShortName>SITZBANK MIT MITTLEREM 3-PUNKT-GURT</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>32704</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DRH11</ns2:ManufacturerCode>
               <ns2:ShortName>REGULIERBARE EIHOEHUNG VO /HI</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>32806</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DJB02</ns2:ManufacturerCode>
               <ns2:ShortName>MONTAGE MIT VORDERER ARMLEHNE FAHRER</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>33208</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DAX01</ns2:ManufacturerCode>
               <ns2:ShortName>BEIFAHRER 2 ER SITZBANK</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>33303</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DIT02</ns2:ManufacturerCode>
               <ns2:ShortName>EINSTELLUNG LENDENWIRBELSTUETZE FAHRERSITZ</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>35301</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DVB09</ns2:ManufacturerCode>
               <ns2:ShortName>ZENTRALVERRIEGELUNG EINFACH + AUTOMATISCH</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>37808</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DJO01</ns2:ManufacturerCode>
               <ns2:ShortName>MIT HAUBE</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>40799</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DUG01</ns2:ManufacturerCode>
               <ns2:ShortName>MIT BREMSASSISTENT</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>42502</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DSE08</ns2:ManufacturerCode>
               <ns2:ShortName>VERSTAERKTE AUFHAENGUNG HI</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>69800</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DDD02</ns2:ManufacturerCode>
               <ns2:ShortName>NICHT VARIABLE SERVOLENKUNG</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>70303</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DUF01</ns2:ManufacturerCode>
               <ns2:ShortName>DYNAMISCHE STABILITAETSKONTROLLE</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>70308</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DUF01</ns2:ManufacturerCode>
               <ns2:ShortName>DYNAMISCHE STABILITAETSKONTROLLE</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>75205</ns2:AvNumberDat>
               <ns2:ManufacturerCode>B0G06</ns2:ManufacturerCode>
               <ns2:ShortName>BVM6</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>75220</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DBMAR</ns2:ManufacturerCode>
               <ns2:ShortName>BVM6 MLGUC14</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>76502</ns2:AvNumberDat>
               <ns2:ManufacturerCode>B0G06</ns2:ManufacturerCode>
               <ns2:ShortName>BVM6</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>77005</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DUW01</ns2:ManufacturerCode>
               <ns2:ShortName>PARTIKELFILTER</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>77403</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DNO01</ns2:ManufacturerCode>
               <ns2:ShortName>KRAFTSTOFFTANK 90 LITER</ns2:ShortName>
            </ns2:VINEquipment>
            <ns2:VINEquipment>
               <ns2:AvNumberDat>78090</ns2:AvNumberDat>
               <ns2:ManufacturerCode>DCK02</ns2:ManufacturerCode>
               <ns2:ShortName>KALTE LAENDER</ns2:ShortName>
            </ns2:VINEquipment>
         </ns2:VINEquipments>
         <ns2:VINColors>
            <ns2:VINColor>
               <ns2:ColorID>A1</ns2:ColorID>
               <ns2:Code>B0NWP/B0MP0/EWP</ns2:Code>
               <ns2:Description>LACK WEISS BANQUISE/DECKENDE LACKIERUNG</ns2:Description>
            </ns2:VINColor>
         </ns2:VINColors>
         <ns2:VINVehicle>
            <ns2:ManufacturerCarCode/>
            <ns2:ManufacturerEngineCode/>
            <ns2:ManufacturerTransmissionCode/>
         </ns2:VINVehicle>
      </ns2:VINResult>
      <ns2:MetaPositions>
         <ns2:MetaPosition key="additionalVehicle" value="4: 026701050100000,5416"/>
      </ns2:MetaPositions>
   </ns2:Vehicle>
</additionalInformation>
```
