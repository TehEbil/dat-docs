---
title: "Mögliche Fehlercodes getVinByOcr"
topic_id: "2024"
breadcrumb: "SilverDAT Produkte > DAT €uropa-Code® Fahrzeugauswahl > Fahrzeugidentifikation - Funktionen > Erkennung einer VIN mit OCR > Mögliche Fehlercodes getVinByOcr"
---

# Mögliche Fehlercodes getVinByOcr

| Rückgabecode | Fehlertext | Beschreibung |
| --- | --- | --- |
| valueNotFound | missing parameter imageBase64 | Wenn der Parameter "imageBase64" fehlt oder leer ist. |
| base64NotValid | imageBase64 is not a valid Base64 encoded string | Wenn der Inhalt von imageBase64 nicht als Base64-kodierte Binärdaten erkannt wurde. |
| imageNotValid | imageBase64 couldn't be recognized as an image | Wenn der Inhalt von imageBase64 nicht in ein Bild konvertiert werden konnte. |
| vinOcrError | The optical VIN recognition didn't work | Die optische VIN-Erkennung hat nicht funktioniert. |
| vinOcrNotSuccessfully | The optical VIN recognition wasn't able to recognize any letters | Die optische VIN-Erkennung hat keine Zeichen finden können. |
