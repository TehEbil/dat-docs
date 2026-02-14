---
title: "Response getEquipmentAttributes"
topic_id: "15094"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Ermittlung der Ausstattungsmerkmale > Response getEquipmentAttributes"
---

# Response getEquipmentAttributes

```
{
[
  {
    "name": "Motor",
    "functionGroups": [
      {
        "features": [
          {
            "name": "Motorbauart",
            "attributes": [
              {
                "propertyName": "Diesel",
                "property": 183,
                "position": "SERIES"
              }
            ],
            "key": 1001
          }
        ],
        "name": "Motorbauart",
        "key": 110
      },
      {
        "features": [
          {
            "name": "Motoraufladung",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 1015
          },
          {
            "name": "Start/Stopp-Anlage",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 1022
          }
        ],
        "name": "Motortechnik",
        "key": 130
      },
      {
        "features": [
          {
            "name": "Partikelfilter",
            "attributes": [
              {
                "propertyName": "Diesel",
                "property": 183,
                "position": "SERIES"
              }
            ],
            "key": 1035
          },
          {
            "name": "Emissionsklasse",
            "attributes": [
              {
                "propertyName": "Euro",
                "precision": "0",
                "property": 1336,
                "position": "SERIES",
                "value": "6"
              }
            ],
            "key": 1034
          }
        ],
        "name": "Abgasanlage/-reinigung",
        "key": 160
      }
    ],
    "key": 1
  },
  {
    "name": "Kraftübertragung",
    "functionGroups": [
      {
        "features": [
          {
            "name": "Getriebebauart",
            "attributes": [
              {
                "propertyName": "Schaltgetriebe",
                "property": 658,
                "position": "SERIES"
              }
            ],
            "key": 2014
          },
          {
            "name": "Getriebemerkmale",
            "attributes": [
              {
                "propertyName": "Gänge/Stufen Anzahl",
                "precision": "0",
                "property": 311,
                "position": "SERIES",
                "value": "6"
              }
            ],
            "key": 2015
          }
        ],
        "name": "Wechselgetriebe",
        "key": 240
      },
      {
        "features": [
          {
            "name": "Vorderradantrieb",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 2002
          }
        ],
        "name": "Antriebsart",
        "key": 210
      },
      {
        "features": [
          {
            "name": "Differentialsperre",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "elektronisch",
                "property": 252,
                "position": "SERIES"
              }
            ],
            "key": 2005
          }
        ],
        "name": "Radantrieb",
        "key": 220
      }
    ],
    "key": 2
  },
  {
    "name": "Achsen, Fahrwerk",
    "functionGroups": [
      {
        "features": [
          {
            "name": "Feststellbremse",
            "attributes": [
              {
                "propertyName": "elektrisch",
                "property": 239,
                "position": "SERIES"
              }
            ],
            "key": 3015
          }
        ],
        "name": "Bremsanlage",
        "key": 320
      },
      {
        "features": [
          {
            "name": "Servolenkung",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "elektronisch geregelt",
                "property": 253,
                "position": "SERIES"
              }
            ],
            "key": 3042
          }
        ],
        "name": "Lenkung",
        "key": 360
      },
      {
        "features": [
          {
            "name": "Felgen",
            "attributes": [
              {
                "propertyName": "Leichtmetall",
                "property": 435,
                "position": "SPECIAL"
              }
            ],
            "key": 3044
          },
          {
            "name": "Felgengröße Vorderachse",
            "attributes": [
              {
                "propertyName": "Felgenbreite Zoll",
                "precision": "2",
                "property": 283,
                "position": "SPECIAL",
                "value": "6.5"
              },
              {
                "propertyName": "Felgendurchmesser Zoll",
                "precision": "1",
                "property": 284,
                "position": "SPECIAL",
                "value": "16"
              }
            ],
            "key": 3047
          },
          {
            "name": "Felgengröße Hinterachse",
            "attributes": [
              {
                "propertyName": "Felgenbreite Zoll",
                "precision": "2",
                "property": 283,
                "position": "SPECIAL",
                "value": "6.5"
              },
              {
                "propertyName": "Felgendurchmesser Zoll",
                "precision": "1",
                "property": 284,
                "position": "SPECIAL",
                "value": "16"
              }
            ],
            "key": 3049
          }
        ],
        "name": "Räder",
        "key": 370
      }
    ],
    "key": 3
  },
  {
    "name": "Karosserie, Exterieur",
    "functionGroups": [
      {
        "features": [
          {
            "name": "Nebelscheinwerfer Dekor",
            "attributes": [
              {
                "propertyName": "Chrom/-optik",
                "property": 164,
                "position": "SPECIAL"
              }
            ],
            "key": 8290
          },
          {
            "name": "Stoßfänger lackiert",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 4057
          },
          {
            "name": "Stoßleisten seitlich",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "schwarz",
                "property": 678,
                "position": "SERIES"
              }
            ],
            "key": 4056
          },
          {
            "name": "Zierleisten Verglasung",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "schwarz",
                "property": 678,
                "position": "SERIES"
              }
            ],
            "key": 4054
          }
        ],
        "name": "Exterieurdetails",
        "key": 416
      },
      {
        "features": [
          {
            "name": "Außenspiegelgehäuse",
            "attributes": [
              {
                "propertyName": "lackiert/glänzend",
                "property": 475,
                "position": "SERIES"
              }
            ],
            "key": 4041
          },
          {
            "name": "Außenspiegel mit Abblendautomatik",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "links",
                "property": 516,
                "position": "SERIES"
              }
            ],
            "key": 9057
          },
          {
            "name": "Außenspiegelglas asphärisch",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "links",
                "property": 516,
                "position": "SERIES"
              }
            ],
            "key": 9508
          },
          {
            "name": "Außenspiegelverstellung elektrisch",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 9055
          },
          {
            "name": "Außenspiegelheizung",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 9056
          }
        ],
        "name": "Außenspiegel",
        "key": 412
      },
      {
        "features": [
          {
            "name": "Heckklappe/-deckel",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "Fernentriegelung",
                "property": 294,
                "position": "SERIES"
              }
            ],
            "key": 4067
          },
          {
            "name": "Türgriffe seitlich außen",
            "attributes": [
              {
                "propertyName": "Wagenfarbe",
                "property": 390,
                "position": "SERIES"
              }
            ],
            "key": 9273
          }
        ],
        "name": "Front-/Heckklappe/Türen",
        "key": 418
      },
      {
        "features": [
          {
            "name": "Fahrzeugaufbauart",
            "attributes": [
              {
                "propertyName": "Türen Anzahl",
                "precision": "0",
                "property": 767,
                "position": "SERIES",
                "value": "4"
              }
            ],
            "key": 4001
          }
        ],
        "name": "Karosserie/Aufbauten",
        "key": 408
      },
      {
        "features": [
          {
            "name": "Metallic-/Perleffekt-Lackierung",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SPECIAL"
              },
              {
                "propertyName": "Perleffekt/Mica",
                "property": 612,
                "position": "SPECIAL"
              }
            ],
            "key": 9274
          }
        ],
        "name": "Lackierung/Dekorfolien außen",
        "key": 426
      },
      {
        "features": [
          {
            "name": "Dachreling",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 4096
          }
        ],
        "name": "Transportsysteme",
        "key": 430
      },
      {
        "features": [
          {
            "name": "Fensterheber elektrisch",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "hinten",
                "property": 362,
                "position": "SERIES"
              },
              {
                "propertyName": "vorn",
                "property": 823,
                "position": "SERIES"
              }
            ],
            "key": 8628
          },
          {
            "name": "Wärmeschutzverglasung/getönt",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "Seitenscheibe/n",
                "property": 1060,
                "position": "SERIES"
              },
              {
                "propertyName": "Heckscheibe",
                "property": 1063,
                "position": "SERIES"
              },
              {
                "propertyName": "Frontscheibe",
                "property": 388,
                "position": "SERIES"
              }
            ],
            "key": 4109
          },
          {
            "name": "Verbundverglasung",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "Frontscheibe",
                "property": 388,
                "position": "SERIES"
              }
            ],
            "key": 9280
          },
          {
            "name": "Regensensor",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 9288
          },
          {
            "name": "Scheibenwaschdüsen vorn",
            "attributes": [
              {
                "propertyName": "heizbar",
                "property": 359,
                "position": "SERIES"
              }
            ],
            "key": 9308
          },
          {
            "name": "Scheibenwischanlage hinten",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 9290
          }
        ],
        "name": "Verglasung",
        "key": 434
      }
    ],
    "key": 4
  },
  {
    "name": "Interieur",
    "functionGroups": [
      {
        "features": [
          {
            "name": "Interieurleisten/Zierteile",
            "attributes": [
              {
                "propertyName": "Design",
                "property": 181,
                "position": "SERIES"
              }
            ],
            "key": 5035
          },
          {
            "name": "Innenspiegel mit Abblendautomatik",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 9092
          },
          {
            "name": "Lenkrad",
            "attributes": [
              {
                "propertyName": "Multifunktion/Fernbedienung",
                "property": 583,
                "position": "SPECIAL"
              }
            ],
            "key": 5036
          },
          {
            "name": "Lenkradverstellung",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "höhenverstellbar",
                "property": 373,
                "position": "SERIES"
              },
              {
                "propertyName": "längsverstellbar",
                "property": 492,
                "position": "SERIES"
              }
            ],
            "key": 5028
          },
          {
            "name": "Lenkradkranz",
            "attributes": [
              {
                "propertyName": "Leder",
                "property": 499,
                "position": "SPECIAL"
              }
            ],
            "key": 5038
          },
          {
            "name": "Schalt-/Wählhebelgriff",
            "attributes": [
              {
                "propertyName": "Leder",
                "property": 499,
                "position": "SERIES"
              }
            ],
            "key": 5039
          },
          {
            "name": "Sonnenblende/n mit Spiegel",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "links",
                "property": 516,
                "position": "SERIES"
              },
              {
                "propertyName": "rechts",
                "property": 635,
                "position": "SERIES"
              }
            ],
            "key": 9111
          }
        ],
        "name": "Interieurdetails",
        "key": 530
      },
      {
        "features": [
          {
            "name": "Handschuhfach",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "kühlbar",
                "property": 459,
                "position": "SERIES"
              }
            ],
            "key": 5005
          }
        ],
        "name": "Ablage-/Staufächer innen",
        "key": 510
      },
      {
        "features": [
          {
            "name": "Fußmatten",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SPECIAL"
              },
              {
                "propertyName": "Teppich/Textil",
                "property": 750,
                "position": "SPECIAL"
              }
            ],
            "key": 9633
          }
        ],
        "name": "Bodenbeläge",
        "key": 882
      },
      {
        "features": [
          {
            "name": "Gepäckraumabtrennung/Netz",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 5071
          },
          {
            "name": "Laderaumabdeckung/Rollo",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 5062
          }
        ],
        "name": "Gepäck-/Laderaum",
        "key": 550
      },
      {
        "features": [
          {
            "name": "Aschenbecher",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SPECIAL"
              },
              {
                "propertyName": "vorn (Raucherpaket)",
                "property": 824,
                "position": "SPECIAL"
              }
            ],
            "key": 5009
          },
          {
            "name": "Notfallausrüstung",
            "attributes": [
              {
                "propertyName": "Warndreieck",
                "property": 110,
                "position": "SERIES"
              },
              {
                "propertyName": "Verbandkasten",
                "property": 135,
                "position": "SERIES"
              }
            ],
            "key": 5011
          }
        ],
        "name": "Innenzubehör",
        "key": 520
      },
      {
        "features": [
          {
            "name": "Sitzbezüge",
            "attributes": [
              {
                "propertyName": "Stoff",
                "property": 725,
                "position": "SERIES"
              }
            ],
            "key": 9131
          },
          {
            "name": "Kopfstützen hinten",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "2. Sitzreihe mitte",
                "property": 224,
                "position": "SERIES"
              },
              {
                "propertyName": "2. Sitzreihe außen",
                "property": 341,
                "position": "SERIES"
              }
            ],
            "key": 9209
          },
          {
            "name": "Armauflage/n vorn",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "mitte",
                "property": 554,
                "position": "SERIES"
              }
            ],
            "key": 9135
          },
          {
            "name": "Armauflage/n hinten",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "2. Sitzreihe",
                "property": 9,
                "position": "SERIES"
              }
            ],
            "key": 9168
          }
        ],
        "name": "Sitze",
        "key": 879
      },
      {
        "features": [
          {
            "name": "Sitzheizung",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "Beifahrersitz",
                "property": 117,
                "position": "SERIES"
              },
              {
                "propertyName": "Fahrersitz",
                "property": 268,
                "position": "SERIES"
              }
            ],
            "key": 9112
          },
          {
            "name": "Lendenwirbelstützen",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "Beifahrersitz",
                "property": 117,
                "position": "SERIES"
              },
              {
                "propertyName": "Fahrersitz",
                "property": 268,
                "position": "SERIES"
              }
            ],
            "key": 9119
          },
          {
            "name": "Sitzhöhenverstellung vorn",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "Beifahrersitz",
                "property": 117,
                "position": "SERIES"
              },
              {
                "propertyName": "Fahrersitz",
                "property": 268,
                "position": "SERIES"
              }
            ],
            "key": 9096
          },
          {
            "name": "Sitze umklapp/-versenkbar vorn",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "Beifahrersitz",
                "property": 117,
                "position": "SERIES"
              }
            ],
            "key": 10009
          },
          {
            "name": "Sitze umklapp-/versenkbar Rücksitze",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "2. Sitzreihe",
                "property": 9,
                "position": "SERIES"
              },
              {
                "propertyName": "Fernentriegelung",
                "property": 294,
                "position": "SERIES"
              }
            ],
            "key": 9148
          },
          {
            "name": "Rücksitze geteilt",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 8274
          }
        ],
        "name": "Sitzfunktionen",
        "key": 540
      }
    ],
    "key": 5
  },
  {
    "name": "Beleuchtung",
    "functionGroups": [
      {
        "features": [
          {
            "name": "Lichtfunktionen",
            "attributes": [
              {
                "propertyName": "Einschaltautomatik Fahrlicht",
                "property": 227,
                "position": "SERIES"
              },
              {
                "propertyName": "Abbiegelicht",
                "property": 33,
                "position": "SPECIAL"
              }
            ],
            "key": 6009
          },
          {
            "name": "Lichtbegleitung",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "Coming Home",
                "property": 168,
                "position": "SERIES"
              },
              {
                "propertyName": "Leaving Home",
                "property": 497,
                "position": "SERIES"
              }
            ],
            "key": 9369
          },
          {
            "name": "Nebelscheinwerfer",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SPECIAL"
              }
            ],
            "key": 6010
          },
          {
            "name": "Tagfahrlicht",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 6012
          }
        ],
        "name": "Frontscheinwerfer",
        "key": 610
      },
      {
        "features": [
          {
            "name": "Heckleuchten",
            "attributes": [
              {
                "propertyName": "LED",
                "property": 498,
                "position": "SERIES"
              }
            ],
            "key": 6015
          },
          {
            "name": "Kennzeichenleuchte",
            "attributes": [
              {
                "propertyName": "LED",
                "property": 498,
                "position": "SERIES"
              }
            ],
            "key": 6018
          },
          {
            "name": "Nebelschlußleuchte",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 6019
          }
        ],
        "name": "Heckleuchten",
        "key": 620
      },
      {
        "features": [
          {
            "name": "Blinkleuchten seitlich",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "im Außenspiegel",
                "property": 384,
                "position": "SERIES"
              }
            ],
            "key": 6021
          }
        ],
        "name": "Blinkleuchten",
        "key": 630
      },
      {
        "features": [
          {
            "name": "Fußraumbeleuchtung",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "LED",
                "property": 498,
                "position": "SERIES"
              },
              {
                "propertyName": "vorn",
                "property": 823,
                "position": "SERIES"
              }
            ],
            "key": 6038
          },
          {
            "name": "Kofferraumbeleuchtung",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 6040
          },
          {
            "name": "Leseleuchten vorn",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "LED",
                "property": 498,
                "position": "SERIES"
              }
            ],
            "key": 6042
          },
          {
            "name": "Leseleuchten hinten",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "LED",
                "property": 498,
                "position": "SERIES"
              }
            ],
            "key": 6041
          },
          {
            "name": "Make-up Spiegel-Beleuchtung",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "links",
                "property": 516,
                "position": "SERIES"
              },
              {
                "propertyName": "rechts",
                "property": 635,
                "position": "SERIES"
              }
            ],
            "key": 6037
          }
        ],
        "name": "Innenleuchten",
        "key": 650
      }
    ],
    "key": 6
  },
  {
    "name": "Audio, Navi, Information, Kommunikation",
    "functionGroups": [
      {
        "features": [
          {
            "name": "Audiosystem/Infotainment",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SPECIAL"
              }
            ],
            "key": 7011
          },
          {
            "name": "Antenne Radio/DAB",
            "attributes": [
              {
                "propertyName": "Diversity (Doppelantenne)",
                "property": 190,
                "position": "SERIES"
              }
            ],
            "key": 7019
          },
          {
            "name": "Bordmonitor",
            "attributes": [
              {
                "propertyName": "Display farbig",
                "property": 280,
                "position": "SPECIAL"
              },
              {
                "propertyName": "Touchscreen",
                "property": 758,
                "position": "SPECIAL"
              },
              {
                "propertyName": "Displaygröße Zoll",
                "precision": "2",
                "property": 188,
                "position": "SPECIAL",
                "value": "6.4"
              }
            ],
            "key": 7018
          },
          {
            "name": "Klangausgabe",
            "attributes": [
              {
                "propertyName": "geschwindigkeitsabhängig",
                "property": 330,
                "position": "SPECIAL"
              },
              {
                "propertyName": "Radioleistung Watt",
                "precision": "0",
                "property": 2175,
                "position": "SPECIAL",
                "value": "80"
              }
            ],
            "key": 7022
          },
          {
            "name": "Medienwiedergabe",
            "attributes": [
              {
                "propertyName": "Audiostreaming Bluetooth",
                "property": 79,
                "position": "SPECIAL"
              },
              {
                "propertyName": "CD",
                "property": 160,
                "position": "SPECIAL"
              },
              {
                "propertyName": "MP3",
                "property": 581,
                "position": "SPECIAL"
              },
              {
                "propertyName": "AUX-In",
                "property": 100,
                "position": "SERIES"
              }
            ],
            "key": 7012
          },
          {
            "name": "Onlinefunktionalität",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SPECIAL"
              },
              {
                "propertyName": "Smartphone-Anbindung",
                "property": 956,
                "position": "SPECIAL"
              }
            ],
            "key": 9388
          },
          {
            "name": "USB-Schnittstelle (Media)",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 8490
          }
        ],
        "name": "Infotainment/Connectivity",
        "key": 730
      },
      {
        "features": [
          {
            "name": "Telefonie",
            "attributes": [
              {
                "propertyName": "Freisprecheinrichtung",
                "property": 308,
                "position": "SPECIAL"
              },
              {
                "propertyName": "Bluetooth",
                "property": 491,
                "position": "SPECIAL"
              }
            ],
            "key": 7001
          }
        ],
        "name": "Kommunikation",
        "key": 710
      },
      {
        "features": [
          {
            "name": "Anzeigen",
            "attributes": [
              {
                "propertyName": "Außentemperatur",
                "property": 87,
                "position": "SERIES"
              },
              {
                "propertyName": "Waschwasserstand",
                "property": 842,
                "position": "SERIES"
              }
            ],
            "key": 7007
          },
          {
            "name": "Bordcomputer",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 8749
          }
        ],
        "name": "Fahrzeuginformationen",
        "key": 720
      }
    ],
    "key": 7
  },
  {
    "name": "Funktion, Sicherheit, Komfort",
    "functionGroups": [
      {
        "features": [
          {
            "name": "Wegfahrsperre",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 8007
          }
        ],
        "name": "Diebstahlschutz",
        "key": 810
      },
      {
        "features": [
          {
            "name": "Temperaturregelung",
            "attributes": [
              {
                "propertyName": "Steuerung im Fond",
                "property": 724,
                "position": "SPECIAL"
              },
              {
                "propertyName": "Temperaturzonen Anzahl",
                "precision": "1",
                "property": 864,
                "position": "SPECIAL",
                "value": "3"
              },
              {
                "propertyName": "vollautomatisch",
                "property": 1375,
                "position": "SPECIAL"
              }
            ],
            "key": 8021
          },
          {
            "name": "Klimatisierung",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SPECIAL"
              }
            ],
            "key": 9408
          },
          {
            "name": "Innenraumfilter",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "Aktivkohlefilter",
                "property": 55,
                "position": "SERIES"
              }
            ],
            "key": 8020
          }
        ],
        "name": "Heizung/Klimaanlage",
        "key": 830
      },
      {
        "features": [
          {
            "name": "Berganfahrassistent",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 10028
          },
          {
            "name": "Geschwindigkeitsregelanlage",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SPECIAL"
              }
            ],
            "key": 8035
          }
        ],
        "name": "Komfortfunktionen",
        "key": 840
      },
      {
        "features": [
          {
            "name": "Parksensoren",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SPECIAL"
              },
              {
                "propertyName": "hinten",
                "property": 362,
                "position": "SPECIAL"
              },
              {
                "propertyName": "vorn",
                "property": 823,
                "position": "SPECIAL"
              }
            ],
            "key": 8044
          }
        ],
        "name": "Parken/Rückwärtsfahrt",
        "key": 850
      },
      {
        "features": [
          {
            "name": "ABS",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 8046
          },
          {
            "name": "Anhänger-Stabilisierung-System",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 8047
          },
          {
            "name": "Bremsassistent (Bremsdruckverstärkung)",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 8148
          },
          {
            "name": "ESP/Stabilitätskontrolle",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 8066
          },
          {
            "name": "Fanfare",
            "attributes": [
              {
                "propertyName": "Doppeltonhorn",
                "property": 200,
                "position": "SERIES"
              }
            ],
            "key": 8051
          },
          {
            "name": "Kollisionswarnung",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "Front",
                "property": 1155,
                "position": "SERIES"
              }
            ],
            "key": 8055
          },
          {
            "name": "Mehrfachkollisionsbremse",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 8065
          },
          {
            "name": "Müdigkeitserkennung",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 8057
          },
          {
            "name": "Reifendrucküberwachung",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 10228
          },
          {
            "name": "Traktionskontrolle/ASR",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 8070
          }
        ],
        "name": "Sicherheitssysteme aktiv",
        "key": 860
      },
      {
        "features": [
          {
            "name": "Frontairbag Fahrer",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 8075
          },
          {
            "name": "Frontairbag Beifahrer",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 9128
          },
          {
            "name": "Seitenairbag vorn",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 8084
          },
          {
            "name": "Kopfairbag",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "Beifahrer",
                "property": 113,
                "position": "SERIES"
              },
              {
                "propertyName": "Fahrer",
                "property": 262,
                "position": "SERIES"
              },
              {
                "propertyName": "hinten",
                "property": 362,
                "position": "SERIES"
              }
            ],
            "key": 8082
          },
          {
            "name": "Abschaltvorrichtung Airbag Beifahrer",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 9330
          },
          {
            "name": "Gurtstraffer vorn",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "Beifahrersitz",
                "property": 117,
                "position": "SERIES"
              },
              {
                "propertyName": "Fahrersitz",
                "property": 268,
                "position": "SERIES"
              }
            ],
            "key": 8083
          },
          {
            "name": "Gurtwarnanlage",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "Beifahrersitz",
                "property": 117,
                "position": "SERIES"
              },
              {
                "propertyName": "Fahrersitz",
                "property": 268,
                "position": "SERIES"
              }
            ],
            "key": 8078
          },
          {
            "name": "Kindersitzaufnahme ISOFIX",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "2. Sitzreihe",
                "property": 9,
                "position": "SERIES"
              }
            ],
            "key": 8080
          },
          {
            "name": "Sicherheitsgurte vorn höhenverstellbar",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 10068
          },
          {
            "name": "Sicherheitsgurte hinten",
            "attributes": [
              {
                "propertyName": "mitte 3-Punkt",
                "property": 555,
                "position": "SERIES"
              }
            ],
            "key": 8086
          }
        ],
        "name": "Sicherheitssysteme passiv",
        "key": 870
      },
      {
        "features": [
          {
            "name": "Zentralverriegelung",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              },
              {
                "propertyName": "Fernbedienung",
                "property": 292,
                "position": "SERIES"
              }
            ],
            "key": 8988
          },
          {
            "name": "Schlüssellose Funktionen",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SPECIAL"
              },
              {
                "propertyName": "Start (KeylessGo)",
                "property": 716,
                "position": "SPECIAL"
              },
              {
                "propertyName": "Zugang (KeylessEntry)",
                "property": 865,
                "position": "SPECIAL"
              }
            ],
            "key": 9474
          }
        ],
        "name": "Verriegelung",
        "key": 878
      }
    ],
    "key": 8
  },
  {
    "name": "sonstiges",
    "functionGroups": [
      {
        "features": [
          {
            "name": "Designpaket",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SERIES"
              }
            ],
            "key": 8170
          },
          {
            "name": "Sicherheitspaket",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SPECIAL"
              },
              {
                "propertyName": "Licht",
                "property": 955,
                "position": "SPECIAL"
              },
              {
                "propertyName": "Sicht",
                "property": 1177,
                "position": "SPECIAL"
              }
            ],
            "key": 9333
          },
          {
            "name": "Sitzpaket",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SPECIAL"
              }
            ],
            "key": 8188
          },
          {
            "name": "Winterpaket",
            "attributes": [
              {
                "propertyName": "vorhanden",
                "property": 1,
                "position": "SPECIAL"
              }
            ],
            "key": 9316
          }
        ],
        "name": "Ausstattungspakete",
        "key": 872
      }
    ],
    "key": 10
  }
]
}
```
