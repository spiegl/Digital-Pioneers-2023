# Übung Schleifen

Erstellen Sie die Skripts für die Aufgaben im head-Tag Ihres HTML-Dokumentes.

## Aufgabe1: Einfache Schleifen

Ihre Seite soll auf Knopfdruck unterschiedliche Schleifen durchlaufen und das Ergebnis in einem `div`-Element ausgeben (
verwenden Sie die `innerHTML`- Eigenschaft des `div`-Elements).
Ein Screenshot Ihrer Seite könnte folgendermassen aussehen (das `div`-Element enthält noch keinen Inhalt und ist deshalb
nicht zu sehen).

![](.resources/schleifen00.png)

Implementieren Sie für jeden Button eine Funktion die folgendes ausführt:

**Schleife1**: For-Schleife zählt von 1 bis 20 in Einserschritten hoch. Bei jedem Schleifendurchlauf wird an eine
Zeichenkettenvariable der Wert des Schleifenzählers hinzugefügt mit einem nachfolgenden Leerraum. Nach Abschluss der
Schleife setzen Sie die `innerHTML`-Eigenschaft des `div`-Elements. Ihre Seite hat dann folgendes Aussehen.

![](.resources/schleifen01.png)

**Schleife2**: Wie Schleife1, allerdings ist der Startwert 10, der Endwert 200 und das Inkrement 10.

![](.resources/schleifen02.png)

**Schleife3**: Wie Schleife1, allerdings soll an den Ausgabe-String der Schleifenzähler multipliziert mit 10 hinzugefügt
werden. Somit sollte die Ausgabe gleich wie bei Schleife2 sein.

**Schleife1a bis 3a:** Gleiche Funktionalität wie bei den ersten drei Schleifen, allerdings verwenden Sie eine `while`
-Schleife (kopf- oder fussgesteuert).

## Aufgabe2: Schleife flexibel

Ihre Seite soll dem Benutzer die Eingabe eines Startwertes, eines Endwertes und eines Inkrementes erlauben.

![](.resources/schleifen03.png)

Bei Klick auf den Button Ausgabe soll eine entsprechende For-Schleife ausgeführt werden und analog der ersten Aufgabe
die Werte ausgegeben werden.

Beachten Sie folgende Punkte:

- Um die Werte der Eingabefelder in der Schleife verwenden zu können, müssen Sie diese mit `parseInt(...)` in Zahlen
  konvertieren.
- Prüfen Sie, ob der Benutzer gültige Zahlen eingegeben hat (Funktion `isNaN(...)`). Auch ein Inkrement von 0 soll nicht
  erlaubt sein. Weisen Sie den Benutzer auf etwaige Eingabefehler hin.
- Um das ganze einfacher zu halten, prüfen Sie, ob das Inkrement eine negative Zahl ist. Trifft dies zu, so wandeln Sie
  das Inkrement in eine positive Zahl um (Multiplikation mit -1).
- Ist der Startwert grösser als der Endwert, so muss Ihre Schleife anders aufgebaut werden (`if`-Anweisung).

## Aufgabe3: Dreieck aus Sternen

Sie bauen eine Seite, die folgendermassen aussieht:

![](.resources/schleifen04.png)

Bei Klick auf die Schaltfläche Dreieck soll ein Dreieck aus Sternen gebaut werden. Um das Dreieck anzuzeigen, befindet
sich unterhalb der Schaltflächen noch ein `div`-Bereich, dessen `innerHTML`-Eigenschaft das Dreieck anzeigt.

Der Benutzer hat die Möglichkeit anzugeben, aus wie vielen Zeilen das Dreieck bestehen soll. Verwenden Sie eine
For-Schleife, um eine Zeichenkette zusammenzustückeln, die alle Sterne enthält.

**Hinweis**: um die Optik zu verbessern, wurde zwischen den Sternen mit der HTML- Entity `&nbsp;` gearbeitet (siehe auch
Unterlagen auf der Plattform).
Die Ausgabe könnte so aussehen:

![](.resources/schleifen05.png)

## Aufgabe4: Schachbrett aus Sternen

Verwenden Sie die in Aufgabe3 erstellte Seite. Bei Klick auf die Schaltfläche Schachbrett soll ein Schachbrett aus
Sternen aufgebaut werden.

**Hinweis**: Verwenden Sie zwei geschachtelte For-Schleifen. Die äussere Schleife steuert die Zeilen, die innere das
Zusammenhängen der Zeichen innerhalb einer Zeile. Ist die Summe aus äusserem und innerem Schleifenzähler eine gerade
Zahl, so hängen Sie einen Stern an Ihre Zeichenkette, ansonsten ein Leerzeichen (verwenden Sie `&nbsp;` für die Ausgabe
der Leerzeichen).

![](.resources/schleifen06.png)

Beachten Sie weiters, dass nur eine gerade Zahl im Feld Anzahl Zeilen erlaubt sein soll, damit das Schachbrett korrekt
aufgebaut wird.

