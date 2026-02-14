---
title: "Änderung der Vererbung der Stundenlöhne für die Arbeitslohnfaktoren"
topic_id: "30660"
breadcrumb: "Technische Informationen > Ausgabe Nr. 92 August 2025 > Reparaturkostenkalkulation > SilverDAT 3 PRO > Abkündigungen > Änderung der Vererbung der Stundenlöhne für die Arbeitslohnfaktoren"
---

# Änderung der Vererbung der Stundenlöhne für die Arbeitslohnfaktoren

Wichtige Änderung!

Bitte beachten Sie, dass nach Ablauf der 6-monatigen Abkündigungsfrist eine wichtige
Änderung bei der Vererbung der Stundenlöhne für die Arbeitslohnfaktoren umgesetzt
wird.

Aktueller Stand:

Derzeit erfolgt bei der Übergabe von Arbeitslohnfaktoren (Mechanik, Karosserie, Elektrik)
keine automatische Vererbung des Stundenlohns auf weitere Stufen, selbst wenn mindestens
eines der Felder in Stufe 1, Stufe 2 oder Stufe 3 übermittelt wird.

Änderung mit dem Dezember Release 2025:

Ab dem Dezember Release 2025 wird eine automatische Vererbung des Stundenlohns auf
alle weiteren Stufen erfolgen, sobald mindestens eines der Felder in Stufe 1, Stufe
2 oder Stufe 3 übergeben wird.

Bitte beachten Sie, dass wenn keine Übergabe von Lohnfaktoren erfolgt, werden diese
auch weiterhin vom Standardverrechnungssatz übernommen.

Bitte berücksichtigen Sie dies in Ihrer eigenen Implementierung. Führen Sie, wenn
nötig, rechtzeitig entsprechende Anpassungen durch!
