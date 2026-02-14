---
title: "Zugriff vom Webbrowser aus"
topic_id: "27903"
breadcrumb: "Data Entry Tool (DET) - Schnittstelle zum Datenabruf > Data Entry Tool (DET) 2026 - Schnittstelle zum Datenabruf > Anmeldung > Zugriff vom Webbrowser aus"
---

# Zugriff vom Webbrowser aus

Wenn die Schnittstelle direkt von einer Web-Anwendung aus dem Web-Browser heraus aufgerufen
wird, speichern Sie keine Zugangsdaten im Session-Storage, sondern nur den Zugangs-Token.

Wenn dieser Zugangs-Token abgelaufen ist, dann verwenden Sie den Refresh-Token, der
auch von der Login-Funktion zurückgegeben wurde, um den Zugangs-Token zu erneuern.
Der Refresh-Token ist einige Stunden lang gültig. Die Login-Funktion liefert den Refresh-Token
als HTTP-only-Cookie zurück, so dass er im Browser nicht von JavaScript gelesen werden
kann und so einen Schutz gegen Cross-Site-Scripting-Angriffe (XSS) bietet. Wenn Sie
vom Browser aus die Refresh-Funktion aufrufen, wird der Browser automatisch diesen Cookie mitgeben, und die Funktion
wird einen neuen Zugangs-Token zurückliefern.

Sollte der Refresh-Token abgelaufen sein, dann meldet die Refresh-Funktion den HTTP-Fehler 401, und es ist einen neue Anmeldung mittels der Benutzer-Zugangsdaten
nötig.

Anfragen mit gültigem Token aber mangelnder Berechtigung werden mit einem HTTP-Fehler
403 ("Zugriff verweigert") beantwortet.
