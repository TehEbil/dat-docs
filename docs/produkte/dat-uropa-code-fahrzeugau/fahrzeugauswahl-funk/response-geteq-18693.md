---
title: "Response getEquipmentsForUniversalSubType"
topic_id: "18693"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugauswahl - Funktionen > getEquipmentsForUniversalSubType > Response getEquipmentsForUniversalSubType"
---

# Response getEquipmentsForUniversalSubType

(in Ausschnitten)

```
{ "subModels":
  [ { "datSubModelId": 1, "description": "basis"
    }
  , { "datSubModelId": 3, "description": "design"
    }
  , { "datSubModelId": 2, "description": "sport"
    }
  ]
, "equipments":
  [ { "datEquipmentId": 23605, "description": "1-K-Kleber für Seitenscheibe(n)"
    , "subModels": [1,2,3]
    }
  , { "datEquipmentId": 1201
    , "description": "Ablage-Paket", "subModels": [1,2,3]
    }
  , /* … more …*/
  , { "datEquipmentId": 4305, "description": "Ausstattungs-Paket: S line Sport-Paket \/ Plus"
    , "subModels": [2]
    }
  , { "datEquipmentId": 4317, "description": "Ausstattungs-Paket: S line Style"
    , "subModels": [2,3]
    }
    /* … more … */
  , { "datEquipmentId": 35301, "description": "Zentralverriegelung mit Fernbedienung"
    , "subModels": [1,2,3]
    }
  ]
}
```
